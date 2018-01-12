# <a name="get-started-with-microsoft-graph-in-a-universal-windows-10-app"></a><span data-ttu-id="500b6-101">ユニバーサル Windows 10 アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="500b6-101">Get started with Microsoft Graph in a universal Windows 10 app</span></span>

> <span data-ttu-id="500b6-p101">**エンタープライズのお客様向けにアプリを作成していますか?**エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。</span><span class="sxs-lookup"><span data-stu-id="500b6-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="500b6-p102">**すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure 管理ポータル]((https://aka.ms/aadapplist))でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="500b6-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal]((https://aka.ms/aadapplist)). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="500b6-p103">この記事では、[Azure AD v2.0 エンドポイント]((https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth))からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[UWP 用 Microsoft Graph Connect サンプル (ライブラリ)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) のサンプル内のコードを説明し、Microsoft Graph を使用するアプリで実装する必要のある主要な概念について説明します。</span><span class="sxs-lookup"><span data-stu-id="500b6-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint]((https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth)) and call Microsoft Graph. It walks you through the code inside the [Microsoft Graph Connect Sample for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) samples to explain the main concepts that you have to implement in an app that uses Microsoft Graph.</span></span>

<span data-ttu-id="500b6-p104">**アプリを作成してみたいですか。**[Microsoft Graph クイック スタート]((https://developer.microsoft.com/graph/quick-start))を使用してすぐに使い始めるか、またはこの記事で取り扱っている [UWP 用 Microsoft Graph Connect サンプル (ライブラリ)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) をダウンロードしてください。[REST バージョンのサンプル]((https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample))も利用できます。</span><span class="sxs-lookup"><span data-stu-id="500b6-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start]((https://developer.microsoft.com/graph/quick-start)) to get up and running fast, or download the [Microsoft Graph Connect Sample for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) that this article is based on. Also note that we have a [REST version of this sample]((https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample)).</span></span>

## <a name="sample-user-interface"></a><span data-ttu-id="500b6-112">サンプル ユーザー インターフェイス</span><span class="sxs-lookup"><span data-stu-id="500b6-112">Sample user interface</span></span>

<span data-ttu-id="500b6-113">サンプルには、上部のコマンド バー、**[接続]** ボタン､**[メールの送信]** ボタン、およびサインイン ユーザーの電子メールアドレスが自動入力された編集可能なテキスト ボックスで構成される非常にシンプルなユーザー インターフェイスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="500b6-113">The sample contains a very simple user interface, consisting of a top command bar, a **connect button**, a **send mail** button, and a text box that is automatically populated with the signed-in user's e-mail address but that can be edited.</span></span>

<span data-ttu-id="500b6-114">**[メールの送信]** ボタンは、ユーザーが接続されていないときは無効になります。</span><span class="sxs-lookup"><span data-stu-id="500b6-114">The **send mail** button is disabled when the user has not connected:</span></span>

![[接続] ボタンが有効になっていて、[メールの送信] ボタンが無効になっていることを示す画面](images/SignedOut.png)

<span data-ttu-id="500b6-116">ユーザーが接続されている場合、上部のコマンド バーに [切断] ボタンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="500b6-116">The top command bar contains a disconnect button when the user has connected:</span></span>

![接続されたユーザーの電子メール アドレスと [メールの送信] ボタンが有効になっていることを示す画面](images/SignedIn.png)

<span data-ttu-id="500b6-118">すべてのサンプルの UI 文字列は、Assets フォルダー内の Resources.resw ファイルに格納されています。</span><span class="sxs-lookup"><span data-stu-id="500b6-118">All of the sample's UI strings are stored in the Resources.resw file inside the Assets folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="500b6-119">前提条件</span><span class="sxs-lookup"><span data-stu-id="500b6-119">Prerequisites</span></span>

<span data-ttu-id="500b6-120">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="500b6-120">To get started, you'll need:</span></span> 

- <span data-ttu-id="500b6-121">[Microsoft アカウント]((https://www.outlook.com/))か[職場または学校アカウント]((http://dev.office.com/devprogram))</span><span class="sxs-lookup"><span data-stu-id="500b6-121">A [Microsoft account]((https://www.outlook.com/)) or a [work or school account]((http://dev.office.com/devprogram))</span></span>
- <span data-ttu-id="500b6-122">Visual Studio 2017</span><span class="sxs-lookup"><span data-stu-id="500b6-122">Using Visual Studio 2017</span></span> 
- <span data-ttu-id="500b6-p105">[UWP 用 Microsoft Graph スターター プロジェクト (ライブラリ)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)/tree/master/starter)。両方のテンプレートには、コードを追加する空のクラスが含まれています。また、リソース文字列も含まれています。このプロジェクトを取得するには、[UWP 用 Microsoft Graph Connect のサンプル (ライブラリ)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) を複製またはダウンロードして、**starter** フォルダー内のソリューションを開きます。</span><span class="sxs-lookup"><span data-stu-id="500b6-p105">The [Microsoft Graph Starter Project for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)/tree/master/starter). Both templates contain empty classes that you'll add code to. They also contains resource strings. To get this project, clone or download the [Microsoft Graph Connect Sample for UWP (Library)]((https://github.com/microsoftgraph/uwp-csharp-connect-sample)) and then open the solution inside the **starter** folder.</span></span>


## <a name="register-the-app"></a><span data-ttu-id="500b6-127">アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="500b6-127">Register the app</span></span>
 
1. <span data-ttu-id="500b6-128">個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル]((https://apps.dev.microsoft.com/))にサインインします。</span><span class="sxs-lookup"><span data-stu-id="500b6-128">Sign into the [App Registration Portal]((https://apps.dev.microsoft.com/)) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="500b6-129">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="500b6-129">Select **Add an app**.</span></span>
3. <span data-ttu-id="500b6-130">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="500b6-130">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="500b6-131">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="500b6-131">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="500b6-132">**[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="500b6-132">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="500b6-133">**[ネイティブ アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="500b6-133">Select **Native Application**.</span></span>
6. <span data-ttu-id="500b6-p106">クライアント ID (アプリ ID) とリダイレクト URI の値の両方をクリップボードにコピーします。サンプル アプリにこれらの値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="500b6-p106">Copy both the Client Id (App Id) and Redirect URI values to the clipboard. You'll need to enter these values into the sample app.</span></span>

    <span data-ttu-id="500b6-p107">アプリ ID は、アプリの一意識別子です。リダイレクト URI は、各アプリケーションに対して Windows 10 で提供される一意の URI であり、その URI に送信されたメッセージだけがそのアプリケーションに送信されます。</span><span class="sxs-lookup"><span data-stu-id="500b6-p107">The app id is a unique identifier for your app. The redirect URI is a unique URI provided by Windows 10 for each application to ensure that messages sent to that URI are only sent to that application.</span></span> 

7. <span data-ttu-id="500b6-138">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="500b6-138">Select **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="500b6-139">プロジェクトを構成する</span><span class="sxs-lookup"><span data-stu-id="500b6-139">Configure the project</span></span>

1. <span data-ttu-id="500b6-140">Visual Studio でスターター プロジェクトのソリューション ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="500b6-140">Open the solution file for the starter project in Visual Studio.</span></span>
2. <span data-ttu-id="500b6-p108">プロジェクトの **App.xaml** ファイルを開き、`Application.Resources` ノードを見つけます。アプリケーション ID とリダイレクト URI のプレースホルダーを、登録したアプリの対応する値に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="500b6-p108">Open the project's **App.xaml** file and locate the `Application.Resources` node. Replace the application ID and redirect URI placeholders with the corresponding values of the app you registered.</span></span>


```xml
    <Application.Resources>
        <!-- Add your Client Id here. -->
        <x:String x:Key="ida:ClientID">ENTER_YOUR_CLIENT_ID</x:String>
        <!-- Add your Redirect URI here. -->
        <x:String x:Key="ida:ReturnUrl">ENTER_YOUR_REDIRECT_URI</x:String>
    </Application.Resources>
```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="500b6-143">Microsoft Graph を使用して電子メールを送信する</span><span class="sxs-lookup"><span data-stu-id="500b6-143">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="500b6-p109">スターター プロジェクトの MailHelper.cs ファイルを開きます。このファイルには、電子メールを作成して送信するコードが含まれています。それは、POST 要求を作成して **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** エンドポイントに送信する単一のメソッド (``ComposeAndSendMailAsync``) で構成されています。</span><span class="sxs-lookup"><span data-stu-id="500b6-p109">Open the MailHelper.cs file in your starter project. This file contains the code that constructs and sends an email. It consists of a single method -- ``ComposeAndSendMailAsync`` -- that constructs and sends a POST request to the **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** endpoint.</span></span> 

<span data-ttu-id="500b6-p110">``ComposeAndSendMailAsync`` メソッドは、MainPage.xaml.cs ファイルによって渡される 3 つの文字列値 (``subject``、``bodyContent``、``recipients``) を取得します。``subject`` および ``bodyContent`` の文字列は、その他のすべての UI 文字列とともに Resources.resw ファイルに格納されます。``recipients`` の文字列はアプリのインターフェイスにあるアドレス ボックスのものです。</span><span class="sxs-lookup"><span data-stu-id="500b6-p110">The ``ComposeAndSendMailAsync`` method takes three string values -- ``subject``, ``bodyContent``, and ``recipients`` -- that are passed to it by the MainPage.xaml.cs file. The ``subject`` and ``bodyContent`` strings are stored, along with all other UI strings, in the Resources.resw file. The ``recipients`` string comes from the address box in the app's interface.</span></span> 

<span data-ttu-id="500b6-p111">``ComposeAndSendMailAsync`` メソッド内の最初のタスクでは、Microsoft Graph から現在のユーザーの写真を取得します。この行は、`GetCurrentUserPhotoStreamAsync` メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="500b6-p111">The first task inside the ``ComposeAndSendMailAsync`` method is to get the current user's photo from Microsoft Graph. This line calls the `GetCurrentUserPhotoStreamAsync` method:</span></span>

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

<span data-ttu-id="500b6-152">完全な `GetCurrentUserPhotoStreamAsync` メソッドは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="500b6-152">This is what the complete `GetCurrentUserPhotoStreamAsync` method looks like:</span></span>

```
        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }
```

<span data-ttu-id="500b6-153">ユーザーが写真を持っていない場合、このロジックでは、プロジェクトに含まれている別のイメージ ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="500b6-153">If the user doesn't have a photo, this logic gets another image file that has been included with the project:</span></span>

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                StorageFile file = await Windows.ApplicationModel.Package.Current.InstalledLocation.GetFileAsync("test.jpg");
                photoStream = (await file.OpenReadAsync()).AsStreamForRead();
            }
```

<span data-ttu-id="500b6-154">イメージ ストリームができたため、`UploadFileToOneDriveAsync` メソッドを呼び出してファイルを OneDrive にアップロードできます。</span><span class="sxs-lookup"><span data-stu-id="500b6-154">Now that we have an image stream, we can upload the file to OneDrive by calling the `UploadFileToOneDriveAsync` method:</span></span>

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

<span data-ttu-id="500b6-155">完全な `UploadFileToOneDriveAsync` メソッドは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="500b6-155">This is what the complete `UploadFileToOneDriveAsync` method looks like:</span></span>

```
        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }
```

<span data-ttu-id="500b6-156">このストリームは、次のメッセージとともに渡すことができる `MessageAttachmentsCollectionPage` オブジェクトの作成にも使用できます。</span><span class="sxs-lookup"><span data-stu-id="500b6-156">We can also use this stream to create a `MessageAttachmentsCollectionPage` object that we can pass along with the message:</span></span>

```
            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });
```

<span data-ttu-id="500b6-p112">`GetSharingLinkAsync` メソッドを呼び出して、新しくアップロードした OneDrive ファイルの共有リンクを取得できます。`bodyContent` 文字列には、共有リンクのプレースホルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="500b6-p112">We can get a sharing link for the newly uploaded OneDrive file by calling the `GetSharingLinkAsync` method. The `bodyContent` string contains a placeholder for the sharing link:</span></span>

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

<span data-ttu-id="500b6-159">完全な `GetSharingLinkAsync` メソッドは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="500b6-159">This is what the complete `GetSharingLinkAsync` method looks like:</span></span>

```
        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }
```

<span data-ttu-id="500b6-160">複数のアドレスを渡すことができるため、次は、``recipients`` 文字列を一連の `EmailAddress` オブジェクトに分割します。それは、`Recipients` オブジェクトの一覧を作成するために使用され、そのオブジェクトは要求の POST 本文に入れて渡されます。</span><span class="sxs-lookup"><span data-stu-id="500b6-160">Since the user can potentially pass more than one address, the next task is to split the ``recipients`` string into a set of `EmailAddress` objects that can then be used to construct the list of `Recipients` objects that will be passed in the POST body of the request:</span></span>

```
            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }
```

<span data-ttu-id="500b6-p113">最後に、`Message` オブジェクトを作成し、`GraphServiceClient` を使用して **me/microsoft.graph.SendMail** エンドポイントに送信します。``bodyContent`` の文字列は HTML 文書であるため、要求によって HTML に **ContentType** 値が設定されます。</span><span class="sxs-lookup"><span data-stu-id="500b6-p113">The last task is to construct a `Message` object and send it to the **me/microsoft.graph.SendMail** endpoint through the `GraphServiceClient`. Since the ``bodyContent`` string is an HTML document, the request sets the **ContentType** value to HTML.</span></span>

```
            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
```

<span data-ttu-id="500b6-163">完全なクラスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="500b6-163">The complete class will look like this:</span></span>

```
    public class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        public async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                StorageFile file = await Windows.ApplicationModel.Package.Current.InstalledLocation.GetFileAsync("test.jpg");
                photoStream = (await file.OpenReadAsync()).AsStreamForRead();
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);

            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }


        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
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
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

    }
``` 

 
<span data-ttu-id="500b6-164">これで、Microsoft Graph と対話するために必要な、アプリの登録、ユーザーの認証、および要求の作成の手順が完了しました。</span><span class="sxs-lookup"><span data-stu-id="500b6-164">You've now performed the steps required for interacting with Microsoft Graph: app registration, user authentication, and making the requests.</span></span> 

## <a name="run-the-app"></a><span data-ttu-id="500b6-165">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="500b6-165">Run the app</span></span>
1. <span data-ttu-id="500b6-166">F5 キーを押して、アプリを構築して実行します。</span><span class="sxs-lookup"><span data-stu-id="500b6-166">Press F5 to build and run the app.</span></span> 

2. <span data-ttu-id="500b6-167">個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="500b6-167">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

3. <span data-ttu-id="500b6-p114">**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。このメール メッセージには添付ファイルとして写真が含まれており、OneDrive にアップロードされたファイルへの共有リンクも提示されます。</span><span class="sxs-lookup"><span data-stu-id="500b6-p114">Choose the **Send email** button. When the mail is sent, a Success message is displayed below the button. the mail message includes the photo as an attachment and also provides a sharing link to the uploaded file in OneDrive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="500b6-171">次の手順</span><span class="sxs-lookup"><span data-stu-id="500b6-171">Next steps</span></span>
- <span data-ttu-id="500b6-172">[Graph エクスプローラー]((https://developer.microsoft.com/ja-JP/graph/graph-explorer))を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="500b6-172">Try out the REST API using the [Graph explorer]((https://developer.microsoft.com/ja-JP/graph/graph-explorer)).</span></span>
- <span data-ttu-id="500b6-173">[Microsoft Graph UWP スニペット サンプル (SDK)]((https://github.com/microsoftgraph/uwp-csharp-snippets-sample)) と [Microsoft Graph UWP スニペット サンプル (REST)]((https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample)) での REST と SDK の両方の操作に共通する操作の例を検索するか、GitHub で他の [UWP サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp)を探索します。</span><span class="sxs-lookup"><span data-stu-id="500b6-173">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph UWP Snippets Sample (SDK)]((https://github.com/microsoftgraph/uwp-csharp-snippets-sample)) and the [Microsoft Graph UWP Snippets Sample (REST)]((https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample)), or explore our other [UWP samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="500b6-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="500b6-174">See also</span></span>
- <span data-ttu-id="500b6-175">[Microsoft Graph .NET クライアント ライブラリ]((https://github.com/microsoftgraph/msgraph-sdk-dotnet))</span><span class="sxs-lookup"><span data-stu-id="500b6-175">[Microsoft Graph .NET Client Library]((https://github.com/microsoftgraph/msgraph-sdk-dotnet))</span></span>
- <span data-ttu-id="500b6-176">[Azure AD v2.0 のプロトコル]((https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/))</span><span class="sxs-lookup"><span data-stu-id="500b6-176">[Azure AD v2.0 protocols]((https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/))</span></span>
- <span data-ttu-id="500b6-177">[Azure AD v2.0 のトークン]((https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/))</span><span class="sxs-lookup"><span data-stu-id="500b6-177">[Azure AD v2.0 tokens]((https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/))</span></span>

