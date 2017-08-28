# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a>AngularJS アプリで Microsoft Graph を使ってみる

この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[AngularJS 用の Microsoft Connect サンプル](https://github.com/microsoftgraph/angular-connect-rest-sample)の構築手順と、Microsoft Graph を使用するために実装する主要な概念について説明します。またこの記事では、[Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) または未加工の REST 呼び出しを使用して Microsoft Graph にアクセスする方法についても説明します。

次の画像は、作成するアプリを示しています。 

![ログイン後に [メールの送信] ボタンを表示する Web アプリ](./images/angular-connect-sample.png)


**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/en-us/getting-started)」を使用すれば、すばやく稼働させることができます。

Azure AD エンドポイントを使用するバージョンの Connect サンプルをダウンロードするには、「[AngularJS 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth)」をご覧ください。


## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

- [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)
- [npm 付きの Node.js](https://nodejs.org/en/download/)
- [Bower](https://bower.io)
- [AngularJS 用 Microsoft Connect のサンプル](https://github.com/microsoftgraph/angular-connect-sample)このチュートリアルには、サンプル ファイル内の **starter-project** フォルダーを使用します。

## <a name="register-the-application"></a>アプリケーションの登録
Microsoft アプリケーション登録ポータルでアプリケーションを登録します。これにより、アプリを Visual Studio で構成する際に使用するアプリ ID とパスワードが生成されます。

1. 個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。

2. **[アプリの追加]** を選択します。

3. アプリの名前を入力して、**[アプリケーションの作成]** を選択します。 
    
    登録ページが表示され、アプリのプロパティが一覧表示されます。

4. アプリケーション ID をコピーします。これは、アプリの構成に使用するアプリの一意識別子です。

5. **[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選びます。

6. **[暗黙的フローを許可する]** のチェック ボックスが選択されていることを確認して、リダイレクト URI として *http://localhost:8080* を入力します。 

7. **[保存]** を選択します。


## <a name="configure-the-project"></a>プロジェクトを構成する
1. サンプル ファイル内の **starter-project** フォルダーを開きます。
2. コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。これにより、プロジェクトの依存関係がインストールされます。

        npm install  
        bower install
    
3. スターター プロジェクトのファイル内の **public/scripts** フォルダーにある、config.js を開きます。
4. **clientID** フィールド内の **ENTER_YOUR_CLIENT_ID** プレースホルダーの値を、前の手順でコピーしたアプリケーション ID に置き換えます。

## <a name="call-microsoft-graph-with-the-sdk"></a>SDK を使用して Microsoft Graph を呼び出す
アプリは Microsoft Graph を呼び出してユーザー情報を取得し、ユーザーの代わりにメールを送信します。これらの呼び出しは UI イベントに応答して MainController から始まります。

app.js を開いて、ファイルの末尾に次に示すコードを追加します。これにより、SDK が初期化されます。

    var authToken;
    var graphClient = MicrosoftGraph.Client.init({
        authProvider: function(done) {
        if (typeof authToken === "undefined") {
          done({err: "No auth token"})
        } else {
          done(null, authToken); //first parameter takes an error if you can't get an access token
        }
        }
    });

### <a name="using-the-sdk"></a>SDK を使用する
1. graphHelper.js で、*// Get the profile of the current user* を次のコードに置き換えます。これにより GET 要求を構成して */me* エンドポイントに送信し、応答を処理します。

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. *// Send an email on behalf of the current user* を次のコードに置き換えます。これにより POST 要求を構成して */me/sendMail* エンドポイントに送信し、応答を処理します。

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. **public/controllers** フォルダーで、mainController.js を開きます。

4. *// Set the default headers and user properties* を次のコードに置き換えます。これにより HTTP 要求にアクセス トークンを追加し、**GraphHelper.me** を呼び出して現在のユーザーのプロファイルを取得し、応答を処理します。

        // Set the default headers and user properties.
        function processAuth() {

        // let the authProvider access the access token
        authToken = localStorage.token;

        if (localStorage.getItem('user') === null) {

          // Get the profile of the current user.
          GraphHelper.me().then(function(user) {

            // Save the user to localStorage.
            localStorage.setItem('user', angular.toJson(user));

            vm.displayName = user.displayName;
            vm.emailAddress = user.mail || user.userPrincipalName;
          });
        } else {
          let user = angular.fromJson(localStorage.user);

          vm.displayName = user.displayName;
          vm.emailAddress = user.mail || user.userPrincipalName;
        }

        }

5. *// Send an email on behalf of the current user* を次のコードに置き換えます。これにより、メール メッセージを作成し、**GraphHelper.sendMail** を呼び出して、応答を処理します。

        // Send an email on behalf of the current user.
        function sendMail() {

          authToken = localStorage.token;       

          // Build the HTTP request payload (the Message object).
          var email = {
          Subject: 'Welcome to Microsoft Graph development with Angular and the Microsoft Graph Connect sample',
          Body: {
            ContentType: 'HTML',
            Content: getEmailContent()
          },
          ToRecipients: [
            {
              EmailAddress: {
            Address: vm.emailAddress
              }
            }
          ]
          };

          // Save email address so it doesn't get lost with two way data binding.
          vm.emailAddressSent = vm.emailAddress;
          GraphHelper.sendMail(email)
        .then(function (response) {
          $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
          vm.requestSuccess = true;
          vm.requestFinished = true;
          $scope.$apply();
        }, function (error) {
          $log.error('HTTP request to the Microsoft Graph API failed.');
          vm.requestSuccess = false;
          vm.requestFinished = true;
          $scope.$apply();
        });

        };

6. 変更をすべて保存します。

## <a name="run-the-app"></a>アプリの実行

1. コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。

        npm start

2. ブラウザーで *http://localhost:8080* にナビゲートし **[Connect]** ボタンを選びます。

3. サインインして要求されたアクセス許可を付与します。 

4. 必要に応じて、受信者のメール アドレスを編集してから、**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。 

## <a name="next-steps"></a>次の手順
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用して REST API を試してみます。
- GitHub で他の [AngularJS サンプル](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)を探します。


## <a name="see-also"></a>関連項目
- [Azure AD v2.0 のプロトコル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 のトークン](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
