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

コードの最初の数行は、サンプルで使用される Python のモジュールとパッケージの[インポート](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L4-L32)です。

* 標準ライブラリからの **base64** モジュールは、電子メール添付ファイルのエンコードに使用します。
* **mimetypes** モジュールを使用して添付ファイルの MIME の種類を決定します。
* **os** モジュールは、一般的なファイル システムの機能を提供します。
* 標準ライブラリからの **pprint** モジュールは、Graph が返すエラー メッセージを整形出力するのに使用します。 (たとえば、無効な電子メール アドレスに送信する場合。) 
* 標準ライブラリからの **uuid** モジュールは、各 Graph 要求を一意に識別する 36 文字で構成される文字列をランダムに生成するのに使用します。 これは、デバッグに役立ちます。
* **flask** パッケージは、サンプル用の Web フレームワークです。
* **flask_oauthlib.client** の **OAuth** クラスは、OAuth 2.0 認証ワークフローを実装する Flask アプリを包含するラッパーです。
* **config** モジュールには、アプリケーション登録設定 (前述のインストール プロセスで構成した設定など) が含まれます。

次に、[Flask アプリを作成](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L15-L17)してから、**MSGRAPH** という名前の [Graph クライアント オブジェクト](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L19-L28)を作成します。

これらの初期セットアップ手順によって、認証ワークフローを実装する 3 つの Flask ルート ハンドラー関数 [homepage()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L30-L33)、[login()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L35-L39)、[authorized()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L41-L48) が生成されます。 この認証ワークフローの詳細については、Python 認証サンプル リポジトリの「[サンプル アーキテクチャ](https://github.com/microsoftgraph/python-sample-auth#sample-architecture)」セクションをご覧ください。

次のルート ハンドラー [mailform()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L50-L83) は、電子メールの受信者、件名、本文を指定するフォームです。 なお、この関数にはユーザー プロファイルとプロファイル写真の取得、OneDrive への写真のアップロード、共有リンクの作成など、Graph への最初の呼び出しも含まれます。 データは [mailform.html テンプレート](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L77-L83)に渡され、そこでメッセージを送信する前に受信者、件名、本文を編集することができます。 

次は [send_mail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L85-L107) 関数です。この関数は、電子メールを送信し、Graph API からの応答を表示します。 それは sendmail() ヘルパー関数を使用します。この関数には、フォームに入力されたクエリ文字列パラメーターが渡されます。

```python
response = sendmail(client=MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    body=flask.request.args['body'],
                    attachments=[profile_pic])
```

[get_token()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L109-L123) 関数が Flask-OAuthlib クライアント インスタンス (```MSGRAPH```) で使用され、Graph に対する呼び出しが行われるたびにアクセス トークンを取得します。 アクセス トークンは **Authorization** という名前の HTTP ヘッダーで渡されますが、コードでこれを処理する必要はありません。 Graph への呼び出しはクライアントの HTTP verb メソッド (get()、post() など) を介して簡単に行えます。クライアント インスタンスは、トークンを取得するための ```get_token()``` の呼び出しを認識します。この関数が、```tokengetter``` で[修飾](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L109-L109)されているためです。

サンプルの他の部分はヘルパー関数であり、一般的な Graph アクティビティを簡素化するものです。

* [request_headers()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L114-L123) は Graph への各呼び出しによって送信される HTTP ヘッダーのディクショナリを返します。
* [profile_photo()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L125-L154) はユーザーのプロファイル写真を返し、そのコピーをローカル ファイルに保存します。
* [sendmail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L156-L202) は ```me/microsoft.graph.sendMail``` エンドポイントを使用してメッセージを送信します。
* [sharing_link()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L204-L221) は OneDrive で指定されたアイテムの共有リンクを作成します。
* [upload_file()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L223-L255) は OneDrive にファイルをアップロードします。

これらのヘルパー関数は他のアプリケーションで役立つ場合があります。

## <a name="other-python-rest-samples"></a>その他の Python REST サンプル

Microsoft Graph のさまざまな側面の使用方法について、その他の Python サンプルで紹介します。

* [Microsoft Graph 用の Python 認証サンプル](https://github.com/microsoftgraph/python-sample-auth)
* [Python で改ページされた Microsoft Graph 応答を処理する](https://github.com/microsoftgraph/python-sample-pagination)
* [Python で Graph オープン拡張機能を処理する](https://github.com/microsoftgraph/python-sample-open-extensions)
* [Python Web アプリをセキュリティ API に接続する](https://github.com/microsoftgraph/python-security-rest-sample)

ご覧になりたい特定のサンプルがある場合、[懸案事項を送信](https://github.com/microsoftgraph/python-sample-auth/issues)してお知らせください。 Python で構築する Microsoft Graph シナリオに対するお客様のフィードバックを大いに歓迎いたします。

Microsoft Graph API は、あらゆる種類の Microsoft データとの対話に使用できる、非常に強力な統合 API です。 [開発者ドキュメント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/overview)または [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) で、Microsoft Graph によってさらに行える事柄について確認してください。
