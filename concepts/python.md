# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>Python アプリで Microsoft Graph を使ってみる 

この記事では、Azure AD からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。 ここでは、[Python から Microsoft Graph を介してメールを送信する](https://github.com/microsoftgraph/python-sample-send-mail)ためのチュートリアルと、Microsoft Graph API を使用するために実装する主要な概念について説明します。 直接 REST 呼び出しを使用して Microsoft Graph にアクセスする方法について説明します。

![[メールの送信] フォーム](https://raw.githubusercontent.com/microsoftgraph/python-sample-send-mail/master/static/images/sendmail.png)

## <a name="choosing-an-authentication-library"></a>認証ライブラリの選択

Microsoft Graph を呼び出すには、Microsoft クラウドの ID サービスである Azure Active Directory (Azure AD) から有効なアクセス トークンをアプリが取得し、そのトークンが Microsoft Graph REST API に対する各呼び出しの HTTP ヘッダーに渡される必要があります。 Graph での認証方法は OAuth 2.0 と Open ID Connect 標準に基づいているため、アプリケーションで認証を実装するために選択可能な[認証ライブラリ](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-libraries)が多数存在します。

以下に取り上げられているサンプルでは、[Flask-OAuthlib](https://flask-oauthlib.readthedocs.io/en/latest/) ライブラリを使用して OAuth 2.0 [認証コードの付与](https://tools.ietf.org/html/rfc6749#section-4.1)ワークフローを実装しています。これは、Python で書かれた Web アプリケーションで推奨されている認証ワークフローです。 その他の認証オプションについては、「[Microsoft Graph 用の Python 認証サンプル](https://github.com/microsoftgraph/python-sample-auth)」を参照してください。

## <a name="installing-and-running-the-send-mail-sample"></a>メールの送信サンプルのインストールと実行

サンプル アプリをインストールして構成するには、「[Python REST サンプルのインストール](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md)」に記されている説明に従います。 以下で取り上げられているメールの送信サンプル用に、次のコマンドを使用してリポジトリを複製します。

    ```git clone https://github.com/microsoftgraph/python-sample-send-mail.git```

[インストール手順](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md)に記されているように、アプリケーションを登録する際、このサンプルに必要な **User.Read** アクセス許可と **Mail.Send** アクセス許可を必ず含めてください。

インストールと構成の完了後、[サンプルの実行](https://github.com/microsoftgraph/python-sample-send-mail#running-the-sample)に関する説明に従ってサンプル アプリを実行できます。

## <a name="code-walkthrough"></a>コードのチュートリアル

サンプル アプリの[ソース コード](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py)に関する概要を以下に示します。

コードの最初の数行は、サンプルで使用される Python のモジュールとパッケージの [import](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L4-L11) です。

* 標準ライブラリからの **base64** モジュールは、電子メール添付ファイルのエンコードに使用します。
* 標準ライブラリからの **pprint** モジュールは、Graph が返すエラー メッセージを整形出力するのに使用します。 (たとえば、無効な電子メール アドレスに送信する場合。) 
* 標準ライブラリからの **uuid** モジュールは、各 Graph 要求を一意に識別する 36 文字で構成される文字列をランダムに生成するのに使用します。 これは、デバッグに役立ちます。
* **flask** パッケージは、サンプル用の Web フレームワークです。
* **flask_oauthlib.client** の **OAuth** クラスは、OAuth 2.0 認証ワークフローを実装する Flask アプリを包含するラッパーです。
* **config** モジュールには、アプリケーション登録設定 (前述のインストール プロセスで構成した設定など) が含まれます。

次に、[Flask アプリを作成](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L13-L15)してから、**MSGRAPH** という名前の [Graph クライアント オブジェクト](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L17-L26)を作成します。

これの初期セットアップ手順によって、認証ワークフローを実装する 3 つの Flask ルート ハンドラー関数 [homepage()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L28-L31)、[login()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L33-L37)、[authorized()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L39-L46) が生成されます。 この認証ワークフローの詳細については、Python 認証サンプル リポジトリの「[サンプル アーキテクチャ](https://github.com/microsoftgraph/python-sample-auth#sample-architecture)」セクションをご覧ください。

次のルート ハンドラー [mailform()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L48-L54) は、電子メールの受信者、件名、本文を指定するフォームです。 なお、この関数には、Graph への最初の呼び出しも含まれ、現在のユーザーの表示名と電子メール アドレスを取得するための[ユーザー プロファイルの取り出し](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L51-L51)が含まれます。ユーザー プロファイルは [ mailform.html テンプレートに渡されます](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L52-L54)。

次は [send_mail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L56-L73) 関数です。この関数は、電子メールを送信し、Graph API からの応答を表示します。 それは sendmail() ヘルパー関数を使用します。この関数には、フォームに入力されたクエリ文字列パラメーターが渡されます。

```python
response = sendmail(MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    html=flask.request.args['body'])
```

[get_token()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L75-L78) 関数が Flask-OAuthlib クライアント インスタンス (```MSGRAPH```) で使用され、Graph に対する呼び出しが行われるたびにアクセス トークンを取得します。 アクセス トークンは **Authorization** という名前の HTTP ヘッダーで渡されますが、コードでこれを処理する必要はありません。 Graph への呼び出しはクライアントの HTTP verb メソッド (get()、post() など) を介して簡単に行えます。クライアント インスタンスは、トークンを取得するための ```get_token()``` の呼び出しを認識します。この関数が、```tokengetter``` で[修飾](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L75-L75)されているためです。

次の [request_headers()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L80-L85) は、Graph への各呼び出しによって送信される HTTP ヘッダーのディクショナリを返します。

最終的に、電子メールを送信するためのヘルパー関数 [sendmail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L87-L129) が完成しました。 この関数は、Microsoft Graph API で ```me/microsoft.graph.sendMail``` エンドポイントを使用してメッセージを送信します。Microsoft Graph を使用して電子メールを送信する必要がある場合に、この関数をコードでいつでも再使用できます。 この関数の呼び出し方法については、「[docstring](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L88-L97)」を参照してください。

## <a name="other-python-rest-samples"></a>その他の Python REST サンプル

既に取り上げたサンプルに加え、次のサンプルにも、Python からの他の Microsoft Graph 機能の処理方法が示されています。

* [Microsoft Graph 用の Python 認証サンプル](https://github.com/microsoftgraph/python-sample-auth)
* [Python で改ページされた Microsoft Graph 応答を処理する](https://github.com/microsoftgraph/python-sample-pagination)
* [Python で Graph オープン拡張機能を処理する](https://github.com/microsoftgraph/python-sample-open-extensions)

表示したい特定のサンプルがある場合、[懸案事項を送信](https://github.com/microsoftgraph/python-sample-auth/issues)してお知らせください。 Python で構築する Microsoft Graph シナリオに対するお客様のフィードバックを大いに歓迎いたします。

Microsoft Graph API は、あらゆる種類の Microsoft データとの対話に使用できる、非常に強力な統合 API です。 [開発者ドキュメント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/overview)または [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) で、Microsoft Graph によってさらに行える事柄について確認してください。
