# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a><span data-ttu-id="fa297-101">AngularJS アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="fa297-101">Get started with Microsoft Graph in an AngularJS app</span></span>

<span data-ttu-id="fa297-p101">この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[AngularJS 用の Microsoft Connect サンプル](https://github.com/microsoftgraph/angular-connect-rest-sample)の構築手順と、Microsoft Graph を使用するために実装する主要な概念について説明します。またこの記事では、[Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) または未加工の REST 呼び出しを使用して Microsoft Graph にアクセスする方法についても説明します。</span><span class="sxs-lookup"><span data-stu-id="fa297-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) or raw REST calls.</span></span>

<span data-ttu-id="fa297-105">次の画像は、作成するアプリを示しています。</span><span class="sxs-lookup"><span data-stu-id="fa297-105">The following image shows the app you'll create.</span></span> 

![ログイン後に [メールの送信] ボタンを表示する Web アプリ](./images/angular-connect-sample.png)


<span data-ttu-id="fa297-p102">**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/ja-JP/getting-started)」を使用すれば、すばやく稼働させることができます。</span><span class="sxs-lookup"><span data-stu-id="fa297-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/ja-JP/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="fa297-109">Azure AD エンドポイントを使用するバージョンの Connect サンプルをダウンロードするには、「[AngularJS 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fa297-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="fa297-110">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa297-110">Prerequisites</span></span>

<span data-ttu-id="fa297-111">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="fa297-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="fa297-112">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="fa297-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- [<span data-ttu-id="fa297-113">npm 付きの Node.js</span><span class="sxs-lookup"><span data-stu-id="fa297-113">Node.js with npm</span></span>](https://nodejs.org/en/download/)
- [<span data-ttu-id="fa297-114">Bower</span><span class="sxs-lookup"><span data-stu-id="fa297-114">Bower</span></span>](https://bower.io)
- <span data-ttu-id="fa297-p103">[AngularJS 用 Microsoft Connect のサンプル](https://github.com/microsoftgraph/angular-connect-sample)このチュートリアルには、サンプル ファイル内の **starter-project** フォルダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="fa297-p103">The [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="fa297-117">アプリケーションの登録</span><span class="sxs-lookup"><span data-stu-id="fa297-117">Register the application</span></span>
<span data-ttu-id="fa297-p104">Microsoft アプリケーション登録ポータルでアプリケーションを登録します。これにより、アプリを Visual Studio で構成する際に使用するアプリ ID とパスワードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="fa297-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="fa297-120">個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="fa297-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="fa297-121">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fa297-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="fa297-122">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fa297-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="fa297-123">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="fa297-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="fa297-p105">アプリケーション ID をコピーします。これは、アプリの構成に使用するアプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="fa297-p105">Copy the application ID. This is the unique identifier for your app that you'll use to configure the app.</span></span>

5. <span data-ttu-id="fa297-126">**[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="fa297-126">Under **Platforms**, choose **Add Platform** > **Web**.</span></span>

6. <span data-ttu-id="fa297-127">**[暗黙的フローを許可する]** のチェック ボックスが選択されていることを確認して、リダイレクト URI として *http://localhost:8080* を入力します。</span><span class="sxs-lookup"><span data-stu-id="fa297-127">Make sure the Allow Implicit Flow check box is selected, and enter http://localhost:8080 as the Redirect URI.</span></span> 

7. <span data-ttu-id="fa297-128">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fa297-128">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="fa297-129">プロジェクトを構成する</span><span class="sxs-lookup"><span data-stu-id="fa297-129">Configure the project</span></span>
1. <span data-ttu-id="fa297-130">サンプル ファイル内の **starter-project** フォルダーを開きます。</span><span class="sxs-lookup"><span data-stu-id="fa297-130">Open the **starter-project** folder in the sample files.</span></span>
2. <span data-ttu-id="fa297-p106">コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。これにより、プロジェクトの依存関係がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="fa297-p106">In a command prompt, run the following commands in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install  
        bower install
    
3. <span data-ttu-id="fa297-133">スターター プロジェクトのファイル内の **public/scripts** フォルダーにある、config.js を開きます。</span><span class="sxs-lookup"><span data-stu-id="fa297-133">In the starter project files, in the **public/scripts** folder, open config.js.</span></span>
4. <span data-ttu-id="fa297-134">**clientID** フィールド内の **ENTER_YOUR_CLIENT_ID** プレースホルダーの値を、前の手順でコピーしたアプリケーション ID に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="fa297-134">In the **clientID** field, replace the **ENTER_YOUR_CLIENT_ID** placeholder value with the application ID you just copied.</span></span>

## <a name="call-microsoft-graph-with-the-sdk"></a><span data-ttu-id="fa297-135">SDK を使用して Microsoft Graph を呼び出す</span><span class="sxs-lookup"><span data-stu-id="fa297-135">Call Microsoft Graph with the SDK</span></span>
<span data-ttu-id="fa297-p107">アプリは Microsoft Graph を呼び出してユーザー情報を取得し、ユーザーの代わりにメールを送信します。これらの呼び出しは UI イベントに応答して MainController から始まります。</span><span class="sxs-lookup"><span data-stu-id="fa297-p107">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the MainController in response to UI events.</span></span>

<span data-ttu-id="fa297-p108">app.js を開いて、ファイルの末尾に次に示すコードを追加します。これにより、SDK が初期化されます。</span><span class="sxs-lookup"><span data-stu-id="fa297-p108">Open app.js and add the following code to the bottom of the file. This initializes the SDK.</span></span>

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

### <a name="using-the-sdk"></a><span data-ttu-id="fa297-140">SDK を使用する</span><span class="sxs-lookup"><span data-stu-id="fa297-140">Using the SDK</span></span>
1. <span data-ttu-id="fa297-p109">graphHelper.js で、*// Get the profile of the current user* を次のコードに置き換えます。これにより GET 要求を構成して */me* エンドポイントに送信し、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="fa297-p109">In graphHelper.js, replace *// Get the profile of the current user* with the following code. This configures and sends the GET request to the */me* endpoint, and processes the response.</span></span>

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. <span data-ttu-id="fa297-p110">*// Send an email on behalf of the current user* を次のコードに置き換えます。これにより POST 要求を構成して */me/sendMail* エンドポイントに送信し、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="fa297-p110">Replace *// Send an email on behalf of the current user* with the following code. This configures and sends the POST request to the */me/sendMail* endpoint, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. <span data-ttu-id="fa297-145">**public/controllers** フォルダーで、mainController.js を開きます。</span><span class="sxs-lookup"><span data-stu-id="fa297-145">In the **public/controllers** folder, open mainController.js.</span></span>

4. <span data-ttu-id="fa297-p111">*// Set the default headers and user properties* を次のコードに置き換えます。これにより HTTP 要求にアクセス トークンを追加し、**GraphHelper.me** を呼び出して現在のユーザーのプロファイルを取得し、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="fa297-p111">Replace *// Set the default headers and user properties* with the following code. This adds the access token to the HTTP request, calls **GraphHelper.me** to get the current user's profile, and processes the response.</span></span>

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

5. <span data-ttu-id="fa297-p112">*// Send an email on behalf of the current user* を次のコードに置き換えます。これにより、メール メッセージを作成し、**GraphHelper.sendMail** を呼び出して、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="fa297-p112">Replace *// Send an email on behalf of the current user* with the following code. This builds the email message, calls **GraphHelper.sendMail**, and processes the response.</span></span>

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

6. <span data-ttu-id="fa297-150">変更をすべて保存します。</span><span class="sxs-lookup"><span data-stu-id="fa297-150">Save all your changes.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="fa297-151">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="fa297-151">Run the app</span></span>

1. <span data-ttu-id="fa297-152">コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="fa297-152">In a command prompt, run the following command in the root directory of the starter project.</span></span>

        npm start

2. <span data-ttu-id="fa297-153">ブラウザーで *http://localhost:8080* にナビゲートし **[Connect]** ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="fa297-153">In a browser, navigate to http://localhost:8080 and choose the Connect button.</span></span>

3. <span data-ttu-id="fa297-154">サインインして要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="fa297-154">Sign in and grant the requested permissions.</span></span> 

4. <span data-ttu-id="fa297-p113">必要に応じて、受信者のメール アドレスを編集してから、**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fa297-p113">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="fa297-157">次の手順</span><span class="sxs-lookup"><span data-stu-id="fa297-157">Next steps</span></span>
- <span data-ttu-id="fa297-158">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="fa297-158">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="fa297-159">GitHub で他の [AngularJS サンプル](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)を探します。</span><span class="sxs-lookup"><span data-stu-id="fa297-159">Explore our other [AngularJS samples](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="fa297-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa297-160">See also</span></span>
- [<span data-ttu-id="fa297-161">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="fa297-161">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="fa297-162">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="fa297-162">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/)
