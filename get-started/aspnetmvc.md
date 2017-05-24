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


## <a name="authenticate-the-user-and-get-an-access-token"></a>ユーザーの認証とアクセス トークンの取得

この手順では、サインインとトークンの管理コードを追加します。しかし、まず認証フローをさらに詳しく見てみましょう。

このアプリは、委任されたユーザー ID で認証コードの付与フローを使用します。Web アプリケーションのフローでは、登録したアプリのアプリケーション ID、パスワード、およびリダイレクト URI が必要です。 

認証フローは、以下の基本的な手順に分けることができます。

1. 認証と同意のためにユーザーをリダイレクトする
2. 認証コードを取得する
3. 認証コードをアクセス トークンに交換する
4. アクセス トークンの有効期限が切れたら、更新トークンを使用して新しいアクセス トークンを取得する

アプリでは、[ASP.Net OpenID Connect OWIN ミドルウェア](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) と [.NET 用 Microsoft 認証ライブラリ (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client) を使用して、サインインとトークンの管理を行います。これにより、ほとんどの認証タスクを処理します。
    
スターター プロジェクトでは、既に次のミドルウェアと MSAL NuGet の依存関係を宣言しています:

  - Microsoft.Owin.Security.OpenIdConnect
  - Microsoft.Owin.Security.Cookies
  - Microsoft.Owin.Host.SystemWeb
  - Microsoft.Identity.Client

ここでアプリの作成に戻ります。

1. **App_Start** フォルダーで、Startup.Auth.cs を開きます。 

1. **ConfigureAuth** メソッドを次のコードに置き換えます。これにより、Azure AD と通信するための座標を設定し、OpenID Connect ミドルウェアによって使用される Cookie 認証を設定します。

        public void ConfigureAuth(IAppBuilder app)
        {
            app.SetDefaultSignInAsAuthenticationType(CookieAuthenticationDefaults.AuthenticationType);

            app.UseCookieAuthentication(new CookieAuthenticationOptions());

            app.UseOpenIdConnectAuthentication(
                new OpenIdConnectAuthenticationOptions
                {

                    // The `Authority` represents the Microsoft v2.0 authentication and authorization service.
                    // The `Scope` describes the permissions that your app will need. See https://azure.microsoft.com/documentation/articles/active-directory-v2-scopes/                    
                    ClientId = appId,
                    Authority = "https://login.microsoftonline.com/common/v2.0",
                    PostLogoutRedirectUri = redirectUri,
                    RedirectUri = redirectUri,
                    Scope = "openid email profile offline_access " + graphScopes,
                    TokenValidationParameters = new TokenValidationParameters
                    {
                        ValidateIssuer = false,
                        // In a real application you would use IssuerValidator for additional checks, 
                        // like making sure the user's organization has signed up for your app.
                        //     IssuerValidator = (issuer, token, tvp) =>
                        //     {
                        //         if (MyCustomTenantValidation(issuer)) 
                        //             return issuer;
                        //         else
                        //             throw new SecurityTokenInvalidIssuerException("Invalid issuer");
                        //     },
                    },
                    Notifications = new OpenIdConnectAuthenticationNotifications
                    {
                        AuthorizationCodeReceived = async (context) =>
                        {
                            var code = context.Code;
                            string signedInUserID = context.AuthenticationTicket.Identity.FindFirst(ClaimTypes.NameIdentifier).Value;
                            ConfidentialClientApplication cca = new ConfidentialClientApplication(
                                appId, 
                                redirectUri,
                                new ClientCredential(appSecret),
                                new SessionTokenCache(signedInUserID, context.OwinContext.Environment["System.Web.HttpContextBase"] as HttpContextBase));
                                string[] scopes = graphScopes.Split(new char[] { ' ' });

                            AuthenticationResult result = await cca.AcquireTokenByAuthorizationCodeAsync(scopes, code);
                        },
                        AuthenticationFailed = (context) =>
                        {
                            context.HandleResponse();
                            context.Response.Redirect("/Error?message=" + context.Exception.Message);
                            return Task.FromResult(0);
                        }
                    }
                });
        }
  
  OWIN Startup クラス (Startup.cs で定義済み) はアプリの起動時に **ConfigureAuth** メソッドを呼び出し、そのメソッドは **app.UseOpenIdConnectAuthentication** を呼び出して、サインインのためのミドルウェアと最初のトークン要求を初期化します。アプリでは、次のアクセス許可スコープを要求します:

  - サインインのための **openid**、**email**、**profile**
  - トークン取得のための **offline\_access** (更新トークンを取得するために必要)、**User.Read**、**Mail.Send**
  
  MSAL **ConfidentialClientApplication** オブジェクトは、アプリを表し、トークンの管理タスクを処理します。それは、**SessionTokenCache** (TokenStorage/SessionTokenCache.cs で定義されるサンプル トークン キャッシュの実装) とともに、トークン情報が保存される場所で、初期化されます。キャッシュは、ユーザー ID に基づいて、現在の HTTP セッションにトークンを保存しますが、運用アプリケーションには、より持続性の高いストレージの使用が適しています。

次に、コードをサンプル認証プロバイダーに追加します。これは独自のカスタム認証プロバイダーと簡単に置き換えられるようにデザインされています。プロジェクトに、インターフェイスおよびプロバイダー クラスが既に追加されているはずです。

1. **[ヘルパー]** フォルダーで、SampleAuthProvider.cs を開きます。

1. **GetUserAccessTokenAsync** メソッドを、MSAL を使用してアクセス トークンを取得する次の実装と置き換えます。

        // Get an access token. First tries to get the token from the token cache.
        public async Task<string> GetUserAccessTokenAsync()
        {
            string signedInUserID = ClaimsPrincipal.Current.FindFirst(ClaimTypes.NameIdentifier).Value;
            tokenCache = new SessionTokenCache(
                signedInUserID, 
                HttpContext.Current.GetOwinContext().Environment["System.Web.HttpContextBase"] as HttpContextBase);
            //var cachedItems = tokenCache.ReadItems(appId); // see what's in the cache

            ConfidentialClientApplication cca = new ConfidentialClientApplication(
                appId, 
                redirectUri,
                new ClientCredential(appSecret), 
                tokenCache);

            try
            {
                AuthenticationResult result = await cca.AcquireTokenSilentAsync(scopes.Split(new char[] { ' ' }));
                return result.Token;
            }

            // Unable to retrieve the access token silently.
            catch (MsalSilentTokenAcquisitionException)
            {
                HttpContext.Current.Request.GetOwinContext().Authentication.Challenge(
                    new AuthenticationProperties() { RedirectUri = "/" },
                    OpenIdConnectAuthenticationDefaults.AuthenticationType);

                throw new Exception(Resource.Error_AuthChallengeNeeded);
            }
        }

  MSAL は、一致するアクセス トークンの、期限切れや期限切れ間近でないものをキャッシュで確認します。有効なものが見つからない場合は、更新トークンを使って (もし有効なものが存在すれば) 新しいアクセス トークンを取得します。サイレント モードで、新しいアクセス トークンを取得できない場合には、MSAL は **MsalSilentTokenAcquisitionException** をスローして、ユーザー プロンプトの表示が必要であることを示します。 

次に、署名と UI からのサインアウトを処理するコードを追加します。

1. **[コントローラー]** フォルダーで、AccountController.cs を開きます。  

1. 次のメソッドを **AccountController** クラスに追加します。**SignIn** メソッドは、ミドルウェアにシグナルを送って、Azure AD への認証要求を送信させます。

        public void SignIn()
        {
            if (!Request.IsAuthenticated)
            {
                // Signal OWIN to send an authorization request to Azure.
                HttpContext.GetOwinContext().Authentication.Challenge(
                    new AuthenticationProperties { RedirectUri = "/" },
                    OpenIdConnectAuthenticationDefaults.AuthenticationType);
            }
        }

        // Here we just clear the token cache, sign out the GraphServiceClient, and end the session with the web app.  
        public void SignOut()
        {
            if (Request.IsAuthenticated)
            {
                // Get the user's token cache and clear it.
                string userObjectId = ClaimsPrincipal.Current.FindFirst(ClaimTypes.NameIdentifier).Value;

                SessionTokenCache tokenCache = new SessionTokenCache(userObjectId, HttpContext);
                tokenCache.Clear(userObjectId);
            }

            //SDKHelper.SignOutClient();

            // Send an OpenID Connect sign-out request. 
            HttpContext.GetOwinContext().Authentication.SignOut(
            CookieAuthenticationDefaults.AuthenticationType);
            Response.Redirect("/");
        }

これで、Microsoft Graph を呼び出すためのコードを追加する準備が整いました。 

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

            // Build the email message.
            Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
           }
        }

次に、ユーザー プロンプトが必要な場合に認証プロバイダーによりスローされる例外を変更します。

1. **[ヘルパー]** フォルダーで、SampleAuthProvider.cs を開きます。

1. 次の **using** ステートメントを追加します。

        using Microsoft.Graph;
  
1. **GetUserAccessTokenAsync** メソッドの **catch** ブロックで、スローされる例外を次のように変更します:

        throw new ServiceException(
            new Error
            {
                Code = GraphErrorCode.AuthenticationFailure.ToString(),
                Message = Resource.Error_AuthChallengeNeeded,
            });

最後に、呼び出しを追加して、クライアントをサインアウトさせます。 

1. **[コントローラー]** フォルダーで、AccountController.cs を開きます。 

1. 次の行のコメントを解除します:

        SDKHelper.SignOutClient();

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
