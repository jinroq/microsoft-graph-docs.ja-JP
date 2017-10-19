# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a><span data-ttu-id="ae477-101">Objectve C iOS アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="ae477-101">Get started with Microsoft Graph in an iOS App</span></span>

> <span data-ttu-id="ae477-p101">**エンタープライズのお客様向けにアプリを作成していますか?**エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ae477-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="ae477-p102">**すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure 管理ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae477-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="ae477-p103">この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[iOS (SDK) 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-objectivec-connect-sample)内のコードを説明し、Microsoft Graph を使用するアプリで実装する必要のある主要な概念について説明します。[iOS 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios) を使用して Microsoft Graph にアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="ae477-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="ae477-110">作成するアプリのバージョンを、この GitHub リポジトリからダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="ae477-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="ae477-111">Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル</span><span class="sxs-lookup"><span data-stu-id="ae477-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="ae477-112">次の画像は、作成するアプリを示しています。</span><span class="sxs-lookup"><span data-stu-id="ae477-112">The following image shows the app you'll create.</span></span>

![Connect のサンプル チュートリアル。アプリにおける接続とメールの送信を示します](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="ae477-114">ワークフローは、Microsoft Graph への接続/認証を行い、職場または個人用アカウントでサインインし、最後に受信者に向けてメールを送信する、というものです。</span><span class="sxs-lookup"><span data-stu-id="ae477-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="ae477-p104">**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/en-us/getting-started)」を使用すれば、すばやく稼働させることができます。</span><span class="sxs-lookup"><span data-stu-id="ae477-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae477-117">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae477-117">Prerequisites</span></span>

<span data-ttu-id="ae477-118">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="ae477-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="ae477-119">Apple 社の [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="ae477-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="ae477-120">依存関係マネージャーとしての [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) のインストール。</span><span class="sxs-lookup"><span data-stu-id="ae477-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="ae477-121">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="ae477-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="ae477-122">[iOS 用 Microsoft Graph スターター プロジェクト](https://github.com/microsoftgraph/ios-objectivec-connect-sample)。</span><span class="sxs-lookup"><span data-stu-id="ae477-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="ae477-123">このテンプレートには、コードを追加するクラスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae477-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="ae477-124">このプロジェクトを取得するには、この場所からサンプル プロジェクトを複製するかダウンロードして、**starter-project** フォルダー内のワークスペース (**ios-objectivec-connect-sample.xcworkspace**) で作業します。</span><span class="sxs-lookup"><span data-stu-id="ae477-124">The Microsoft Graph Starter Project for iOS. This template contains classes that you'll add code to. To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="ae477-125">アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="ae477-125">Register the app</span></span>
 
1. <span data-ttu-id="ae477-126">個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ae477-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="ae477-127">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae477-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="ae477-128">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae477-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="ae477-129">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="ae477-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="ae477-130">**[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae477-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="ae477-131">**[ネイティブ プラットフォーム]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae477-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="ae477-p106">クライアント ID をクリップボードにコピーします。サンプル アプリにこの値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae477-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="ae477-134">アプリ ID は、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="ae477-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="ae477-135">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="ae477-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="ae477-136">プロジェクトの依存関係のインポート</span><span class="sxs-lookup"><span data-stu-id="ae477-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="ae477-137">このリポジトリ ([Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-objectivec-connect-sample)) を複製します。</span><span class="sxs-lookup"><span data-stu-id="ae477-137">[Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample)</span></span> 
><span data-ttu-id="ae477-138">重要: プロジェクトのルートにあるサンプルではなく、starter-project フォルダーのサンプルを使用してください。</span><span class="sxs-lookup"><span data-stu-id="ae477-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="ae477-p107">CocoaPods を使用して、Microsoft Graph SDK と認証の依存関係をインポートします。このサンプル アプリには、プロジェクトに pod を取り込む podfile が既に含まれています。**ターミナル** アプリでフォルダー **starter-project** に移動し、**ターミナル**から以下を実行します。</span><span class="sxs-lookup"><span data-stu-id="ae477-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="ae477-p108">pod がプロジェクトにインポートされたことの確認が表示されます。詳細については、「[CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ae477-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="ae477-144">キーチェーンの共有の有効化</span><span class="sxs-lookup"><span data-stu-id="ae477-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="ae477-p109">Xcode8 には、キーチェーンのグループを追加する必要があります。これを行わないと、アプリがキーチェーンにアクセスできなくなります。キーチェーン グループを追加するには:</span><span class="sxs-lookup"><span data-stu-id="ae477-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="ae477-p110">Xcode のプロジェクト マネージャーのパネルで、プロジェクトを選択します (⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="ae477-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="ae477-149">**iOS-ObjectiveC-Connect-Sample** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae477-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="ae477-150">[機能] タブで **[キーチェーンを共有]** を有効にします。</span><span class="sxs-lookup"><span data-stu-id="ae477-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="ae477-151">**com.microsoft.ios-objectivec-connect-sample** をキーチェーン グループに追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-151">Add **com.microsoft.O365-iOS-Microsoft-Graph-SDK** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="ae477-152">Microsoft Graph での認証</span><span class="sxs-lookup"><span data-stu-id="ae477-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="ae477-p111">UI のワークフローを見直すため、アプリはユーザーに認証を実行させます。こうすると指定されたユーザーにメールを送信できるようになります。Microsoft Graph サービスに対して要求を実行するには、適切な OAuth 2.0 ベアラー トークンを使用して HTTPS 要求を認証できる認証プロバイダーを指定する必要があります。サンプル プロジェクトには、既にスタブ アウトされていた **AuthenticationProvider.m** という認証クラスがあります。Microsoft Graph API を呼び出すためのアクセス トークンを要求および取得する関数を追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-p111">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="ae477-157">**starter-project** フォルダー内の Xcode プロジェクト ワークスペース (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) を開き、**Authentication** フォルダーに移動して、ファイルの **AuthenticationProvider.m.** を開きます。</span><span class="sxs-lookup"><span data-stu-id="ae477-157">Open the Xcode project workspace (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.** Add the following code to that class.</span></span> <span data-ttu-id="ae477-158">そのクラスに次のコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-158">Add the following code to the body of the class:</span></span>

```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)    (NSError *))completion{
      [NXOAuth2AuthenticationProvider setClientId:kClientId scopes:scopes];
      /**
      Obtains access token by performing login with UI, where viewController specifies the parent view controller.
      @param viewController The view controller to present the UI on.
      @param completionHandler The completion handler to be called when the authentication has completed.
      error should be non nil if there was no error, and should contain any error(s) that occurred.
      */

      if ([[NXOAuth2AuthenticationProvider sharedAuthProvider] loginSilent]) {
         completion(nil);
      }
      else {
         [[NXOAuth2AuthenticationProvider sharedAuthProvider] loginWithViewController:nil completion:^(NSError *error) {
            if (!error) {
               NSLog(@"Authentication successful.");
               completion(nil);
            }
            else {
               NSLog(@"Authentication failed - %@", error.localizedDescription);
               completion(error);
            }
         }];
      }
   }
```     

2. <span data-ttu-id="ae477-p113">次にヘッダー ファイルにメソッドを追加します。ファイル **AuthenticationProvider.h** を開き、このクラスに次のコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-p113">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. <span data-ttu-id="ae477-p114">最後に、**ConnectViewController.m** からこのメソッドを呼び出します。このコントローラーはアプリが読み込む既定のビューであり、**[Connect]** という 1 つのボタンがあり、ユーザーがこれをタップすると認証プロセスが開始します。このメソッドには **Client ID** と **scopes** という 2 つのパラメーターを指定します。これらについては以下の部分で詳しく説明します。次の処理を **ConnectViewController.m** に追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-p114">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

```objectivec
- (IBAction)connectTapped:(id)sender {
   [self showLoadingUI:YES];
   NSArray *scopes = [kScopes componentsSeparatedByString:@","];
   [self.authProvider connectToGraphWithClientId:kClientId scopes:scopes completion:^(NSError *error) {
   if (!error) {
      [self performSegueWithIdentifier:@"showSendMail" sender:nil];
      [self showLoadingUI:NO];
      NSLog(@"Authentication successful.");
   }
   else{
      NSLog(NSLocalizedString(@"CHECK_LOG_ERROR", error.localizedDescription));
      [self showLoadingUI:NO];
   };
  }];
}
```     

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="ae477-165">Microsoft Graph を使用して電子メールを送信する</span><span class="sxs-lookup"><span data-stu-id="ae477-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="ae477-p115">認証できるようにプロジェクトを構成したら、次のタスクは、Microsoft Graph API を使用してユーザーにメールを送信することです。既定では、ログインしているユーザーが受信者ですが、他の任意の受信者に変更することができます。ここで操作するコードは **Controllers** フォルダーと **SendMailViewController.m** クラスにあります。ここには、UI を表す他のコードや、Microsoft Graph サービスからユーザー プロファイル情報を取得するヘルパー メソッドも入っています。メール メッセージの作成とそのメッセージの送信を行うメソッドに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="ae477-p115">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="ae477-171">Controllers フォルダー内の **SendMailViewController.m** を開いて、**viewDidLoad** メソッドの `self.graphClient = [MSGraphClient client]` の後に次のコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-171">Open SendMailViewController.m. in the Controllers folder and add the following helper method to the class:</span></span>
   ```objectivec
       [self getUserInfo:(self.emailAddress) completion:^( NSError *error) {
        if (!error) {
            [self getUserPicture:(self.emailAddress)  completion:^(UIImage *image, NSError *error) {
                if (!error) {
                    self.userPicture = image;
                } else {
                    //get the test image out of the project resources
                    self.userPicture = [UIImage imageNamed:(@"test.png")];
                }
                [self uploadPictureToOneDrive:(self.userPicture) completion:^(NSString *webUrl, NSError *error) {
                    if (!error) {
                        self.pictureWebUrl = webUrl;
                        dispatch_async(dispatch_get_main_queue(), ^{
                            self.sendMailButton.enabled = true;
                        });
                    } else {
                        dispatch_async(dispatch_get_main_queue(), ^{
                            NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                            self.statusTextView.text = NSLocalizedString(@"PICTURE_UPLOAD_FAILURE", comment: "");
                        });
                    }
                }];
            }];
        }
    }];
   ```

1. <span data-ttu-id="ae477-172">Controllers フォルダー内の **SendMailViewController.m** を開いて、</span><span class="sxs-lookup"><span data-stu-id="ae477-172">Open **SendMailViewController.m.**</span></span> <span data-ttu-id="ae477-173">このクラスに次のヘルパー メソッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-173">Open SendMailViewController.m. in the Controllers folder and add the following helper method to the class:</span></span>
```objectivec
  //Create a sample test message to send to specified user account
  -(MSGraphMessage*) getSampleMessage{
      MSGraphMessage *message = [[MSGraphMessage alloc]init];
      MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
      MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
      //need to get email text field for send to!
    
      email.address = self.emailAddress;
      toRecipient.emailAddress = email;
    
      NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
      [toRecipients addObject:toRecipient];
    
      message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
      MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
      NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
      NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
      emailBody.content = htmlContentString;
      NSString *replaceString = @"a href=";
      replaceString = [replaceString stringByAppendingString:(self.pictureWebUrl)];
      emailBody.content = [emailBody.content stringByReplacingOccurrencesOfString:(@"a href=%s") withString:(replaceString)];
      emailBody.contentType = [MSGraphBodyType html];
      message.body = emailBody;
    
      message.toRecipients = toRecipients;
    
      MSGraphFileAttachment *fileAttachment= [[MSGraphFileAttachment alloc]init];
      fileAttachment.oDataType = @"#microsoft.graph.fileAttachment";
      fileAttachment.contentType = @"image/png";
    
      NSString *decodedString = [UIImagePNGRepresentation(self.userPicture) base64EncodedStringWithOptions:NSDataBase64EncodingEndLineWithCarriageReturn];
    
      fileAttachment.contentBytes = decodedString;
      fileAttachment.name = @"me.png";
      message.attachments = [message.attachments arrayByAddingObject:(fileAttachment)];
      return message;
    
    }
```
3. <span data-ttu-id="ae477-174">**SendMailViewController.m** を開きます。このクラスに次のメソッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-174">Open **SendMailViewController.m.** Add the following send mail method to the class.</span></span>
<span data-ttu-id="ae477-175">**uploadPictureToOneDrive** によって、[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) の情報からの [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) のプロフィール画像がアップロードされ、サンプルによって送信される電子メールの本文に埋め込まれる Web 共有 URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="ae477-175">**uploadPictureToOneDrive** uploads the [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)'s profile picture from their [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) information and returns the web sharing Url to be embedded in the body of the email that is sent by the sample.</span></span>

  ```objectivec
  -(void) uploadPictureToOneDrive: (UIImage *) image completion:(void(^) (NSString*, NSError*))completionBlock{
    
    NSData *data = UIImagePNGRepresentation(image);
    [[[[[[[self.graphClient me]
          drive]
         root]
        children]
       driveItem:(@"me.png")]
      contentRequest]
     uploadFromData:(data) completion:^(MSGraphDriveItem *response, NSError *error) {
         
         if (!error) {
             NSString *webUrl = response.webUrl;
             completionBlock(webUrl, error);
         } else {
             dispatch_async(dispatch_get_main_queue(), ^{
                 self.statusTextView.text =  NSLocalizedString(@"USER_GET_PICTURE_FAILURE", comment: "");
                 NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
             });
         }
     }];
    }
  ```
4. <span data-ttu-id="ae477-176">**SendMailViewController.m** を開き、このクラスに次のメソッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-176">Open **SendMailViewController.m.** in the Controllers folder and add the following helper method to the class:</span></span> 
<span data-ttu-id="ae477-177">[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) のプロフィール画像がある場合、**getUserPicture** によってその画像が返されます。</span><span class="sxs-lookup"><span data-stu-id="ae477-177">**getUserPicture** returns the [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)'s profile picture if it is available.</span></span>
   ```objectivec
   -(void) getUserPicture: (NSString *)url completion:(void(^) (UIImage*, NSError*))completionBlock {
    
    [[[self.graphClient me] photoValue] downloadWithCompletion:^(NSURL *location, NSURLResponse *response, NSError *error) {
        //code
        if (!error) {
            NSData *data = [NSData dataWithContentsOfURL:location];
            UIImage *img = [[UIImage alloc] initWithData:data];
            completionBlock(img, error);
        } else{
            completionBlock(nil, error);

        }
    }];
    }

   ```
3. <span data-ttu-id="ae477-178">**SendMailViewcontroller.m** を開き、このクラスに次のメソッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-178">Open **SendMailViewController.m.** in the Controllers folder and add the following helper method to the class:</span></span>
<span data-ttu-id="ae477-179">このメソッドでは、認証されたユーザーを示す [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) リソースを取得し、ユーザーのプロフィール画像を取得して電子メールを送信するために必要なフィールドをキャッシュします。</span><span class="sxs-lookup"><span data-stu-id="ae477-179">This method gets the [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) resource representing the authenticated user and caches the fields necessary to get the user's profile picture and send an email.</span></span>
   ```objectivec
   //Retrieve the logged in user's display name and email address
   -(void) getUserInfo: (NSString *)url completion:(void(^) ( NSError*))completionBlock{
    
    [[[self.graphClient me]request]getWithCompletion:^(MSGraphUser *response, NSError *error) {
        if(!error){
            dispatch_async(dispatch_get_main_queue(), ^{
                self.emailAddress = response.userPrincipalName;
                self.emailTextField.text = self.emailAddress;
                self.headerLabel.text = [NSString stringWithFormat:(NSLocalizedString(@"HI_USER", comment "")), response.displayName];
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_SUCCESS", comment: "");
            });

            completionBlock(nil);
        }
        else{
            dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_FAILURE", comment: "");
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            });
            completionBlock(error);
        }
    }];
    
   }

   ```
3. <span data-ttu-id="ae477-180">**SendMailViewController.m** を開きます。このクラスに次の送信メール メソッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae477-180">Open **SendMailViewController.m.** Add the following send mail method to the class.</span></span>
<span data-ttu-id="ae477-181">**getSampleMessage** によって、デモのために使用する HTML 形式のサンプル メールの下書きが作成されます。</span><span class="sxs-lookup"><span data-stu-id="ae477-181">**getSampleMessage** creates a draft HTML sample mail to use for demo purposes.</span></span> <span data-ttu-id="ae477-182">すると、次のメソッド (**sendMail**) がそのメッセージを受け取り、それを送信するための要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="ae477-182">So getSampleMessage creates a draft HTML sample mail to use for demo purposes. The next method, **sendMail**, then takes that message and executes the request to send it. Again the default recipient is the signed-in user.</span></span> <span data-ttu-id="ae477-183">この場合も、既定の受信者はサインインしているユーザーです。</span><span class="sxs-lookup"><span data-stu-id="ae477-183">Again the default recipient is the signed-in user.</span></span>


  ```objectivec
   //Send mail to the specified user in the email text field
   -(void) sendMail {
    MSGraphMessage *message = [self getSampleMessage];
    MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
    NSLog(@"%@", requestBuilder);
    MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
    [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
        if(!error){
            NSLog(@"response %@", response);
             dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                self.descriptionLabel.text = @"Check your inbox. You have a new message :)";
            });
        }
        else {
            dispatch_async(dispatch_get_main_queue(), ^{
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
            });
        }
    }];
   }
   ```



## <a name="run-the-app"></a><span data-ttu-id="ae477-184">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="ae477-184">Run the app</span></span>
1. <span data-ttu-id="ae477-p121">サンプルを実行する前に、セクション「**アプリの登録**」で登録プロセスから受け取ったクライアント ID を指定する必要があります。**Application** フォルダー内の **AuthenticationConstants.m** を開きます。登録プロセスから受け取った ClientID をファイルの最上部に追加できることがわかります。</span><span class="sxs-lookup"><span data-stu-id="ae477-p121">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

><span data-ttu-id="ae477-p122">注:次のアクセス許可の適用範囲がこのプロジェクトに対して構成されていることが分かります。: **"https://graph.microsoft.com/Mail.Send"、 "https://graph.microsoft.com/User.Read"、 "offline_access"**。このプロジェクトで使用されるサービス呼び出し、メール アカウントへのメールの送信、および一部のプロファイル情報 (表示名、メール アドレス) の取得では、アプリが適切に実行するためにこれらのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae477-p122">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="ae477-190">サンプルを実行し、**[Connect]**をタップして、個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="ae477-190">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="ae477-p123">**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ae477-p123">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae477-193">次の手順</span><span class="sxs-lookup"><span data-stu-id="ae477-193">Next steps</span></span>
- <span data-ttu-id="ae477-194">[Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="ae477-194">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="ae477-195">[Microsoft Graph iOS オブジェクティブ C スニペット サンプル](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample)に、REST 操作と SDK 操作の両方に共通する操作の例があります。</span><span class="sxs-lookup"><span data-stu-id="ae477-195">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="ae477-196">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae477-196">See also</span></span>
- [<span data-ttu-id="ae477-197">iOS 用 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="ae477-197">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="ae477-198">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="ae477-198">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="ae477-199">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="ae477-199">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
