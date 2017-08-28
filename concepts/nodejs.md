# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a><span data-ttu-id="31e20-101">Node.js アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="31e20-101">Get started with Microsoft Graph in a Node.js app</span></span>

<span data-ttu-id="31e20-p101">この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[Node.js 用の Microsoft Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)の構築手順と、Microsoft Graph を使用するために実装する主要な概念について説明します。この記事では、生の REST 呼び出しを使用して Microsoft Graph API にアクセスする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="31e20-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article describes how to access the Microsoft Graph API by using raw REST calls.</span></span>

<span data-ttu-id="31e20-105">次の画像は、作成するアプリを示しています。</span><span class="sxs-lookup"><span data-stu-id="31e20-105">The following image shows is the app you'll create.</span></span> 

![ログイン後に [メールの送信] ボタンを表示する Web アプリ](./images/web-screenshot.png)


<span data-ttu-id="31e20-p102">**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/en-us/getting-started)」を使用すれば、すばやく稼働させることができます。</span><span class="sxs-lookup"><span data-stu-id="31e20-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="31e20-109">Azure AD エンドポイントを使用するバージョンの Connect サンプルをダウンロードするには、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="31e20-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="31e20-110">前提条件</span><span class="sxs-lookup"><span data-stu-id="31e20-110">Prerequisites</span></span>

<span data-ttu-id="31e20-111">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="31e20-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="31e20-112">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="31e20-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- [<span data-ttu-id="31e20-113">npm 付きの Node.js</span><span class="sxs-lookup"><span data-stu-id="31e20-113">Node.js with npm</span></span>](https://nodejs.org/en/download/) 
- <span data-ttu-id="31e20-p103">[Node.js 用 Microsoft Connect のサンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)このチュートリアルには、サンプル ファイル内の **starter-project** フォルダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="31e20-p103">The [Microsoft Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="31e20-116">アプリケーションの登録</span><span class="sxs-lookup"><span data-stu-id="31e20-116">Register the application</span></span>
<span data-ttu-id="31e20-p104">Microsoft アプリケーション登録ポータルでアプリケーションを登録します。これにより、アプリを Visual Studio で構成する際に使用するアプリ ID とパスワードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="31e20-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="31e20-119">個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="31e20-119">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="31e20-120">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="31e20-120">Choose **Add an app**.</span></span>

3. <span data-ttu-id="31e20-121">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="31e20-121">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="31e20-122">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="31e20-122">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="31e20-p105">アプリケーション ID をコピーします。これは、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="31e20-p105">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="31e20-p106">**[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選びます。**[新しいパスワードが生成されました]** ダイアログからパスワードをコピーします。</span><span class="sxs-lookup"><span data-stu-id="31e20-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="31e20-127">アプリを構成するには、アプリケーション ID とアプリケーション パスワード (シークレット) を使用します。</span><span class="sxs-lookup"><span data-stu-id="31e20-127">You'll use the application ID and application password (secret) to configure the app.</span></span> 

6. <span data-ttu-id="31e20-128">**[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="31e20-128">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="31e20-129">リダイレクト URI には、*http://localhost:3000/token* と入力します。</span><span class="sxs-lookup"><span data-stu-id="31e20-129">Enter *http://localhost:3000/token* as the Redirect URI.</span></span> 

8. <span data-ttu-id="31e20-130">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="31e20-130">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="31e20-131">プロジェクトを構成する</span><span class="sxs-lookup"><span data-stu-id="31e20-131">Configure the project</span></span>
1. <span data-ttu-id="31e20-132">サンプル ファイル内の **starter-project** フォルダーを開きます。</span><span class="sxs-lookup"><span data-stu-id="31e20-132">Open the **starter-project** folder in the sample files.</span></span>

1. <span data-ttu-id="31e20-p107">コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。これにより、プロジェクトの依存関係がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="31e20-p107">In a command prompt, run the following command in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install

1. <span data-ttu-id="31e20-135">スターター プロジェクト ファイル内の utils\config.js を開きます。</span><span class="sxs-lookup"><span data-stu-id="31e20-135">In the starter project files, open utils\config.js.</span></span>


1. <span data-ttu-id="31e20-136">**credentials** フィールド内の **ENTER\_YOUR\_CLIENT\_ID** プレースホルダーと **ENTER\_YOUR\_SECRET** プレースホルダーの値を、直前にコピーした値に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="31e20-136">In the **credentials** field, replace the **ENTER\_YOUR\_CLIENT\_ID** and **ENTER\_YOUR\_SECRET** placeholder values with the values you just copied.</span></span>

  
## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="31e20-137">ユーザーの認証とアクセス トークンの取得</span><span class="sxs-lookup"><span data-stu-id="31e20-137">Authenticate the user and get an access token</span></span>
<span data-ttu-id="31e20-p108">この手順では、サインインとトークンの管理コードを追加します。しかし、まず認証フローをさらに詳しく見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="31e20-p108">In this step, you'll add sign-in and token management code. But first, let's take a closer look at the auth flow.</span></span>

<span data-ttu-id="31e20-p109">このアプリは、委任されたユーザー ID で認証コードの付与フローを使用します。Web アプリケーションのフローでは、登録したアプリのアプリケーション ID、シークレット、およびリダイレクト URI が必要です。</span><span class="sxs-lookup"><span data-stu-id="31e20-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="31e20-142">認証フローは、以下の基本的な手順に分けることができます。</span><span class="sxs-lookup"><span data-stu-id="31e20-142">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="31e20-143">認証と同意のためにユーザーをリダイレクトする</span><span class="sxs-lookup"><span data-stu-id="31e20-143">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="31e20-144">認証コードを取得する</span><span class="sxs-lookup"><span data-stu-id="31e20-144">Get an authorization code</span></span>
3. <span data-ttu-id="31e20-145">認証コードをアクセス トークンに交換する</span><span class="sxs-lookup"><span data-stu-id="31e20-145">Redeem the authorization code for an access token</span></span>
4. <span data-ttu-id="31e20-146">アクセス トークンの有効期限が切れたら、更新トークンを使用して新しいアクセス トークンを取得する</span><span class="sxs-lookup"><span data-stu-id="31e20-146">Use the refresh token to get a new access token when the access token expires</span></span>

<span data-ttu-id="31e20-p110">アプリは [oauth](https://www.npmjs.com/package/oauth) ミドルウェアを使用して認証し、トークンを取得します。アプリは [cookie-parser](https://www.npmjs.com/package/cookie-parser) ミドルウェアを使用して、トークン情報をクッキーにキャッシュします。トークン情報の格納とアクセスに使用されるコードは、index.js コントローラーにあります。</span><span class="sxs-lookup"><span data-stu-id="31e20-p110">The app uses the [oauth](https://www.npmjs.com/package/oauth) middleware to authenticate and obtain tokens. It uses the [cookie-parser](https://www.npmjs.com/package/cookie-parser) middleware to cache token information in cookies. The code used to store and access token information is found in the index.js controller.</span></span>
    
   ><span data-ttu-id="31e20-p111">**重要** このプロジェクトでは、サンプルの目的で単純な認証とトークンの処理を使用しているに過ぎません。運用アプリでは、検証やセキュリティで保護されたトークンの処理など、認証を処理するためのより信頼性の高い方法を構築する必要があります。</span><span class="sxs-lookup"><span data-stu-id="31e20-p111">**Important** The simple authentication and token handling in this project is for sample purposes only. In a production app, you should construct a more robust way of handling authentication, including validation and secure token handling.</span></span>

<span data-ttu-id="31e20-152">これで、Microsoft Graph を呼び出すためのコードを追加する準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="31e20-152">Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph"></a><span data-ttu-id="31e20-153">Microsoft Graph を呼び出す</span><span class="sxs-lookup"><span data-stu-id="31e20-153">Call Microsoft Graph</span></span>
<span data-ttu-id="31e20-p112">アプリは Microsoft Graph を呼び出してユーザー情報を取得し、ユーザーの代わりにメールを送信します。これらの呼び出しは UI イベントに応答して index.js コントローラーから始まります。</span><span class="sxs-lookup"><span data-stu-id="31e20-p112">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the index.js controller in response to UI events.</span></span>

1. <span data-ttu-id="31e20-156">utils\graphHelper.js を開きます。</span><span class="sxs-lookup"><span data-stu-id="31e20-156">Open utils\graphHelper.js.</span></span>

1. <span data-ttu-id="31e20-p113">**getUserData** 関数を、以下のコードに置き換えます。これにより GET 要求を構成して */me* エンドポイントに送信し、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="31e20-p113">Replace the **getUserData** function with the following code. This configures and sends the GET request to the */me* endpoint and processes the response.</span></span>

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. <span data-ttu-id="31e20-p114">**getProfilePhoto** 関数を次のコードに置き換えます。これにより、GET 要求を構成して */me/photo/$value* エンドポイントに送信し、応答を処理します。現在、プロフィール写真は MSA アカウントで使用できないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="31e20-p114">Replace the **getProfilePhoto** function with the following code. This configures and sends the GET request to the */me/photo/$value* endpoint and processes the response. Note that profile photos aren't currently available for MSA accounts.</span></span>
    
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

1. <span data-ttu-id="31e20-p115">**uploadFile** 関数を次のコードに置き換えます。これにより、PUT 要求を構成して */me/drive/root/children/mypic.jpg/content* エンドポイントに送信します。ファイルが存在する場合、この要求によってコンテンツが更新されます。存在しない場合、ファイルが作成され、プロフィール写真のコンテンツがアップロードされます。</span><span class="sxs-lookup"><span data-stu-id="31e20-p115">Replace the **uploadFile** function with the following code. This configures and sends the PUT request to the */me/drive/root/children/mypic.jpg/content* endpoint. If the file exists, this requests updates the content. If it doesn't exist, it creates the file and uploads the contents of the profile photo.</span></span> 

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

1. <span data-ttu-id="31e20-p116">**getSharingLink** 関数を次のコードに置き換えます。これにより、GET 要求を構成して */me/drive/items/{file id}/createLink* エンドポイントに送信し、結果を処理します。結果はメッセージに含まれるファイルへの共有リンクになります。</span><span class="sxs-lookup"><span data-stu-id="31e20-p116">Replace the **getSharingLink** function with the following code. This configures and sends the GET request to the */me/drive/items/{file id}/createLink* endpoint and processes the result. The result is a sharing link to the file that will be included in the message.</span></span>

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

1. <span data-ttu-id="31e20-p117">**postSendMail** 関数を次のコードに置き換えます。これにより POST 要求を構成して */me/sendMail* エンドポイントに送信し、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="31e20-p117">Replace the **postSendMail** function with the following code. This configures and sends the POST request to the */me/sendMail* endpoint and processes the response.</span></span>

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

1. <span data-ttu-id="31e20-171">utils\emailer.js を開きます。</span><span class="sxs-lookup"><span data-stu-id="31e20-171">Open utils\emailer.js.</span></span>

1. <span data-ttu-id="31e20-p118">**wrapEmail** 関数を次のコードに置き換えます。これにより、送信するメール メッセージを表すペイロードを構築します。</span><span class="sxs-lookup"><span data-stu-id="31e20-p118">Replace the **wrapEmail** function with the following code. This builds the payload that represents the email message to send.</span></span>

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

## <a name="run-the-app"></a><span data-ttu-id="31e20-174">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="31e20-174">Run the app</span></span>

1. <span data-ttu-id="31e20-175">コマンド プロンプトで、スターター プロジェクトのルート ディレクトリから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="31e20-175">In a command prompt, run the following command in the root directory of the starter project.</span></span>


        npm start

1. <span data-ttu-id="31e20-176">ブラウザーで *http://localhost:3000* にナビゲートし、**[Office 365 に接続する]** ボタンを選びます。</span><span class="sxs-lookup"><span data-stu-id="31e20-176">In a browser, navigate to *http://localhost:3000* and choose the **Connect to Office 365** button.</span></span>

1. <span data-ttu-id="31e20-177">サインインして要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="31e20-177">Sign in and grant the requested permissions.</span></span> 

1. <span data-ttu-id="31e20-p119">必要に応じて、受信者のメール アドレスを編集してから、**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="31e20-p119">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="31e20-180">次の手順</span><span class="sxs-lookup"><span data-stu-id="31e20-180">Next steps</span></span>
- <span data-ttu-id="31e20-181">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="31e20-181">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="31e20-182">GitHub で他の [Node.js サンプル](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)を探します。</span><span class="sxs-lookup"><span data-stu-id="31e20-182">Explore our other [Node.js samples](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="31e20-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="31e20-183">See also</span></span>
- [<span data-ttu-id="31e20-184">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="31e20-184">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="31e20-185">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="31e20-185">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
