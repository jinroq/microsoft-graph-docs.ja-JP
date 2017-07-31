# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a>ASP.NET 4.6 MVC アプリで Microsoft Graph を使ってみる

この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[ASP.NET 4.6 用の Microsoft Graph 接続サンプル](https://github.com/microsoftgraph/aspnet-connect-sample)の構築手順と、Microsoft Graph を使用するために実装する主要な概念について説明します。

次の画像は、作成するアプリを示しています。 

![[メール アドレスの取得] および [メールの送信] ボタンを持つ Web アプリケーション](images/aspnet-connect-sample.png "[メール アドレスの取得] と [メールの送信] ボタンを持つ Web アプリケーション")

[Azure AD v2.0 エンドポイント](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview) では、ユーザーは Microsoft アカウント (MSA) や、職場または学校のアカウントを使用してサインインします。アプリでは、[ASP.Net OpenID Connect OWIN ミドルウェア](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) および [.NET 用 Microsoft 認証ライブラリ (MSAL) ](https://www.nuget.org/packages/Microsoft.Identity.Client) を使用して、サインインとトークンの管理を行います。

**アプリを作成してみたいですか。**「[Microsoft Graph クイック スタート](https://developer.microsoft.com/en-us/graph/quick-start)」を使用すれば、すぐに始めることができます。[REST バージョンのサンプル](https://github.com/microsoftgraph/aspnet-connect-rest-sample)も利用できます。

## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

- [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)
- Visual Studio 2015 
- [ASP.NET 4.6 用 Microsoft Graph 接続サンプル](https://github.com/microsoftgraph/aspnet-connect-sample)。サンプル ファイルの **starter-project** フォルダーを開きます。


## <a name="register-the-application"></a>アプリケーションの登録

この手順では、Microsoft アプリ登録ポータルでアプリを登録します。これにより、アプリを Visual Studio で構成する際に使用するアプリ ID とパスワードが生成されます。

1. 個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。

2. **[アプリの追加]** を選択します。

3. アプリの名前を入力して、**[アプリケーションの作成]** を選択します。 
    
    登録ページが表示され、アプリのプロパティが一覧表示されます。

4. アプリケーション ID をコピーします。これは、アプリの一意識別子です。 

5. **[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選びます。**[新しいパスワードが生成されました]** ダイアログからパスワードをコピーします。

    アプリを構成するために、アプリケーション ID とパスワードを使用します。 

6. **[プラットフォーム]** で、**[プラットフォームの追加]** > **[Web]** の順に選択します。

7. **[暗黙的フローを許可する]** のチェック ボックスが選択されていることを確認して、リダイレクト URI として *http://localhost:55065/* を入力します。 

    **[暗黙的フローを許可する]** オプションにより、OpenID Connect ハイブリッド フローが有効になります。これにより、認証時にアプリはサインイン情報 (**id_token**) と成果物 (この場合は認証コード) の両方を受け取れるようになり、アプリはアクセス トークンを取得するときにこれらを使用できます。

8. **[保存]** を選択します。

### <a name="configure-the-project"></a>プロジェクトを構成する

1. Visual Studio でスターター プロジェクトのソリューション ファイルを開きます。

2. プロジェクトの Web.config ファイルを開きます。

3. **appSettings** 要素内のアプリの構成キーの位置を確認します。ENTER_YOUR_CLIENT_ID と ENTER_YOUR_SECRET のプレース ホルダー値をコピーした値に置き換えます。

リダイレクト URI は、登録したプロジェクトの URL です。要求される[アクセス許可のスコープ](https://developer.microsoft.com/en-us/graph/docs/concepts/permission_scopes)によって、アプリはユーザー プロファイル情報を取得したり、電子メールを送信したりできます。

## <a name="call-microsoft-graph"></a>Microsoft Graph を呼び出す

この手順では、**SDKHelper**、**GraphService**、**HomeController** クラスにフォーカスします。 

 - **SDKHelper** は、Microsoft Graph を呼び出す前に毎回、ライブラリから **GraphServiceClient** のインスタンスを初期化します。このときに、アクセス トークンが要求に追加されます。 
 - **GraphService** は、ライブラリを使用して Microsoft Graph への要求をビルドして送信し、応答を処理します。
 - **HomeController** には、UI イベントへの応答としてライブラリへの呼び出しを開始するアクションが含まれています。

スターター プロジェクトでは、既に Microsoft Graph .NET Client Library NuGet パッケージの依存関係を宣言しています: *Microsoft.Graph*。

1. **[ヘルパー]** フォルダーを右クリックし、**[追加]** > **[クラス]** の順に選択します。 

1. 新しいクラスの名前を *SDKHelper* にして、**[追加]** を選択します。

1. コンテンツを次のコードで置き換えます。

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

  **SampleAuthProvider** を呼び出して、クライアントが初期化されたときにトークンを取得するようにします。

1. **[モデル]** フォルダーで、GraphService.cs を開きます。サービスでは、ライブラリを使用して、Microsoft Graph を操作します。

1. 次の **using** ステートメントを追加します。

        using Microsoft.Graph;

1. *//GetMyEmailAddress* を次のメソッドに置き換えます。これにより、現在のユーザーの電子メール アドレスを取得します。 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  **[選択]** セグメントは、**メール** と **userPrinicipalName** が返されるように要求することにご注意ください。**[選択]** と **[フィルター]** を使って、応答データのペイロードのサイズを小さくできます。

1. 電子メールをビルドし、送信するために、*//SendEmail* を以下のメソッドに置き換えます。

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

1. **[コントローラー]** フォルダーで、HomeController.cs を開きます。

1. 次の **using** ステートメントを追加します。

        using Microsoft.Graph;
  
1. *// Controller actions* を、次のアクションに置き換えます。

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

これで、[アプリを実行する](#run-the-app)準備ができました。

## <a name="run-the-app"></a>アプリの実行
1. F5 キーを押して、アプリを構築して実行します。 

2. 個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。

3. **[メール アドレスの取得]** ボタンを選択します。操作が完了すると、サインインしているユーザーのメール アドレスがページに表示されます。

4. 必要に応じて、受信者一覧とメールの件名を編集し、**[メールの送信]** ボタンを選択します。メールが送信されると、ボタンの下に成功メッセージが表示されます。


## <a name="next-steps"></a>次の手順
- [Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみましょう。
- [ASP.NET 4.6 用の Microsoft Graph スニペットのサンプル](https://github.com/microsoftgraph/aspnet-snippets-sample)で一般的な操作の例を見つけるか、GitHub で別の [ASP.NET サンプル](http://aka.ms/aspnetgraphsamples)を探します。

## <a name="see-also"></a>関連項目
- [Microsoft Graph .NET クライアント ライブラリ](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Web アプリケーションから Web への API 認証シナリオ](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [OpenID Connect を使用して、Microsoft Identity と Microsoft Graph を Web アプリケーションに統合する](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [Azure AD v2.0 のプロトコル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 のトークン](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
