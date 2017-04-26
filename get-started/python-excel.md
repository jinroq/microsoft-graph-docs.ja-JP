# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a>Microsoft Graph を使用して、Python アプリの Excel にアクセスする

Microsoft Graph API を使用して、OneDrive や SharePoint などのサポートされているオンライン ストレージ プラットフォームに格納されているブックの読み取りと更新を実行できます。`Workbook` (または Excel ファイル) リソースには、他の Excel リソースがすべて含まれおり、アプリはこれらに単純なナビゲーションを使用してアクセスできます。 

ブックに対して作成、読み取り、更新、削除 (CRUD) 操作を実行するための標準 REST API を使用して、一連の Excel オブジェクト (テーブル、範囲、グラフなど) にアクセスできます。たとえば、`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/` では、  
ブックの一部であるワークシート オブジェクトのコレクションが返されます。    

このチュートリアルでは、Python Web アプリから Excel REST API への要求を実行する方法について説明します。 

##  <a name="prerequisites"></a>前提条件

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* [職場または学校のアカウント](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. -->


## <a name="authorization-and-scopes"></a>承認とスコープ
[Azure AD v.20 エンドポイント](https://graph.microsoft.io/en-us/docs/authorization/converged_auth) を使用して Excel REST API 呼び出しを認証できます。すべての API には、`Authorization: Bearer {access-token}` HTTP ヘッダーが必要です。   
  
Excel リソースを使用するには、次のいずれかの[アクセス許可のスコープ](https://graph.microsoft.io/en-us/docs/authorization/permission_scopes)が必要です。

* Files.Read 
* Files.ReadWrite

## <a name="sessions-and-persistence"></a>セッションと永続化

2 つのモードのいずれかで、Excel API を呼び出すことができます。 

1. 永続セッション - ブックに加えられたすべての変更は永続化 (保存) されます。これは通常の操作モードです。 
2. 非永続セッション - API によって加えられた変更は元の場所に保存されません。代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。Excel のセッションの有効期限が切れると、変更は失われます。分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるものの、ドキュメントの状態には影響を与えないアプリには、このモードが便利です。   

API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。 

## <a name="register-the-application-in-azure-active-directory"></a>Azure Active Directory にアプリケーションを登録する

最初に、アプリケーションを登録し、Microsoft Graph を使用するアクセス許可を設定する必要があります。これにより、ユーザーが職場または学校アカウントでアプリケーションにサインインできるようになります。

### <a name="register-the-application"></a>アプリケーションの登録

Microsoft アプリ登録ポータルでアプリを登録します。これにより、認証するアプリの構成に使用するアプリ ID とパスワードが生成されます。

1. 個人用アカウントか、職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。

2. **[アプリの追加]** を選択します。

3. アプリの名前を入力して、**[アプリケーションの作成]** を選択します。

    登録ページが表示され、アプリのプロパティが一覧表示されます。

4. アプリケーション ID をコピーします。これは、アプリの一意識別子です。

5. **[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選択します。**[新しいパスワードが生成されました]** ダイアログ ボックスからアプリ シークレットをコピーします。

    アプリを構成するには、アプリケーション ID とアプリ シークレットを使用します。

6. **[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。

7. **[暗黙的フローを許可する]** のチェック ボックスが選択されていることを確認して、アプリのリダイレクト URI を入力します。

    **[暗黙的フローを許可する]** オプションにより、OpenID Connect ハイブリッド フローが有効になります。これにより、認証時にアプリはサインイン情報 (**id_token**) と成果物 (この場合は認証コード) の両方を受け取れるようになり、アプリはアクセス トークンを取得するときにこれらを使用できます。

8. **[保存]** を選択します。

### <a name="create-oauth-client"></a>OAuth クライアントを作成する

OAuth フローを開始し、アクセス トークンを取得するために使用する Flask-OAuth クライアントのインスタンスをアプリに登録する必要があります。永続化された変更をサポートする Excel セッションを取得するには、*Files.ReadWrite* スコープが必要であることに注意してください。

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key = client_id,
        consumer_secret = client_secret,
        request_token_params = {'scope': 'User.Read Files.ReadWrite'},
        base_url = 'https://graph.microsoft.com/v1.0/',
        request_token_url = None,
        access_token_method = 'POST',
        access_token_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a>応答 URL ページで認証コードを受け取る

ユーザーがサインインすると、ブラウザーは応答 URL にリダイレクトされます。承認が成功すると、アクセス トークン (追加の要求を承認するために使用される) が、応答本体で返されます。 

```python
    @app.route('/login/authorized')
    def authorized():
        response = microsoft.authorized_response()
        if response is None:
            return "Access Denied: Reason=%s\nError=%s" % (
                request.args['error'], 
                request.args['error_description']
            )
    
        # Check response for state
        if str(session['state']) != str(request.args['state']):
            raise Exception('State has been messed with, end authentication')
        # Remove state session variable to prevent reuse.
        session['state'] = ""
            
        # Okay to store this in a local variable, encrypt if it's going to client
        # machine or database. Treat as a password. 
        session['microsoft_token'] = (response['access_token'], '')
        # Store the token in another session variable for easy access
        session['access_token'] = response['access_token']
```

## <a name="make-requests-to-the-excel-api"></a>Excel API への要求を実行します。

### <a name="request-headers"></a>要求ヘッダー 
アクセス トークンを使用することにより、あなたのアプリは Microsoft Graph API へ認証された要求を行うことができます。アプリで各要求の **Authorization** ヘッダーにアクセス トークンを追加する必要があります。

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
         'Accept' : 'application/json',
         'Content-Type' : 'application/json'
    }
```
> **注**: 要求は **Content-Type** ヘッダーに `application/json` など、Graph API に受け入れられる値も指定して送信します。

### <a name="getting-an-excel-session"></a>Excel セッションの取得
#### <a name="request"></a>要求 

`persistChanges` 値を `true` または `false` に設定して JSON オブジェクトを渡します。`persistChanges` の値が `false` に設定された場合に、非永続セッション ID が返されます。この例では、[要求](http://docs.python-requests.org/en/latest/user/quickstart) HTTP ライブラリを使用します。 

```python
     # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/createSession'
    # Set request headers
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
    # Specify type of session
    body = {
        'persistChanges': True
    }
    
    response = requests.post(url, headers = headers, json = body)
```

#### <a name="response"></a>応答

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201, Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a>使用方法 

以前の呼び出しから返されたセッション ID は、後続の API 要求で **Workbook-Session-Id** HTTP ヘッダーに入れてヘッダーとして渡します。たとえば、その Excel ブックのワークシートを一覧表示します。

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/worksheets'
    # Set request headers - note the session header 
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Workbook-Session-Id': 'cluster=PP1&session=12.a04039942e021.A272...'
    }
    
    response = requests.get(url, headers = headers)
```

#### <a name="response"></a>応答

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets",
    "value": [
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0000-000000000000}",
        "name": "Session 1",
        "position": 0,
        "visibility": "Visible"
    },
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0100-000000000000}",
        "name": "Session 2",
        "position": 1,
        "visibility": "Visible"
    }]
}
```

## <a name="next-steps"></a>次の手順

**Workbook-Session-Id** HTTP ヘッダーを使って、データのフェッチ、グラフの作成などを実行するための要求の発行を始めることができます。 

* [一般的な Excel API のシナリオ](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [Microsoft Graph での Excel の操作](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

Microsoft Graph の Excel REST API は、Excel ブック内のデータにアクセスして対話する強力な方法を提供します。Microsoft Graph で他に何ができるかを調べます。

* [Microsoft Graph の概要](https://developer.microsoft.com/graph/docs)
* [Python アプリで Microsoft Graph を使ってみる](https://developer.microsoft.com/graph/docs/get-started/python)
