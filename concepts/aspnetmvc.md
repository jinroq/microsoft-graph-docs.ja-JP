# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a><span data-ttu-id="ac085-101">ASP.NET 4.6 MVC アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="ac085-101">Get started with Microsoft Graph in an ASP.NET 4.6 MVC app</span></span>

<span data-ttu-id="ac085-p101">この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[ASP.NET 4.6 用の Microsoft Graph 接続サンプル](https://github.com/microsoftgraph/aspnet-connect-sample)の構築手順と、Microsoft Graph を使用するために実装する主要な概念について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac085-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span>

<span data-ttu-id="ac085-104">次の画像は、作成するアプリを示しています。</span><span class="sxs-lookup"><span data-stu-id="ac085-104">The following image shows the app you'll create.</span></span> 

<span data-ttu-id="ac085-105">![[メール アドレスの取得] および [メールの送信] ボタンを持つ Web アプリケーション](images/aspnet-connect-sample.png "[メール アドレスの取得] と [メールの送信] ボタンを持つ Web アプリケーション")</span><span class="sxs-lookup"><span data-stu-id="ac085-105">![The web app with "Get email address" and "Send email" buttons](images/aspnet-connect-sample.png "The web app with 'Get email address' and 'Send email' buttons")</span></span>

<span data-ttu-id="ac085-p102">[Azure AD v2.0 エンドポイント](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview) では、ユーザーは Microsoft アカウント (MSA) や、職場または学校のアカウントを使用してサインインします。アプリでは、[ASP.Net OpenID Connect OWIN ミドルウェア](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) および [.NET 用 Microsoft 認証ライブラリ (MSAL) ](https://www.nuget.org/packages/Microsoft.Identity.Client) を使用して、サインインとトークンの管理を行います。</span><span class="sxs-lookup"><span data-stu-id="ac085-p102">The [Azure AD v2.0 endpoint](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview) lets users sign in with a Microsoft account (MSA) or a work or school account. The app uses the [ASP.Net OpenID Connect OWIN middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) and the [Microsoft Authentication Library (MSAL) for .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) for sign in and token management.</span></span>

<span data-ttu-id="ac085-p103">**アプリを作成してみたいですか。**「[Microsoft Graph クイック スタート](https://developer.microsoft.com/ja-JP/graph/quick-start)」を使用すれば、すぐに始めることができます。[REST バージョンのサンプル](https://github.com/microsoftgraph/aspnet-connect-rest-sample)も利用できます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/ja-JP/graph/quick-start) to get up and running fast. Also note that we have a [REST version of this sample](https://github.com/microsoftgraph/aspnet-connect-rest-sample).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac085-111">前提条件</span><span class="sxs-lookup"><span data-stu-id="ac085-111">Prerequisites</span></span>

<span data-ttu-id="ac085-112">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="ac085-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="ac085-113">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="ac085-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="ac085-114">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="ac085-114">Visual Studio 2015</span></span> 
- <span data-ttu-id="ac085-p104">[ASP.NET 4.6 用 Microsoft Graph 接続サンプル](https://github.com/microsoftgraph/aspnet-connect-sample)。サンプル ファイルの **starter-project** フォルダーを開きます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p104">The [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). You'll use the **starter-project** folder in the sample files.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="ac085-117">アプリケーションの登録</span><span class="sxs-lookup"><span data-stu-id="ac085-117">Register the application</span></span>

<span data-ttu-id="ac085-p105">この手順では、Microsoft アプリ登録ポータルでアプリを登録します。これにより、アプリを Visual Studio で構成する際に使用するアプリ ID とパスワードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p105">In this step, you'll register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="ac085-120">個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ac085-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="ac085-121">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ac085-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="ac085-122">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ac085-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="ac085-123">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="ac085-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="ac085-p106">アプリケーション ID をコピーします。これは、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="ac085-p106">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="ac085-p107">**[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選びます。**[新しいパスワードが生成されました]** ダイアログからパスワードをコピーします。</span><span class="sxs-lookup"><span data-stu-id="ac085-p107">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="ac085-128">アプリを構成するために、アプリケーション ID とパスワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="ac085-128">You'll use the application ID and password to configure the app.</span></span> 

6. <span data-ttu-id="ac085-129">**[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="ac085-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="ac085-130">**[暗黙的フローを許可する]** のチェック ボックスが選択されていることを確認して、リダイレクト URI として *http://localhost:55065/* を入力します。</span><span class="sxs-lookup"><span data-stu-id="ac085-130">Make sure the Allow Implicit Flow check box is selected, and enter http://localhost:55065/ as the Redirect URI.</span></span> 

    <span data-ttu-id="ac085-p108">**[暗黙的フローを許可する]** オプションにより、OpenID Connect ハイブリッド フローが有効になります。これにより、認証時にアプリはサインイン情報 (**id_token**) と成果物 (この場合は認証コード) の両方を受け取れるようになり、アプリはアクセス トークンを取得するときにこれらを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the **id_token**) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

8. <span data-ttu-id="ac085-133">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ac085-133">Choose **Save**.</span></span>

### <a name="configure-the-project"></a><span data-ttu-id="ac085-134">プロジェクトを構成する</span><span class="sxs-lookup"><span data-stu-id="ac085-134">Configure the project</span></span>

1. <span data-ttu-id="ac085-135">Visual Studio でスターター プロジェクトのソリューション ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ac085-135">Open the solution file for the starter project in Visual Studio.</span></span>

2. <span data-ttu-id="ac085-136">プロジェクトの Web.config ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ac085-136">Open the project's Web.config file.</span></span>

3. <span data-ttu-id="ac085-p109">**appSettings** 要素内のアプリの構成キーの位置を確認します。ENTER_YOUR_CLIENT_ID と ENTER_YOUR_SECRET のプレース ホルダー値をコピーした値に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p109">Locate the app configuration keys in the **appSettings** element. Replace the ENTER_YOUR_CLIENT_ID and ENTER_YOUR_SECRET placeholder values with the values you just copied.</span></span>

<span data-ttu-id="ac085-p110">リダイレクト URI は、登録したプロジェクトの URL です。要求される[アクセス許可のスコープ](https://developer.microsoft.com/ja-JP/graph/docs/concepts/permission_scopes)によって、アプリはユーザー プロファイル情報を取得したり、電子メールを送信したりできます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p110">The redirect URI is the URL of the project that you registered. The requested [permission scopes](https://developer.microsoft.com/ja-JP/graph/docs/concepts/permission_scopes) allow the app to get user profile information and send an email.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="ac085-141">Microsoft Graph を呼び出す</span><span class="sxs-lookup"><span data-stu-id="ac085-141">Call Microsoft Graph</span></span>

<span data-ttu-id="ac085-142">この手順では、**SDKHelper**、**GraphService**、**HomeController** クラスにフォーカスします。</span><span class="sxs-lookup"><span data-stu-id="ac085-142">In this step, you'll focus on the **SDKHelper**, **GraphService**, and **HomeController** classes.</span></span> 

 - <span data-ttu-id="ac085-p111">**SDKHelper** は、Microsoft Graph を呼び出す前に毎回、ライブラリから **GraphServiceClient** のインスタンスを初期化します。このときに、アクセス トークンが要求に追加されます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p111">**SDKHelper** intializes an instance of the **GraphServiceClient** from the library before each call to the Microsoft Graph. This is when the access token is added to the request.</span></span> 
 - <span data-ttu-id="ac085-145">**GraphService** は、ライブラリを使用して Microsoft Graph への要求をビルドして送信し、応答を処理します。</span><span class="sxs-lookup"><span data-stu-id="ac085-145">**GraphService** builds and sends requests to the Microsoft Graph using the library, and processes the responses.</span></span>
 - <span data-ttu-id="ac085-146">**HomeController** には、UI イベントへの応答としてライブラリへの呼び出しを開始するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ac085-146">**HomeController** contains actions that initiate the calls to the library in response to UI events.</span></span>

<span data-ttu-id="ac085-147">スターター プロジェクトでは、既に Microsoft Graph .NET Client Library NuGet パッケージの依存関係を宣言しています: *Microsoft.Graph*。</span><span class="sxs-lookup"><span data-stu-id="ac085-147">The starter project already declares a dependency for the Microsoft Graph .NET Client Library NuGet package:  *Microsoft.Graph*.</span></span>

1. <span data-ttu-id="ac085-148">**[ヘルパー]** フォルダーを右クリックし、**[追加]** > **[クラス]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="ac085-148">Right-click the **Helpers** folder and choose **Add** > **Class**.</span></span> 

1. <span data-ttu-id="ac085-149">新しいクラスの名前を *SDKHelper* にして、**[追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ac085-149">Name the new class *SDKHelper* and choose **Add**.</span></span>

1. <span data-ttu-id="ac085-150">コンテンツを次のコードで置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ac085-150">Replace the contents with the following code.</span></span>

        using System.Net.Http.Headers;
        using Microsoft.Graph;

        namespace Microsoft_Graph_SDK_ASPNET_Connect.Helpers
        {
            public class SDKHelper
            {   
                private static GraphServiceClient graphClient = null;

                // Get an authenticated Microsoft Graph Service client.
                public static GraphServiceClient GetAuthenticatedClient()
                {
                    GraphServiceClient graphClient = new GraphServiceClient(
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                                // Append the access token to the request.
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);
                            }));
                    return graphClient;
                }

                public static void SignOutClient()
                {
                    graphClient = null;
                }
            }
        }

  <span data-ttu-id="ac085-151">**SampleAuthProvider** を呼び出して、クライアントが初期化されたときにトークンを取得するようにします。</span><span class="sxs-lookup"><span data-stu-id="ac085-151">Note the call to **SampleAuthProvider** to get the token when the client is initialized.</span></span>

1. <span data-ttu-id="ac085-p112">**[モデル]** フォルダーで、GraphService.cs を開きます。サービスでは、ライブラリを使用して、Microsoft Graph を操作します。</span><span class="sxs-lookup"><span data-stu-id="ac085-p112">In the **Models** folder, open GraphService.cs. The service uses the library to interact with the Microsoft Graph.</span></span>

1. <span data-ttu-id="ac085-154">次の **using** ステートメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="ac085-154">Add the following **using** statement.</span></span>

        using Microsoft.Graph;

1. <span data-ttu-id="ac085-p113">*//GetMyEmailAddress* を次のメソッドに置き換えます。これにより、現在のユーザーの電子メール アドレスを取得します。</span><span class="sxs-lookup"><span data-stu-id="ac085-p113">Replace *// GetMyEmailAddress* with the following method. This gets the current user's email address.</span></span> 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  <span data-ttu-id="ac085-p114">**[選択]** セグメントは、**メール** と **userPrinicipalName** が返されるように要求することにご注意ください。**[選択]** と **[フィルター]** を使って、応答データのペイロードのサイズを小さくできます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p114">Note the **Select** segment, which requests only the **mail** and **userPrinicipalName** to be returned. You can use **Select** and **Filter** to reduce the size of the response data payload.</span></span>

1. <span data-ttu-id="ac085-159">電子メールをビルドし、送信するために、*//SendEmail* を以下のメソッドに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ac085-159">Replace *// SendEmail* with the following methods to build and send the email.</span></span>

        // Send an email message from the current user.
        public async Task SendEmail(GraphServiceClient graphClient, Message message)
        {
            await graphClient.Me.SendMail(message, true).Request().PostAsync();
        }

        public async Task<Message> BuildEmailMessage(GraphServiceClient graphClient, string recipients, string subject)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync(graphClient);


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if ( photoStream == null)
            {
                photoStream = System.IO.File.OpenRead(System.Web.Hosting.HostingEnvironment.MapPath("/Content/test.jpg"));
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDrive(graphClient, photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            Permission sharingLink = await GetSharingLinkAsync(graphClient, photoFile.Id);

            // Add the sharing link to the email body.
            string bodyContent = string.Format(Resource.Graph_SendMail_Body_Content, sharingLink.Link.WebUrl);

            // Prepare the recipient list.
            string[] splitter = { ";" };
            string[] splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();
            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Address = recipient.Trim()
                    }
                });
            }

            // Build the email message.
            Message email = new Message
            {
                Body = new ItemBody
                {
                    Content = bodyContent,
                    ContentType = BodyType.Html,
                },
                Subject = subject,
                ToRecipients = recipientList,
                Attachments = attachments
            };
            return email;
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync(GraphServiceClient graphClient)
        {
            Stream currentUserPhotoStream = null;

            try
            {
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }

        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(GraphServiceClient graphClient, string Id)
        {
            Permission permission = null;

            try
            {
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

1. <span data-ttu-id="ac085-160">**[コントローラー]** フォルダーで、HomeController.cs を開きます。</span><span class="sxs-lookup"><span data-stu-id="ac085-160">In the **Controllers** folder, open HomeController.cs.</span></span>

1. <span data-ttu-id="ac085-161">次の **using** ステートメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="ac085-161">Add the following **using** statement.</span></span>

        using Microsoft.Graph;
  
1. <span data-ttu-id="ac085-162">*// Controller actions* を、次のアクションに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ac085-162">Replace *// Controller actions* with the following actions.</span></span>

        [Authorize]
        // Get the current user's email address from their profile.
        public async Task<ActionResult> GetMyEmailAddress()
        {
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Get the current user's email address. 
                ViewBag.Email = await graphService.GetMyEmailAddress(graphClient);
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

        [Authorize]
        // Send mail on behalf of the current user.
        public async Task<ActionResult> SendEmail()
        {
            if (string.IsNullOrEmpty(Request.Form["email-address"]))
            {
                ViewBag.Message = Resource.Graph_SendMail_Message_GetEmailFirst;
                return View("Graph");
            }

            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Build the email message.
                Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Code == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

<span data-ttu-id="ac085-163">これで、[アプリを実行する](#run-the-app)準備ができました。</span><span class="sxs-lookup"><span data-stu-id="ac085-163">Now you're ready to [run the app](#run-the-app).</span></span>

## <a name="run-the-app"></a><span data-ttu-id="ac085-164">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="ac085-164">Run the app</span></span>
1. <span data-ttu-id="ac085-165">F5 キーを押して、アプリを構築して実行します。</span><span class="sxs-lookup"><span data-stu-id="ac085-165">Press F5 to build and run the app.</span></span> 

2. <span data-ttu-id="ac085-166">個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="ac085-166">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

3. <span data-ttu-id="ac085-p115">**[メール アドレスの取得]** ボタンを選択します。操作が完了すると、サインインしているユーザーのメール アドレスがページに表示されます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p115">Choose the **Get email address** button. When the operation completes, the email address of the signed-in user is displayed on the page.</span></span>

4. <span data-ttu-id="ac085-p116">必要に応じて、受信者一覧とメールの件名を編集し、**[メールの送信]** ボタンを選択します。メールが送信されると、ボタンの下に成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ac085-p116">Optionally edit the recipient list and email subject, and then choose the **Send email** button. When the mail is sent, a Success message is displayed below the button.</span></span>


## <a name="next-steps"></a><span data-ttu-id="ac085-171">次の手順</span><span class="sxs-lookup"><span data-stu-id="ac085-171">Next steps</span></span>
- <span data-ttu-id="ac085-172">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="ac085-172">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="ac085-173">[ASP.NET 4.6 用の Microsoft Graph スニペットのサンプル](https://github.com/microsoftgraph/aspnet-snippets-sample)で一般的な操作の例を見つけるか、GitHub で別の [ASP.NET サンプル](http://aka.ms/aspnetgraphsamples)を探します。</span><span class="sxs-lookup"><span data-stu-id="ac085-173">Find examples of common operations in the [Microsoft Graph Snippets Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample), or explore our other [ASP.NET samples](http://aka.ms/aspnetgraphsamples) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="ac085-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac085-174">See also</span></span>
- [<span data-ttu-id="ac085-175">Microsoft Graph .NET クライアント ライブラリ</span><span class="sxs-lookup"><span data-stu-id="ac085-175">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="ac085-176">Web アプリケーションから Web への API 認証シナリオ</span><span class="sxs-lookup"><span data-stu-id="ac085-176">Web application to web API authentication scenario</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [<span data-ttu-id="ac085-177">OpenID Connect を使用して、Microsoft Identity と Microsoft Graph を Web アプリケーションに統合する</span><span class="sxs-lookup"><span data-stu-id="ac085-177">Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect</span></span>](https://azure.microsoft.com/ja-JP/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [<span data-ttu-id="ac085-178">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="ac085-178">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="ac085-179">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="ac085-179">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/)
