# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a><span data-ttu-id="b5673-101">Microsoft Graph を使用して、Python アプリの Excel にアクセスする</span><span class="sxs-lookup"><span data-stu-id="b5673-101">Use Microsoft Graph to access Excel in a Python app</span></span>

<span data-ttu-id="b5673-102">Microsoft Graph API を使用して、OneDrive や SharePoint などのサポートされているオンライン ストレージ プラットフォームに格納されているブックの読み取りと更新を実行できます。</span><span class="sxs-lookup"><span data-stu-id="b5673-102">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The  (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> <span data-ttu-id="b5673-103">`Workbook` (または Excel ファイル) リソースには、他の Excel リソースがすべて含まれおり、アプリはこれらに単純なナビゲーションを使用してアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b5673-103">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The `Workbook` (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> 

<span data-ttu-id="b5673-104">ブックに対して作成、読み取り、更新、削除 (CRUD) 操作を実行するための標準 REST API を使用して、一連の Excel オブジェクト (テーブル、範囲、グラフなど) にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b5673-104">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, </span></span> <span data-ttu-id="b5673-105">たとえば、`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/` では、</span><span class="sxs-lookup"><span data-stu-id="b5673-105">For example:`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="b5673-106">ブックの一部であるワークシート オブジェクトのコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="b5673-106">returns a collection of worksheet objects that are part of the workbook.</span></span>    

<span data-ttu-id="b5673-107">このチュートリアルでは、Python Web アプリから Excel REST API への要求を実行する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b5673-107">This walkthrough describes how to make requests to the Excel REST API from a Python web app.</span></span> 

##  <a name="prerequisites"></a><span data-ttu-id="b5673-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b5673-108">Prerequisites</span></span>

* [<span data-ttu-id="b5673-109">Python 3.5.2</span><span class="sxs-lookup"><span data-stu-id="b5673-109">Python 3.5.2</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="b5673-110">Flask-OAuthlib</span><span class="sxs-lookup"><span data-stu-id="b5673-110">Flask-OAuthlib</span></span>](https://github.com/lepture/flask-oauthlib)
* <span data-ttu-id="b5673-111">[職場または学校のアカウント](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span><span class="sxs-lookup"><span data-stu-id="b5673-111">A [work or school account](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span></span>


## <a name="authorization-and-scopes"></a><span data-ttu-id="b5673-112">承認とスコープ</span><span class="sxs-lookup"><span data-stu-id="b5673-112">Authorization and scopes</span></span>
<span data-ttu-id="b5673-113">[Azure AD v2.0 エンドポイント](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) を使用して Excel REST API 呼び出しを認証できます。</span><span class="sxs-lookup"><span data-stu-id="b5673-113">You can use the [Azure AD v2.0 endpoint](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) to authenticate Excel REST API calls. All APIs require the  HTTP header.</span></span> <span data-ttu-id="b5673-114">すべての API には、`Authorization: Bearer {access-token}` HTTP ヘッダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5673-114">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="b5673-115">Excel リソースを使用するには、次のいずれかの[アクセス許可のスコープ](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5673-115">One of the following [permission scopes](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="b5673-116">Files.Read</span><span class="sxs-lookup"><span data-stu-id="b5673-116">Files.Read</span></span> 
* <span data-ttu-id="b5673-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5673-117">Files.ReadWrite</span></span>

## <a name="sessions-and-persistence"></a><span data-ttu-id="b5673-118">セッションと永続化</span><span class="sxs-lookup"><span data-stu-id="b5673-118">Sessions and persistence</span></span>

<span data-ttu-id="b5673-119">2 つのモードのいずれかで、Excel API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="b5673-119">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="b5673-p104">永続セッション - ブックに加えられたすべての変更は永続化 (保存) されます。これは通常の操作モードです。</span><span class="sxs-lookup"><span data-stu-id="b5673-p104">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="b5673-p105">非永続セッション - API によって加えられた変更は元の場所に保存されません。代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。Excel のセッションの有効期限が切れると、変更は失われます。分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるものの、ドキュメントの状態には影響を与えないアプリには、このモードが便利です。</span><span class="sxs-lookup"><span data-stu-id="b5673-p105">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="b5673-126">API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="b5673-126">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

## <a name="register-the-application-in-azure-active-directory"></a><span data-ttu-id="b5673-127">Azure Active Directory にアプリケーションを登録する</span><span class="sxs-lookup"><span data-stu-id="b5673-127">Register the application in Azure Active Directory</span></span>

<span data-ttu-id="b5673-p106">最初に、アプリケーションを登録し、Microsoft Graph を使用するアクセス許可を設定する必要があります。これにより、ユーザーが職場または学校アカウントでアプリケーションにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="b5673-p106">First, you need to register your application and set permissions to use Microsoft Graph. This lets users sign in to the application with work or school accounts.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="b5673-130">アプリケーションの登録</span><span class="sxs-lookup"><span data-stu-id="b5673-130">Register the application</span></span>

<span data-ttu-id="b5673-p107">Microsoft アプリ登録ポータルでアプリを登録します。これにより、認証するアプリの構成に使用するアプリ ID とパスワードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="b5673-p107">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="b5673-133">個人用アカウントか、職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b5673-133">Sign in to the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="b5673-134">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b5673-134">Choose **Add an app**.</span></span>

3. <span data-ttu-id="b5673-135">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b5673-135">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="b5673-136">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="b5673-136">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="b5673-p108">アプリケーション ID をコピーします。これは、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="b5673-p108">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="b5673-p109">**[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選択します。**[新しいパスワードが生成されました]** ダイアログ ボックスからアプリ シークレットをコピーします。</span><span class="sxs-lookup"><span data-stu-id="b5673-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>

    <span data-ttu-id="b5673-141">アプリを構成するには、アプリケーション ID とアプリ シークレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="b5673-141">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="b5673-142">**[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="b5673-142">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="b5673-143">**[暗黙的フローを許可する]** のチェック ボックスが選択されていることを確認して、アプリのリダイレクト URI を入力します。</span><span class="sxs-lookup"><span data-stu-id="b5673-143">Make sure the **Allow Implicit Flow** check box is selected, and enter your app's Redirect URI.</span></span>

    <span data-ttu-id="b5673-144">**[暗黙的フローを許可する]** オプションにより、OpenID Connect ハイブリッド フローが有効になります。</span><span class="sxs-lookup"><span data-stu-id="b5673-144">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow.</span></span> <span data-ttu-id="b5673-145">これにより、認証時にアプリはサインイン情報 (**id_token**) と成果物 (この場合は認証コード) の両方を受け取れるようになり、アプリはアクセス トークンを取得するときにこれらを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b5673-145">During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app can use to obtain an access token.</span></span>

8. <span data-ttu-id="b5673-146">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b5673-146">Choose **Save**.</span></span>

### <a name="create-oauth-client"></a><span data-ttu-id="b5673-147">OAuth クライアントを作成する</span><span class="sxs-lookup"><span data-stu-id="b5673-147">Create OAuth client</span></span>

<span data-ttu-id="b5673-148">OAuth フローを開始し、アクセス トークンを取得するために使用する Flask-OAuth クライアントのインスタンスをアプリに登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5673-148">Your app needs to register an instance of the Flask-OAuth client that you'll use to start the OAuth flow and get an access token.</span></span> <span data-ttu-id="b5673-149">永続化された変更をサポートする Excel セッションを取得するには、*Files.ReadWrite* スコープが必要であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b5673-149">Note that the *Files.ReadWrite* scope is required to obtain an Excel session that supports persisted changes.</span></span>

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

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a><span data-ttu-id="b5673-150">応答 URL ページで認証コードを受け取る</span><span class="sxs-lookup"><span data-stu-id="b5673-150">Receive an authorization code in your reply URL page</span></span>

<span data-ttu-id="b5673-p112">ユーザーがサインインすると、ブラウザーは応答 URL にリダイレクトされます。承認が成功すると、アクセス トークン (追加の要求を承認するために使用される) が、応答本体で返されます。</span><span class="sxs-lookup"><span data-stu-id="b5673-p112">After the user signs in, the browser is redirected to your reply URL. Upon successful authorization, the access token (which will be used to authorize additional requests) will be returned in the response body.</span></span> 

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

## <a name="make-requests-to-the-excel-api"></a><span data-ttu-id="b5673-153">Excel API への要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="b5673-153">Make requests to the Excel API</span></span>

### <a name="request-headers"></a><span data-ttu-id="b5673-154">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5673-154">Request headers</span></span> 
<span data-ttu-id="b5673-p113">アクセス トークンを使用することにより、あなたのアプリは Microsoft Graph API へ認証された要求を行うことができます。アプリで各要求の **Authorization** ヘッダーにアクセス トークンを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5673-p113">With an access token, your app can make authenticated requests to the Microsoft Graph API. Your app must append the access token to the **Authorization** header of each request.</span></span>

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
```
> <span data-ttu-id="b5673-157">**注**: 要求は **Content-Type** ヘッダーに `application/json` など、Graph API に受け入れられる値も指定して送信します。</span><span class="sxs-lookup"><span data-stu-id="b5673-157">**Note** The request must also send a **Content-Type** header with a value accepted by the Graph API, for example, `application/json`.</span></span>

### <a name="getting-an-excel-session"></a><span data-ttu-id="b5673-158">Excel セッションの取得</span><span class="sxs-lookup"><span data-stu-id="b5673-158">Getting an Excel Session</span></span>
#### <a name="request"></a><span data-ttu-id="b5673-159">要求</span><span class="sxs-lookup"><span data-stu-id="b5673-159">Request</span></span> 

<span data-ttu-id="b5673-160">`persistChanges` 値を `true` または `false` に設定して JSON オブジェクトを渡します。</span><span class="sxs-lookup"><span data-stu-id="b5673-160">Pass a JSON object by setting the `persistChanges` value to `true` or `false`.</span></span> <span data-ttu-id="b5673-161">`persistChanges` の値が `false` に設定された場合に、非永続セッション ID が返されます。</span><span class="sxs-lookup"><span data-stu-id="b5673-161">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span> <span data-ttu-id="b5673-162">この例では、[要求](http://docs.python-requests.org/en/latest/user/quickstart) HTTP ライブラリを使用します。</span><span class="sxs-lookup"><span data-stu-id="b5673-162">This example uses the [Requests](http://docs.python-requests.org/en/latest/user/quickstart) HTTP library</span></span> 

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

#### <a name="response"></a><span data-ttu-id="b5673-163">応答</span><span class="sxs-lookup"><span data-stu-id="b5673-163">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="b5673-164">使用方法</span><span class="sxs-lookup"><span data-stu-id="b5673-164">Usage</span></span> 

<span data-ttu-id="b5673-165">以前の呼び出しから返されたセッション ID は、後続の API 要求で **Workbook-Session-Id** HTTP ヘッダーに入れてヘッダーとして渡します。</span><span class="sxs-lookup"><span data-stu-id="b5673-165">The session ID returned from the previous call is passed as a header on subsequent API requests in the **Workbook-Session-Id** HTTP header. For instance, to list worksheets in that Excel workbook.</span></span> <span data-ttu-id="b5673-166">たとえば、その Excel ブックのワークシートを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b5673-166">For instance, to list worksheets in that Excel workbook.</span></span>

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

#### <a name="response"></a><span data-ttu-id="b5673-167">応答</span><span class="sxs-lookup"><span data-stu-id="b5673-167">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
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

## <a name="next-steps"></a><span data-ttu-id="b5673-168">次の手順</span><span class="sxs-lookup"><span data-stu-id="b5673-168">Next steps</span></span>

<span data-ttu-id="b5673-169">**Workbook-Session-Id** HTTP ヘッダーを使って、データのフェッチ、グラフの作成などを実行するための要求の発行を始めることができます。</span><span class="sxs-lookup"><span data-stu-id="b5673-169">With the **Workbook-Session-Id** HTTP header, you can begin issuing requests to fetch data, create charts, and much more.</span></span> 

* [<span data-ttu-id="b5673-170">一般的な Excel API のシナリオ</span><span class="sxs-lookup"><span data-stu-id="b5673-170">Common Excel API scenarios</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [<span data-ttu-id="b5673-171">Microsoft Graph での Excel の操作</span><span class="sxs-lookup"><span data-stu-id="b5673-171">Working with Excel in Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

<span data-ttu-id="b5673-p116">Microsoft Graph の Excel REST API は、Excel ブック内のデータにアクセスして対話する強力な方法を提供します。Microsoft Graph で他に何ができるかを調べます。</span><span class="sxs-lookup"><span data-stu-id="b5673-p116">The Excel REST API in Microsoft Graph provides a powerful way to access and interact with data in Excel workbooks. Explore what else is possible with Microsoft Graph.</span></span>

* [<span data-ttu-id="b5673-174">Microsoft Graph の概要</span><span class="sxs-lookup"><span data-stu-id="b5673-174">Overview of Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs)
* [<span data-ttu-id="b5673-175">Python アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="b5673-175">Get started with Microsoft Graph in a Python app</span></span>](https://developer.microsoft.com/graph/docs/get-started/python)
