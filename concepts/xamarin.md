# <a name="get-started-with-microsoft-graph-in-a-xamarin-forms-app"></a><span data-ttu-id="52f5e-101">Xamarin Forms アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="52f5e-101">Get started with Microsoft Graph in a Xamarin Forms app</span></span>

> <span data-ttu-id="52f5e-p101">**エンタープライズのお客様向けにアプリを作成していますか?** エンタープライズのお客様が、<a href="https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

<span data-ttu-id="52f5e-p102">この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[Xamarin Forms 用 Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) のサンプル内のコードを説明し、Microsoft Graph を使用するアプリで実装する必要のある主要な概念について説明します。また、この記事では、[Microsoft Graph クライアント ライブラリ](http://www.nuget.org/packages/Microsoft.Graph/)を使用して Microsoft Graph にアクセスする方法についても説明します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p102">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) sample to explain the main concepts that you have to implement in an app that uses Microsoft Graph. The article also describes how to access Microsoft Graph by using the [Microsoft Graph Client Library](http://www.nuget.org/packages/Microsoft.Graph/).</span></span>

<span data-ttu-id="52f5e-108">次のアプリを作成します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-108">This is the app you'll create.</span></span>

| <span data-ttu-id="52f5e-109">UWP</span><span class="sxs-lookup"><span data-stu-id="52f5e-109">UWP</span></span> | <span data-ttu-id="52f5e-110">Android</span><span class="sxs-lookup"><span data-stu-id="52f5e-110">Android</span></span> | <span data-ttu-id="52f5e-111">iOS</span><span class="sxs-lookup"><span data-stu-id="52f5e-111">iOS</span></span> |
| --- | ------- | ----|
| <img src="images/UWP.png" alt="Connect sample on UWP" width="100%" /> | <img src="images/Droid.png" alt="Connect sample on Android" width="100%" /> | <img src="images/iOS.png" alt="Connect sample on iOS" width="100%" /> |

<span data-ttu-id="52f5e-p103">**アプリを作成してみたくありませんか。**[Microsoft Graph クイック スタート](https://developer.microsoft.com/graph/quick-start)を使用してすぐに使い始めるか、またはこの記事で取り扱っている [Xamarin Forms 用 Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/xamarin-csharp-connect-sample)をダウンロードしてください。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/graph/quick-start) to get up and running fast, or download the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) that this article is based on.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52f5e-114">前提条件</span><span class="sxs-lookup"><span data-stu-id="52f5e-114">Prerequisites</span></span>

<span data-ttu-id="52f5e-115">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="52f5e-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="52f5e-116">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="52f5e-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="52f5e-117">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="52f5e-117">Visual Studio 2015</span></span> 
- [<span data-ttu-id="52f5e-118">Xamarin for Visual Studio</span><span class="sxs-lookup"><span data-stu-id="52f5e-118">Xamarin for Visual Studio</span></span>](https://www.xamarin.com/visual-studio)
- <span data-ttu-id="52f5e-119">Windows 10 ([開発モードが有効](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx))</span><span class="sxs-lookup"><span data-stu-id="52f5e-119">Windows 10 ([development mode enabled](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx))</span></span>
- <span data-ttu-id="52f5e-p104">[Xamarin Forms 用の Microsoft Graph Connect スターター プロジェクト](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter)。このテンプレートには、コード追加先のいくつかのクラスが含まれています。完全なビューおよびリソース文字列も含まれています。このプロジェクトを取得するには、[Xamarin Forms 用 Microsoft Graph Connect のサンプル](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) を複製またはダウンロードして、**スターター** フォルダー内の **XamarinConnect** ソリューションを開きます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p104">The [Microsoft Graph Connect Starter Project for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter). This template contains several classes that you'll add code to. It also contains complete views and resource strings. To get this project, clone or download the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) and open the **XamarinConnect** solution inside the **starter** folder.</span></span> 

<span data-ttu-id="52f5e-124">このサンプルで iOS プロジェクトを実行する場合は、以下のものが必要です:</span><span class="sxs-lookup"><span data-stu-id="52f5e-124">If you want to run the iOS project in this sample, you'll need the following:</span></span>

- <span data-ttu-id="52f5e-125">最新の iOS SDK</span><span class="sxs-lookup"><span data-stu-id="52f5e-125">The latest iOS SDK</span></span>
- <span data-ttu-id="52f5e-126">最新バージョンの Xcode</span><span class="sxs-lookup"><span data-stu-id="52f5e-126">The latest version of Xcode</span></span>
- <span data-ttu-id="52f5e-127">Mac OS X Sierra(10.12) 以上</span><span class="sxs-lookup"><span data-stu-id="52f5e-127">Mac OS X Sierra(10.12) & above</span></span> 
- [<span data-ttu-id="52f5e-128">Xamarin.iOS</span><span class="sxs-lookup"><span data-stu-id="52f5e-128">Xamarin.iOS</span></span>](https://docs.microsoft.com/visualstudio/mac/installation)
- <span data-ttu-id="52f5e-129">[Visual Studio に接続されている Xamarin Mac エージェント](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)</span><span class="sxs-lookup"><span data-stu-id="52f5e-129">A [Xamarin Mac agent connected to Visual Studio](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)</span></span>


## <a name="register-the-app"></a><span data-ttu-id="52f5e-130">アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="52f5e-130">Register the app</span></span>
 
1. <span data-ttu-id="52f5e-131">個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="52f5e-131">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="52f5e-132">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-132">Select **Add an app**.</span></span>
3. <span data-ttu-id="52f5e-133">アプリの名前を入力して、**[作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-133">Enter a name for the app, and select **Create**.</span></span>
    
    <span data-ttu-id="52f5e-134">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-134">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="52f5e-135">**[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-135">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="52f5e-136">**[ネイティブ アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-136">Select **Native Application**.</span></span>
6. <span data-ttu-id="52f5e-p105">**[ネイティブ アプリケーション]** プラットフォームを追加したときに作成されたアプリケーション ID の値とカスタム リダイレクト URI の値 (**[ネイティブ アプリケーション]** ヘッダーの下) をコピーします。この URI は、お客様のアプリケーション ID の値が含まれており、次の形式である必要があります。`msal[Application Id]://auth` サンプル アプリにこれらの値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p105">Copy the Application Id value and the Custom Redirect URI value (under the **Native Application** header) that was created for you when you added the **Native Application** platform. This URI should contain your Application Id value and be in this form: `msal[Application Id]://auth` You'll need to enter these values into the sample app.</span></span>

    <span data-ttu-id="52f5e-139">アプリ ID は、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="52f5e-139">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="52f5e-140">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-140">Select **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="52f5e-141">プロジェクトを構成する</span><span class="sxs-lookup"><span data-stu-id="52f5e-141">Configure the project</span></span>

1. <span data-ttu-id="52f5e-142">Visual Studio でスターター プロジェクトのソリューション ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-142">Open the solution file for the starter project in Visual Studio.</span></span>
2. <span data-ttu-id="52f5e-p106">**XamarinConnect (ポータブル)** プロジェクト内にある **App.cs** ファイルを開き、`ClientId` フィールドを検索します。アプリケーション ID のプレースホルダーを、登録したアプリのアプリケーション ID と置き換えます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p106">Open the **App.cs** file inside the **XamarinConnect (Portable)** project and locate the `ClientId` field. Replace the application ID placeholder with the application id of the app you registered.</span></span>

    ```
    public static string ClientID = "ENTER_YOUR_CLIENT_ID";
    public static string RedirectUri = "msal" + ClientID + "://auth";
    public static string[] Scopes = { "User.Read", "Mail.Send", "Files.ReadWrite" };
    ```
    <span data-ttu-id="52f5e-p107">`Scopes` 値は、ユーザーが認証を行うときにアプリが要求する必要のある Microsoft Graph のアクセス許可スコープを保存します。`App` クラス コンストラクターが、ClientID 値を使用して MSAL `PublicClientApplication` クラスのインスタンスをインスタンス化する点に注意してください。ユーザーを認証するために後でこのクラスを使用します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p107">The `Scopes` value stores the Microsoft Graph permission scopes that the app will need to request when the user authenticates. Note that the `App` class constructor uses the ClientID value to instantiate an instance of the MSAL `PublicClientApplication` class. You'll use this class later to authenticate the user.</span></span>
    
    ```
    IdentityClientApp = new PublicClientApplication(ClientID);
    ```

3. <span data-ttu-id="52f5e-p108">UserDetailsClient.iOS\info.plist ファイルをテキスト エディターで開きます。残念ながらこのファイルは Visual Studio では編集できません。`<string>msalENTER_YOUR_CLIENT_ID</string>` 要素を `CFBundleURLSchemes` キーの下に配置します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p108">Open the UserDetailsClient.iOS\info.plist file in a text editor. Unfortunately you can't edit this file in Visual Studio. Locate the `<string>msalENTER_YOUR_CLIENT_ID</string>` element under `CFBundleURLSchemes` key.</span></span>

4. <span data-ttu-id="52f5e-p109">`ENTER_YOUR_CLIENT_ID` を、アプリの登録時に取得したアプリケーション ID の値と置き換えます。アプリケーション ID の前に `msal` を保持してください。結果の文字列値は、次のようになります: `<string>msal[application id]</string>`。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p109">Replace `ENTER_YOUR_CLIENT_ID` with the application id value that you got when you registered your app. Be sure to retain `msal` before the application id. The resulting string value should look like this: `<string>msal[application id]</string>`.</span></span>

5. <span data-ttu-id="52f5e-p110">UserDetailsClient.Droid\Properties\AndroidManifest.xml ファイルを開きます。次の要素を検索します: `<data android:scheme="msalENTER_YOUR_CLIENT_ID" android:host="auth" />`。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p110">Open the UserDetailsClient.Droid\Properties\AndroidManifest.xml file. Locate this element: `<data android:scheme="msalENTER_YOUR_CLIENT_ID" android:host="auth" />`.</span></span>

6. <span data-ttu-id="52f5e-p111">`ENTER_YOUR_CLIENT_ID` を、アプリの登録時に取得したアプリケーション ID の値と置き換えます。アプリケーション ID の前に `msal` を保持してください。結果の文字列値は、次のようになります: `<data android:scheme="msal[application id]" android:host="auth" />`。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p111">Replace `ENTER_YOUR_CLIENT_ID` with the application id value that you got when you registered your app. Be sure to retain `msal` before the application id. The resulting string value should look like this: `<data android:scheme="msal[application id]" android:host="auth" />`.</span></span>

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="52f5e-157">Microsoft Graph を使用してメールを送信する</span><span class="sxs-lookup"><span data-stu-id="52f5e-157">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="52f5e-158">スターター プロジェクトの MailHelper.cs ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-158">Open the MailHelper.cs file in your starter project.</span></span> <span data-ttu-id="52f5e-159">このファイルには、電子メールを作成して送信するコードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="52f5e-159">This file contains the code that constructs and sends an email.</span></span> <span data-ttu-id="52f5e-160">これは単一のメソッド (``ComposeAndSendMailAsync``) で構成されており、POST 要求を作成し、**https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** エンドポイントに送信します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-160">The MailHelper.cs file contains the code that constructs and sends an email. It consists of a single method --  -- that constructs and sends a POST request to the https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail endpoint.</span></span> 

<span data-ttu-id="52f5e-p113">``ComposeAndSendMailAsync`` メソッドは、MainPage.xaml.cs ファイルによって渡される``subject``、``bodyContent``、および``recipients`` の 3 つの文字列の値を取ります。``subject`` および ``bodyContent`` の文字列は、その他のすべての UI 文字列とともに AppResources.resx ファイルに格納されます。``recipients`` の文字列はアプリのインターフェイスにあるアドレス ボックスのものです。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p113">The ``ComposeAndSendMailAsync`` method takes three string values -- ``subject``, ``bodyContent``, and ``recipients`` -- that are passed to it by the MainPage.xaml.cs file. The ``subject`` and ``bodyContent`` strings are stored, along with all other UI strings, in the AppResources.resx file. The ``recipients`` string comes from the address box in the app's interface.</span></span> 

<span data-ttu-id="52f5e-164">**宣言の使用**</span><span class="sxs-lookup"><span data-stu-id="52f5e-164">**Using declarations**</span></span>

<span data-ttu-id="52f5e-165">ファイルの先頭にこれらの宣言があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-165">Make sure you have these declarations at the top of the file:</span></span>

```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Reflection;
using System.Threading.Tasks;
using Microsoft.Graph;
```

<span data-ttu-id="52f5e-p114">``ComposeAndSendMailAsync`` メソッド内の最初のタスクでは、Microsoft Graph から現在のユーザーの写真を取得します。この行は、スタブアウトした `GetCurrentUserPhotoStreamAsync` メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p114">The first task inside the ``ComposeAndSendMailAsync`` method is to get the current user's photo from Microsoft Graph. This line calls the stubbed-out `GetCurrentUserPhotoStreamAsync` method:</span></span>

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

<span data-ttu-id="52f5e-168">完全な `GetCurrentUserPhotoStreamAsync` メソッドは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-168">This is what the complete `GetCurrentUserPhotoStreamAsync` method looks like:</span></span>

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

<span data-ttu-id="52f5e-169">ユーザーが写真を持っていない場合、このロジックでは、プロジェクトに含まれている別のイメージ ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-169">If the user doesn't have a photo, this logic gets another image file that has been included with the project:</span></span>

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
            }
```

<span data-ttu-id="52f5e-170">イメージ ストリームを取得したら、スタブアウトした `UploadFileToOneDriveAsync` メソッドを呼び出してファイルを OneDrive にアップロードできます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-170">Now that we have an image stream, we can upload the file to OneDrive by calling the stubbed-out `UploadFileToOneDriveAsync` method:</span></span>

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

<span data-ttu-id="52f5e-171">完全な `UploadFileToOneDriveAsync` メソッドは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-171">This is what the complete `UploadFileToOneDriveAsync` method looks like:</span></span>

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

<span data-ttu-id="52f5e-172">このストリームは、次のメッセージとともに渡すことができる `MessageAttachmentsCollectionPage` オブジェクトの作成にも使用できます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-172">We can also use this stream to create a `MessageAttachmentsCollectionPage` object that we can pass along with the message:</span></span>

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

<span data-ttu-id="52f5e-p115">スタブアウトした `GetSharingLinkAsync` メソッドを呼び出して、新しくアップロードした OneDrive ファイルの共有リンクを取得できます。`bodyContent` 文字列には、共有リンクのプレースホルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p115">We can get a sharing link for the newly uploaded OneDrive file by calling the stubbed-out `GetSharingLinkAsync` method. The `bodyContent` string contains a placeholder for the sharing link:</span></span>

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

<span data-ttu-id="52f5e-175">完全な `GetSharingLinkAsync` メソッドは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-175">This is what the complete `GetSharingLinkAsync` method looks like:</span></span>

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

<span data-ttu-id="52f5e-176">複数のアドレスを渡すことができるため、次は、``recipients`` 文字列を一連の `EmailAddress` オブジェクトに分割します。それは、`Recipients` オブジェクトの一覧を作成するために使用され、そのオブジェクトは要求の POST 本文に入れて渡されます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-176">Since the user can potentially pass more than one address, the next task is to split the ``recipients`` string into a set of `EmailAddress` objects that can then be used to construct the list of `Recipients` objects that will be passed in the POST body of the request:</span></span>

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

<span data-ttu-id="52f5e-p116">最後に、`Message` オブジェクトを作成し、`GraphServiceClient` を使用して **me/microsoft.graph.SendMail** エンドポイントに送信します。``bodyContent`` の文字列は HTML 文書であるため、要求によって HTML に **ContentType** 値が設定されます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p116">The last task is to construct a `Message` object and send it to the **me/microsoft.graph.SendMail** endpoint through the `GraphServiceClient`. Since the ``bodyContent`` string is an HTML document, the request sets the **ContentType** value to HTML.</span></span>

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

<span data-ttu-id="52f5e-179">完全なクラスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-179">The complete class will look like this:</span></span>

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
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
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

<span data-ttu-id="52f5e-180">これで、Microsoft Graph と対話するために必要な、アプリの登録、ユーザーの認証、および要求の作成の 3 つの手順が完了しました。</span><span class="sxs-lookup"><span data-stu-id="52f5e-180">You've now performed the three steps required for interacting with Microsoft Graph: app registration, user authentication, and making a request.</span></span> 

## <a name="run-the-app"></a><span data-ttu-id="52f5e-181">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="52f5e-181">Run the app</span></span>
1. <span data-ttu-id="52f5e-p117">実行するプロジェクトを選びます。ユニバーサル Windows プラットフォームのオプションを選択すると、ローカル コンピューターでサンプルを実行できます。iOS プロジェクトを実行する場合は、[Xamarin ツールがインストールされた Mac](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/) に接続する必要があります。(また、このソリューションを Mac 上の Xamarin Studio で開いて、そこからサンプルを直接実行することもできます。)Android プロジェクトを実行する場合は、[Visual Studio Emulator for Android](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p117">Select the project that you want to run. If you select the Universal Windows Platform option, you can run the sample on the local machine. If you want to run the iOS project, you'll need to connect to a [Mac that has the Xamarin tools](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/) installed on it. (You can also open this solution in Xamarin Studio on a Mac and run the sample directly from there.) You can use the [Visual Studio Emulator for Android](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx) if you want to run the Android project.</span></span> 

    <span data-ttu-id="52f5e-186">![](images/SelectProject.png "Visual Studio でプロジェクトを選択する")</span><span class="sxs-lookup"><span data-stu-id="52f5e-186">![](images/SelectProject.png "Select project in Visual Studio")</span></span>

2. <span data-ttu-id="52f5e-p118">F5 キーを押して、ビルドとデバッグを実行します。ソリューションを実行し、個人用アカウント、あるいは職場または学校のアカウントのいずれかでサインインします。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p118">Press F5 to build and debug. Run the solution and sign in with either your personal or work or school account.</span></span>
    > <span data-ttu-id="52f5e-189">**注** ビルド構成マネージャーを開いて、ビルドと展開の手順が UWP プロジェクトに対して選択されていることを確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="52f5e-189">**Note** You might have to open the Build Configuration Manager to make sure that the Build and Deploy steps are selected for the UWP project.</span></span> 

3. <span data-ttu-id="52f5e-190">個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-190">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

4. <span data-ttu-id="52f5e-p119">**[メールの送信]** ボタンを選びます。メールが送信されると、成功メッセージが表示されます。このメール メッセージには添付ファイルとして写真が含まれており、OneDrive にアップロードされたファイルへの共有リンクも提供します。</span><span class="sxs-lookup"><span data-stu-id="52f5e-p119">Choose the **Send mail** button. When the mail is sent, a Success message is displayed. This mail message includes the photo as an attachment and also provides a sharing link to the uploaded file in OneDrive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="52f5e-194">次の手順</span><span class="sxs-lookup"><span data-stu-id="52f5e-194">Next steps</span></span>
- <span data-ttu-id="52f5e-195">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="52f5e-195">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="52f5e-196">[Xamarin.Forms 用 Microsoft Graph SDK スニペット ライブラリ](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample) で一般的な操作の例を検索するか、または GitHub 上のその他の [Xamarin サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin) を探してください。</span><span class="sxs-lookup"><span data-stu-id="52f5e-196">Find examples of common operations in the [Microsoft Graph SDK Snippets Library for Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample), or explore our other [Xamarin samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="52f5e-197">関連項目</span><span class="sxs-lookup"><span data-stu-id="52f5e-197">See also</span></span>
- [<span data-ttu-id="52f5e-198">Microsoft Graph .NET クライアント ライブラリ</span><span class="sxs-lookup"><span data-stu-id="52f5e-198">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="52f5e-199">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="52f5e-199">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="52f5e-200">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="52f5e-200">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-v2-tokens/)
