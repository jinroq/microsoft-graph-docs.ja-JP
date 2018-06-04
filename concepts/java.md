# <a name="get-started-with-microsoft-graph-in-a-java-app"></a><span data-ttu-id="7e3cd-101">Java アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="7e3cd-101">Get started with Microsoft Graph in a PHP app</span></span>

<span data-ttu-id="7e3cd-102">この記事では、[console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample) を使用して、Java コンソール アプリケーションから Microsoft Graph 経由でメールを送信する方法について順を追って説明します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-102">This article uses the [console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample) to walk through sending mail via Microsoft Graph from a Java console application.</span></span> <span data-ttu-id="7e3cd-103">この記事では、Microsoft Graph API を使用できるようにするために、Java アプリに追加する必要のあるコードについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-103">The article shows you the code that you need to add to your Java app so that you can use the Microsoft Graph API.</span></span> <span data-ttu-id="7e3cd-104">このアプリは、[Java 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-java) を使用して Microsoft Graph にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-104">The app accesses Microsoft Graph by using the [Microsoft Graph SDK for Java](https://github.com/microsoftgraph/msgraph-sdk-java).</span></span>

## <a name="choose-an-authentication-library"></a><span data-ttu-id="7e3cd-105">認証ライブラリの選択</span><span class="sxs-lookup"><span data-stu-id="7e3cd-105">Choosing an authentication library</span></span>

<span data-ttu-id="7e3cd-106">Microsoft Graph では OAuth 2.0 および Open ID Connect 標準を採用しているので、多彩なオープン ソース OAuth 2 Java ライブラリから選択できます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-106">Microsoft Graph adopted the OAuth 2.0 and Open ID Connect standards, which lets you choose from many available open source OAuth 2 Java libraries.</span></span> <span data-ttu-id="7e3cd-107">Azure AD チームは、Java 用の単純な OAuth2 ライブラリである [ScribeJava](https://github.com/scribejava/scribejava) の使用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-107">The Azure AD team recommends using [ScribeJava](https://github.com/scribejava/scribejava), a simple OAuth2 library for Java.</span></span>

<span data-ttu-id="7e3cd-108">以下のサンプルは、クライアント承認シナリオ、ユーザー、OAuth 2 対応エンドポイントで選択するのに適した、認証コードの付与フローを実装します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-108">The sample implements the Authorization Code Grant flow which is the right choice for a client authorization scenario, a user, and an OAuth 2-enabled endpoint.</span></span> <span data-ttu-id="7e3cd-109">運用サーバー間 Java アプリケーションでは、クライアント資格情報の認証フローが使用されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-109">In production server-to-server Java applications, the Client Credentials authorization flow is used.</span></span> <span data-ttu-id="7e3cd-110">**ScribeJava** は、これらの認証フローを両方とも処理します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-110">**ScribeJava** handles both of these authorization flows.</span></span> <span data-ttu-id="7e3cd-111">以下のサンプルは、登録、認証、実行をしやすくするため、最も簡単なフローでデモンストレーションします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-111">To make this sample easy to register, authenticate, and run, we demonstrate the simplest flow.</span></span>

<span data-ttu-id="7e3cd-112">アプリは、Microsoft Graph で呼び出しを行う前に、Azure Active Directory (Azure AD) からアクセス トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-112">Before your app can make calls on Microsoft Graph, the app must get an access token from Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7e3cd-113">このトークンは、Microsoft Graph に対する各呼び出しの HTTP 認証ヘッダー内に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-113">This token must be present in an HTTP authentication header with each call to Microsoft Graph.</span></span> <span data-ttu-id="7e3cd-114">[IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java) を実装すると、各呼び出しに対するヘッダーの挿入とトークンの追加を **Microsoft Graph SDK** が処理します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-114">The **Microsoft Graph SDK** takes care of inserting the header and adding the token for each call when you implement [IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java).</span></span> <span data-ttu-id="7e3cd-115">**ScribeJava** は認証とアクセス トークンの取得を処理します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-115">**ScribeJava** handles authentication and getting an access token.</span></span> <span data-ttu-id="7e3cd-116">アプリは、**IAuthenticationProvider** インターフェイス経由で Microsoft Graph SDK にアクセス トークンを提供します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-116">Your app provides the access token to the Microsoft Graph SDK via the **IAuthenticationProvider** interface.</span></span>

## <a name="install-and-run-the-sample"></a><span data-ttu-id="7e3cd-117">サンプルのインストールと実行</span><span class="sxs-lookup"><span data-stu-id="7e3cd-117">Install and run the solution</span></span>

<span data-ttu-id="7e3cd-118">サンプル アプリをインストールして設定するには、GitHub の **console-java-connect-sample** リポジトリにある「[Readme](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md)」ドキュメントの手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-118">To install and configure the sample app, follow the instructions in the [README](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md) document in the **console-java-connect-sample** repository on GitHub.</span></span> <span data-ttu-id="7e3cd-119">リポジトリを複製する次のコマンドを使用して、サンプルを複製し、お気に入りの Java IDE でコードを順を追って確認できます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-119">You can clone the sample and walk through the code in your favorite Java IDE by using this command to clone the repository:</span></span>

```
git@github.com:microsoftgraph/console-java-connect-sample.git
```

<span data-ttu-id="7e3cd-120">[コンソール Java 接続アプリを登録する](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app)際に、委任されたスコープ (アクセス許可) をサンプルに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-120">When you [register the Console Java Connect app](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app), assign delegated scopes (permissions) to the sample.</span></span> <span data-ttu-id="7e3cd-121">スコープは、必ず次の図に示すように設定します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-121">Be sure to scopes as shown in the following image:</span></span>

![Java 接続コンソール サンプルのアクセス許可](../concepts/images/console-java-connnect-sample-permissions.JPG)

<span data-ttu-id="7e3cd-123">アプリケーションを登録し、そのアプリケーション登録で入手する**アプリケーション ID** に合わせて[サンプルを構成する](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app)と、サンプルをビルドして実行できるようになります。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-123">After you register the application and [configure the sample](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app) for the **Application Id** you get from the application registration, you can build and run the sample.</span></span>

## <a name="console-java-connect-code"></a><span data-ttu-id="7e3cd-124">コンソール Java 接続コード</span><span class="sxs-lookup"><span data-stu-id="7e3cd-124">Console-Java-Connect code</span></span> 

<span data-ttu-id="7e3cd-125">サンプルのロジック フローを確認する前に、「[サンプル プロジェクトの構造](#sample-project-structure)」を概観してください。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-125">Before you look at the sample logic flow, take a few minutes to learn about the [sample project's structure](#sample-project-structure).</span></span> <span data-ttu-id="7e3cd-126">それが済んでから、以下に示すサンプルのロジックの説明に移るようにお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-126">When you're ready, lets step through the logic in the sample:</span></span>


   
### <a name="walk-through-the-code"></a><span data-ttu-id="7e3cd-127">コードの概観</span><span class="sxs-lookup"><span data-stu-id="7e3cd-127">Walk through the code</span></span>
<span data-ttu-id="7e3cd-128">まず、サンプル コードの全体像を説明し、次にメール メッセージの作成と送信に関する詳細を説明します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-128">We'll look at the sample code at a high level and then dive into the details of creating an email message and sending it.</span></span>

#### <a name="the-user-experience"></a><span data-ttu-id="7e3cd-129">ユーザー エクスペリエンス</span><span class="sxs-lookup"><span data-stu-id="7e3cd-129">The user experience</span></span>

<span data-ttu-id="7e3cd-130">この項では、アプリケーションの起動ロジックを説明し、ユーザーがサンプルを実行すると表示されるサンプル出力について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-130">This section takes a look at the logic that starts up the application and then shows you the sample output that the user sees when they run the sample.</span></span>

<span data-ttu-id="7e3cd-131">[PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) の **main** 静的メソッドが、**PublicClient** のインスタンスを作成し、サインインと認証プロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-131">The [PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) **main** static method creates an instance of **PublicClient** and then kicks off the sign in and authentication process.</span></span>  

<span data-ttu-id="7e3cd-132">[AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) は、ユーザーを Microsoft Graph に接続する際に使用されるシングルトン インスタンスを提供します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-132">[AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) provides a singleton instance which is used to connect the user to Microsoft Graph.</span></span> <span data-ttu-id="7e3cd-133">**AuthenticationManager** が、**アクセス トークン**を文字列プロパティとして公開します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-133">**AuthenticationManager** exposes an **access token** as a string property.</span></span> <span data-ttu-id="7e3cd-134">ユーザーが認証され、要求された Microsoft Graph リソースにアクセスする許可をサンプルに付与すると、このアクセス トークンが **Azure AD** によって返されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-134">The access token is returned by **Azure AD** when the user is authenticated and gives the sample permission to access requested Microsoft Graph resources.</span></span> 

<span data-ttu-id="7e3cd-135">**PublicClient.startSendMail** メソッドが、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-135">The **PublicClient.startSendMail** method performs the following steps:</span></span>

- <span data-ttu-id="7e3cd-136">[GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java) クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-136">Creates a new instance of the  [InputComponentSubmission](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java) class.</span></span> 
- <span data-ttu-id="7e3cd-137">サンプル コンソール オブジェクトがユーザーに表示するプロンプトのパーソナル設定を行えるように、**GraphSendMail.getMeUser()** を呼び出して、現在のユーザーの **Azure AD** プロファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-137">Calls **GraphSendMail.getMeUser()** to return the **Azure AD** profile of the current user so that the sample console object can personalize the prompts that it displays to the user.</span></span> 
- <span data-ttu-id="7e3cd-138">コンソールに次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-138">The console displays:</span></span>

   `Hello, Laura Steele. Would you like to send an email to yourself or someone else?`

   `Enter the address to which you'd like to send a message. If you enter nothing, the message will go to your address`

- <span data-ttu-id="7e3cd-139">ユーザーの入力を処理する **GraphSendMail.sendMail** メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-139">Calls the **GraphSendMail.sendMail** method which takes the user's input.</span></span> <span data-ttu-id="7e3cd-140">メール アドレスが入力された場合、**sendMail** はそのアドレスにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-140">If an email address is provided, **sendMail** sends a message to that address.</span></span> <span data-ttu-id="7e3cd-141">入力されなかった場合は、現在のユーザーにそのメッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-141">Otherwise, the message is sent to the current user.</span></span> 

- <span data-ttu-id="7e3cd-142">別のメールを送信するか、コンソール アプリを終了するかをユーザーに確認するプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-142">Prompts the user to send another email or quit the console app.</span></span>

   `Email sent!`

   `Want to send another message? Type 'y' for yes and any other key to exit.`

#### <a name="the-send-mail-logic"></a><span data-ttu-id="7e3cd-143">メールの送信ロジック</span><span class="sxs-lookup"><span data-stu-id="7e3cd-143">The send mail logic</span></span>

<span data-ttu-id="7e3cd-144">メールの送信ロジックは次の手順で行われます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-144">The mail sending logic takes the following steps:</span></span>



1. <span data-ttu-id="7e3cd-145">**プロフィール画像の取得**:</span><span class="sxs-lookup"><span data-stu-id="7e3cd-145">Get profile picture</span></span><br/> <span data-ttu-id="7e3cd-146">**GraphServiceController.getUserProfilePicture()** を呼び出して、サンプルにサインインしている **Azure AD** ユーザーのプロフィール画像を表すバイトの配列を取得します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-146">Calls **GraphServiceController.getUserProfilePicture()** to get an array of bytes representing the profile picture of the **Azure AD** user who signed into the sample.</span></span>

   <span data-ttu-id="7e3cd-147">**API 呼び出し**</span><span class="sxs-lookup"><span data-stu-id="7e3cd-147">**The API call**</span></span>

```java
            photoStream = mGraphServiceClient
                    .me()
                    .photo()
                    .content()
                    .buildRequest()
                    .get();

```
2. <span data-ttu-id="7e3cd-148">**OneDrive への画像のアップロード**:</span><span class="sxs-lookup"><span data-stu-id="7e3cd-148">**Upload picture to OneDrive**:</span></span>
<br/><span data-ttu-id="7e3cd-149">**GraphServiceController.uploadPictureToOneDrive(bytes)** を呼び出して、そのユーザーの OneDrive のルート フォルダーにあるプロフィール画像を POST します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-149">Calls **GraphServiceController.uploadPictureToOneDrive(bytes)** to POST the profile picture in the user's OneDrive root folder.</span></span> <span data-ttu-id="7e3cd-150">Microsoft Graph SDK の **DriveItem** オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-150">A Microsoft Graph SDK **DriveItem** object is returned.</span></span> 

   <span data-ttu-id="7e3cd-151">**API 呼び出し**</span><span class="sxs-lookup"><span data-stu-id="7e3cd-151">**The API call**</span></span>
```java
            driveItem = mGraphServiceClient
                    .me()
                    .drive()
                    .root()
                    .itemWithPath("me2.png")
                    .content()
                    .buildRequest()
                    .put(picture);

```
3. <span data-ttu-id="7e3cd-152">**画像の OneDrive 共有リンクの取得**:</span><span class="sxs-lookup"><span data-stu-id="7e3cd-152">**Get the OneDrive sharing link for the picture**:</span></span><br/><span data-ttu-id="7e3cd-153">**GraphServiceController.getPermissionSharingLink** を呼び出して、新しい共有リンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-153">Calls **GraphServiceController.getPermissionSharingLink** to create a new sharing link.</span></span> <span data-ttu-id="7e3cd-154">Microsoft Graph SDK の **Permission** オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-154">A Microsoft Graph SDK **Permission** object is returned.</span></span>

   <span data-ttu-id="7e3cd-155">**API 呼び出し**</span><span class="sxs-lookup"><span data-stu-id="7e3cd-155">**The API call**</span></span>
```java
            permission = mGraphServiceClient
                    .me()
                    .drive()
                    .items(id)
                    .createLink("view", "organization")
                    .buildRequest()
                    .post();

```
4. <span data-ttu-id="7e3cd-156">前の手順で作成した共有リンクの **webUrl** で、**HTML テンプレートのアンカー タグの内容を置換**します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-156">**Replace the contents of the HTML template anchor tag** with the **webUrl** for the sharing link in the previous step.</span></span> 
> <span data-ttu-id="7e3cd-157">**注:** アプリケーションから送信されたメッセージの本文は、[Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java) に静的な文字列として保存される HTML テンプレートとして生成されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-157">**Note:** The body of the message sent by the application originates as an HTML template stored in [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java) as a static string.</span></span> <span data-ttu-id="7e3cd-158">送信時に、メッセージの本文には、サンプルがユーザーの OneDrive ルート フォルダーにアップロードする画像へのパブリック共有ハイパーリンクが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-158">When sent, the body of the message contains a public sharing hyperlink to a picture that the sample uploads to the user's OneDrive root folder.</span></span> 
5. <span data-ttu-id="7e3cd-159">**下書きメッセージの作成**:</span><span class="sxs-lookup"><span data-stu-id="7e3cd-159">Create a draft message</span></span> <br/><span data-ttu-id="7e3cd-160">**GraphServiceController.createDraftMail** を呼び出し、受信者のメール アドレス、件名のテキスト、および更新された HTML テンプレートを渡します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-160">Calls **GraphServiceController.createDraftMail**, passing the recipient email address, subject text, and the updated HTML template.</span></span> <span data-ttu-id="7e3cd-161">下書きメッセージが作成され、ユーザーの下書きメッセージ フォルダーに POST されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-161">A draft message is created and POSTed to the user's draft message folder.</span></span>

   <span data-ttu-id="7e3cd-162">**API 呼び出し**</span><span class="sxs-lookup"><span data-stu-id="7e3cd-162">**The API call**</span></span>
```java
            message = mGraphServiceClient
                    .me()
                    .messages()
                    .buildRequest()
                    .post(message);

```
6. <span data-ttu-id="7e3cd-163">**下書きメッセージへの画像添付**:</span><span class="sxs-lookup"><span data-stu-id="7e3cd-163">**Attach picture to draft message**:</span></span> <br/><span data-ttu-id="7e3cd-164">**GraphServiceController.addPictureToDraftMessage** を呼び出し、下書きメッセージを取得して、オブジェクトの添付ファイルとしてメッセージに画像を追加します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-164">Calls **GraphServiceController.addPictureToDraftMessage** to get the draft message and add the picture to the message as an object attachment.</span></span>

   <span data-ttu-id="7e3cd-165">**API 呼び出し**</span><span class="sxs-lookup"><span data-stu-id="7e3cd-165">**The API call**</span></span>
```java
            FileAttachment fileAttachment = new FileAttachment();
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment";
            fileAttachment.contentBytes = attachementBytes;
            fileAttachment.name = "me.png";
            fileAttachment.size = attachementBytes.length;
            fileAttachment.isInline = false;
            fileAttachment.id = "my profile picture";

            attachment = mGraphServiceClient
                    .me()
                    .messages(messageId)
                    .attachments()
                    .buildRequest()
                    .post(fileAttachment);

```
7. <span data-ttu-id="7e3cd-166">**下書きメッセージの送信**:</span><span class="sxs-lookup"><span data-stu-id="7e3cd-166">**Send the draft message**:</span></span><br/><span data-ttu-id="7e3cd-167">**GraphServiceController.sendDraftMessage** を呼び出し、更新した下書きメッセージを意図したユーザーに送信します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-167">Calls **GraphServiceController.sendDraftMessage** to send the updated draft message to the intended user.</span></span>

   <span data-ttu-id="7e3cd-168">**API 呼び出し**</span><span class="sxs-lookup"><span data-stu-id="7e3cd-168">**The API call**</span></span>
```java
            mGraphServiceClient
                    .me()
                    .mailFolders("Drafts")
                    .messages(messageId)
                    .send()
                    .buildRequest()
                    .post();

```



### <a name="sample-project-structure"></a><span data-ttu-id="7e3cd-169">サンプル プロジェクトの構造</span><span class="sxs-lookup"><span data-stu-id="7e3cd-169">Sample project structure</span></span>

### <a name="connect-package"></a><span data-ttu-id="7e3cd-170">接続パッケージ</span><span class="sxs-lookup"><span data-stu-id="7e3cd-170">connect package</span></span>
<span data-ttu-id="7e3cd-171">このパッケージには、OAuth2 認証フロー ロジック、および更新対象の構成が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-171">This package contains the OAuth2 authentication flow logic and the configuration that you'll be updating.</span></span>

- <span data-ttu-id="7e3cd-172">[AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java): このクラスは、認証コードの付与フローで使用する **ScribeJava** オブジェクトをインポートします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-172">[AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java):  This class imports the  **ScribeJava** objects used for the Authorization Code Grant flow.</span></span>
- <span data-ttu-id="7e3cd-173">[Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java): アプリの登録に関連した値を提供するパブリックの静的文字列と、アプリケーションが送信するメール メッセージのテンプレートを格納しています。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-173">[Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java): Holds public static strings for providing app registration related values and the template for the email message that the application sends.</span></span>
- <span data-ttu-id="7e3cd-174">[Debug.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java): パブリック デバッグ レベルのフラグです。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-174">[Debug.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java): Public debug level flag.</span></span> <span data-ttu-id="7e3cd-175">値を設定して、サンプル アプリのログの動作を変更します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-175">Set it's value to change the logging behavior of the sample app.</span></span>
- <span data-ttu-id="7e3cd-176">[DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java): デバッグ レベル設定に従って、コンソールに情報を書き込むログ ユーティリティです。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-176">[DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java): Logging utility that writes information to the console according to the debug level set.</span></span>
- <span data-ttu-id="7e3cd-177">[IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java): **ScribeJava.getAccessToken** メソッドの非同期オーバーロードを呼び出す場合に使用するコールバック メソッドを定義します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-177">[IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java): Defines the callback method that you'd use if you call the asynchronous overload of the **ScribeJava.getAccessToken** method.</span></span>
- <span data-ttu-id="7e3cd-178">[SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java): **Exception** の派生クラスで、Microsoft Graph 固有の例外情報をカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-178">[SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java): A class that is derived from **Exception** and encapsulates Microsoft Graph-specific exception information.</span></span> <span data-ttu-id="7e3cd-179">**GraphSendMail** パッケージのクラスは、この種類の例外をスローする場合があります。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-179">Classes in the **GraphSendMail** package can throw this type of exception.</span></span>

### <a name="msgraph-package"></a><span data-ttu-id="7e3cd-180">msgraph パッケージ</span><span class="sxs-lookup"><span data-stu-id="7e3cd-180">msgraph package</span></span>

<span data-ttu-id="7e3cd-181">このパッケージには、Microsoft Graph で呼び出しを実行するロジックが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-181">This package contains all of the logic that makes calls on Microsoft Graph.</span></span>

- <span data-ttu-id="7e3cd-182">[GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java): 呼び出しを **GraphServiceController** (Microsoft Graph API サンプル ヘルパー クラス) に連鎖して、画像が添付されたメール メッセージを作成および送信します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-182">[GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java): Chains together calls into **GraphServiceController** (a Microsoft Graph API sample helper class) to create and send an email message with a picture attachment.</span></span>
- <span data-ttu-id="7e3cd-183">[GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java): Microsoft Graph SDK [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java) をインスタンス化し、Microsoft Graph エンドポイント上のすべての発信 API 呼び出しにアクセス トークンを追加します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-183">[GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java): Instantiates the Microsoft Graph SDK [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java) and adds an access token to all outgoing API calls on the Microsoft Graph endpoint.</span></span>

- <span data-ttu-id="7e3cd-184">[GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java): Microsoft Graph SDK を使用して、**GraphServiceClient** 上のすべての呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-184">[GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java): Uses the Microsoft Graph SDK to make all of the calls on the **GraphServiceClient**.</span></span> <span data-ttu-id="7e3cd-185">次の呼び出しが作成されます。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-185">Calls include:</span></span>

   - <span data-ttu-id="7e3cd-186">**createDraftMail**: メール メッセージの下書きを作成し、下書きメッセージ フォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-186">**createDraftMail**: creates a draft email message and saves it in your draft messages folder.</span></span>
   - <span data-ttu-id="7e3cd-187">**sendNewMessageAsync**: メール メッセージを作成および送信します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-187">**sendNewMessageAsync**: Creates and sends an email message.</span></span>
   - <span data-ttu-id="7e3cd-188">**addPictureToDraftMessage**: メッセージ ID で、下書きメッセージの添付ファイルを POST します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-188">**addPictureToDraftMessage**: Posts a file attachment in a draft message by message Id</span></span>
   - <span data-ttu-id="7e3cd-189">**addAttachmentToDraftAsync**: 下書きメッセージに添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-189">**addAttachmentToDraftAsync**: Adds an attachment to a draft message.</span></span>
   - <span data-ttu-id="7e3cd-190">**sendDraftMessage**: 下書きフォルダーからメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-190">**sendDraftMessage**: Sends a message from the drafts folder.</span></span>
   - <span data-ttu-id="7e3cd-191">**getDraftMessage**: メッセージ ID で、ユーザーのメッセージ コレクションからメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-191">**getDraftMessage**: Gets a message from the user' message collection by message id.</span></span>
   - <span data-ttu-id="7e3cd-192">**getUser**: Microsoft Graph API エンドポイントで認証されるローカル ユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-192">**getUser**: Gets the local user who is authenticated with the Microsoft Graph API endpoint.</span></span>
   - <span data-ttu-id="7e3cd-193">**getUserProfilePicture**: サインインしているユーザーのプロフィール画像を Microsoft Graph から取得します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-193">**getUserProfilePicture**: Gets the signed in user's profile picture from the Microsoft Graph.</span></span>
   - <span data-ttu-id="7e3cd-194">**uploadPictureToOneDrive**: 画像をバイト配列として、ユーザーの OneDrive ルート フォルダーにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-194">**uploadPictureToOneDrive**: Uploads a picture as byte array to the user's OneDrive root folder.</span></span>
   - <span data-ttu-id="7e3cd-195">**getPermissionSharingLink**: OneDrive に保存されている画像への公開共有リンクを作成するように OneDrive に要求します。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-195">**getPermissionSharingLink**: Requests OneDrive to create a public sharing link to a picture stored in OneDrive.</span></span>

## <a name="other-microsoft-graph-samples"></a><span data-ttu-id="7e3cd-196">Microsoft Graph の他のサンプル</span><span class="sxs-lookup"><span data-stu-id="7e3cd-196">Other Microsoft Graph Snippets samples</span></span>

<span data-ttu-id="7e3cd-197">ご覧になりたい特定のサンプルがある場合、[懸案事項を送信](https://github.com/microsoftgraph/console-java-connect-sample/issues)してお知らせください。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-197">If there's a particular sample you'd like to see, please let us know by [submitting an issue](https://github.com/microsoftgraph/console-java-connect-sample/issues).</span></span> <span data-ttu-id="7e3cd-198">Java で構築する Microsoft Graph シナリオに対するお客様のフィードバックを大いに歓迎いたします。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-198">We're very interested in your feedback on any Microsoft Graph scenario you'd like to build in Python!</span></span>

<span data-ttu-id="7e3cd-199">Microsoft Graph API は、あらゆる種類の Microsoft データとの対話に使用できる、非常に強力な統合 API です。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-199">The Microsoft Graph API is a very powerful, unifiying API that can be used to interact with all kinds of Microsoft data.</span></span> <span data-ttu-id="7e3cd-200">[開発者ドキュメント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/overview)または [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) で、Microsoft Graph によってさらに行える事柄について確認してください。</span><span class="sxs-lookup"><span data-stu-id="7e3cd-200">Check out the [developer documentation](https://developer.microsoft.com/ja-JP/graph/docs/concepts/overview) or the [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) to explore what else you can accomplish with Microsoft Graph.</span></span>
