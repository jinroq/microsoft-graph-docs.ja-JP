# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a>Node.js アプリで Microsoft Graph を使ってみる

この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[Node.js 用の Microsoft Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)の構築手順と、Microsoft Graph を使用するために実装する主要な概念について説明します。この記事では、生の REST 呼び出しを使用して Microsoft Graph API にアクセスする方法について説明します。

次の画像は、作成するアプリを示しています。 

![ログイン後に [メールの送信] ボタンを表示する Web アプリ](./images/web-screenshot.png)


**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/en-us/getting-started)」を使用すれば、すばやく稼働させることができます。

Azure AD エンドポイントを使用するバージョンの Connect サンプルをダウンロードするには、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth)」をご覧ください。


## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

- [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)
- [npm 付きの Node.js](https://nodejs.org/en/download/) 
- [Node.js 用 Microsoft Connect のサンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)このチュートリアルには、サンプル ファイル内の **starter-project** フォルダーを使用します。

## <a name="register-the-application"></a>アプリケーションの登録
Microsoft アプリケーション登録ポータルでアプリケーションを登録します。これにより、アプリを Visual Studio で構成する際に使用するアプリ ID とパスワードが生成されます。

1. 個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。

2. **[アプリの追加]** を選択します。

3. アプリの名前を入力して、**[アプリケーションの作成]** を選択します。 
    
    登録ページが表示され、アプリのプロパティが一覧表示されます。

4. アプリケーション ID をコピーします。これは、アプリの一意識別子です。 

5. **[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選びます。**[新しいパスワードが生成されました]** ダイアログからパスワードをコピーします。

    アプリを構成するには、アプリケーション ID とアプリケーション パスワード (シークレット) を使用します。 

6. **[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。

7. リダイレクト URI には、*http://localhost:3000/token* と入力します。 

8. **[保存]** を選択します。


## <a name="configure-the-project"></a>プロジェクトを構成する
1. サンプル ファイル内の **starter-project** フォルダーを開きます。

1. コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。これにより、プロジェクトの依存関係がインストールされます。

        npm install

1. スターター プロジェクト ファイル内の utils\config.js を開きます。


1. **credentials** フィールド内の **ENTER\_YOUR\_CLIENT\_ID** プレースホルダーと **ENTER\_YOUR\_SECRET** プレースホルダーの値を、直前にコピーした値に置き換えます。

  
## <a name="authenticate-the-user-and-get-an-access-token"></a>ユーザーの認証とアクセス トークンの取得
この手順では、サインインとトークンの管理コードを追加します。しかし、まず認証フローをさらに詳しく見てみましょう。

このアプリは、委任されたユーザー ID で認証コードの付与フローを使用します。Web アプリケーションのフローでは、登録したアプリのアプリケーション ID、シークレット、およびリダイレクト URI が必要です。 

認証フローは、以下の基本的な手順に分けることができます。

1. 認証と同意のためにユーザーをリダイレクトする
2. 認証コードを取得する
3. 認証コードをアクセス トークンに交換する
4. アクセス トークンの有効期限が切れたら、更新トークンを使用して新しいアクセス トークンを取得する

アプリは [oauth](https://www.npmjs.com/package/oauth) ミドルウェアを使用して認証し、トークンを取得します。アプリは [cookie-parser](https://www.npmjs.com/package/cookie-parser) ミドルウェアを使用して、トークン情報をクッキーにキャッシュします。トークン情報の格納とアクセスに使用されるコードは、index.js コントローラーにあります。
    
   >**重要** このプロジェクトでは、サンプルの目的で単純な認証とトークンの処理を使用しているに過ぎません。運用アプリでは、検証やセキュリティで保護されたトークンの処理など、認証を処理するためのより信頼性の高い方法を構築する必要があります。

これで、Microsoft Graph を呼び出すためのコードを追加する準備が整いました。 

## <a name="call-microsoft-graph"></a>Microsoft Graph を呼び出す
アプリは Microsoft Graph を呼び出してユーザー情報を取得し、ユーザーの代わりにメールを送信します。これらの呼び出しは UI イベントに応答して index.js コントローラーから始まります。

1. utils\graphHelper.js を開きます。

1. **getUserData** 関数を、以下のコードに置き換えます。これにより GET 要求を構成して */me* エンドポイントに送信し、応答を処理します。

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. **getProfilePhoto** 関数を次のコードに置き換えます。これにより、GET 要求を構成して */me/photo/$value* エンドポイントに送信し、応答を処理します。現在、プロフィール写真は MSA アカウントで使用できないことにご注意ください。
    
        function getProfilePhoto(accessToken, callback) {
          // Get the profile photo of the current user (from the user's mailbox on Exchange Online).
          // This operation in version 1.0 supports only work or school mailboxes, not personal mailboxes.
          request
           .get('https://graph.microsoft.com/v1.0/me/photo/$value')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             // Returns 200 OK and the photo in the body. If no photo exists, returns 404 Not Found.
             callback(err, res.body);
           });
        }

1. **uploadFile** 関数を次のコードに置き換えます。これにより、PUT 要求を構成して */me/drive/root/children/mypic.jpg/content* エンドポイントに送信します。ファイルが存在する場合、この要求によってコンテンツが更新されます。存在しない場合、ファイルが作成され、プロフィール写真のコンテンツがアップロードされます。 

        function uploadFile(accessToken, file, callback) {
          // This operation only supports files up to 4MB in size.
          // To upload larger files, see `https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/item_createUploadSession`.
          request
           .put('https://graph.microsoft.com/v1.0/me/drive/root/children/mypic.jpg/content')
           .send(file)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'image/jpg')
           .end((err, res) => {
             // Returns 200 OK and the file metadata in the body.
             callback(err, res.body);
           });
        }

1. **getSharingLink** 関数を次のコードに置き換えます。これにより、GET 要求を構成して */me/drive/items/{file id}/createLink* エンドポイントに送信し、結果を処理します。結果はメッセージに含まれるファイルへの共有リンクになります。

        function getSharingLink(accessToken, id, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/drive/items/' + id + '/createLink')
           .send({ type: 'view' })
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .end((err, res) => {
             // Returns 200 OK and the permission with the link in the body.
             callback(err, res.body.link);
           });
        }

1. **postSendMail** 関数を次のコードに置き換えます。これにより POST 要求を構成して */me/sendMail* エンドポイントに送信し、応答を処理します。

        function postSendMail(accessToken, message, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/sendMail')
           .send(message)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .set('Content-Length', message.length)
           .end((err, res) => {
             // Returns 202 if successful.
             // Note: If you receive a 500 - Internal Server Error
             // while using a Microsoft account (outlook.com, hotmail.com or live.com),
             // it's possible that your account has not been migrated to support this flow.
             // Check the inner error object for code 'ErrorInternalServerTransientError'.
             // You can try using a newly created Microsoft account or contact support.
             callback(err, res);
           });
        }

1. utils\emailer.js を開きます。

1. **wrapEmail** 関数を次のコードに置き換えます。これにより、送信するメール メッセージを表すペイロードを構築します。

        function wrapEmail(content, recipient, file) {
          const attachments = [{
            '@odata.type': '#microsoft.graph.fileAttachment',
            ContentBytes: file,
            Name: 'mypic.jpg'
          }];
          const emailAsPayload = {
            Message: {
              Subject: 'Welcome to Microsoft Graph development with Node.js and the Microsoft Graph Connect sample',
              Body: {
                ContentType: 'HTML',
                Content: content
              },
              ToRecipients: [
                {
                  EmailAddress: {
                    Address: recipient
                  }
                }
              ]
            },
            SaveToSentItems: true,
            Attachments: attachments
          };
          return emailAsPayload;
        }

## <a name="run-the-app"></a>アプリの実行

1. コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。


        npm start

1. ブラウザーで *http://localhost:3000* にナビゲートし、**[Office 365 に接続する]** ボタンを選びます。

1. サインインして要求されたアクセス許可を付与します。 

1. 必要に応じて、受信者のメール アドレスを編集してから、**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。 

## <a name="next-steps"></a>次の手順
- [Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。
- GitHub で他の [Node.js サンプル](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)を探します。


## <a name="see-also"></a>関連項目
- [Azure AD v2.0 のプロトコル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 のトークン](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
