# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="9dfcd-101">Swift iOS アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="9dfcd-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="9dfcd-p101">**エンタープライズのお客様向けにアプリを作成していますか?**エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="9dfcd-p102">**すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="9dfcd-p103">この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[iOS (SDK) 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-swift-connect-sample)内のコードを説明し、Microsoft Graph を使用するアプリで実装する必要のある主要な概念について説明します。[iOS 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios) を使用して Microsoft Graph にアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="9dfcd-110">作成するアプリのバージョンを、この GitHub リポジトリからダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="9dfcd-111">Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル</span><span class="sxs-lookup"><span data-stu-id="9dfcd-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="9dfcd-112">次の画像は、作成するアプリを示しています。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-112">The following image shows the app you'll create.</span></span>

![Connect のサンプル チュートリアル。アプリにおける接続とメールの送信を示します](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="9dfcd-114">ワークフローは、Microsoft Graph への接続/認証を行い、職場または個人用アカウントでサインインし、最後に受信者に向けてメールを送信する、というものです。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="9dfcd-p104">**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/ja-JP/getting-started)」を使用すれば、すばやく稼働させることができます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/ja-JP/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dfcd-117">前提条件</span><span class="sxs-lookup"><span data-stu-id="9dfcd-117">Prerequisites</span></span>

<span data-ttu-id="9dfcd-118">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="9dfcd-119">Apple 社の [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="9dfcd-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="9dfcd-120">依存関係マネージャーとしての [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) のインストール。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="9dfcd-121">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="9dfcd-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="9dfcd-122">[iOS 用 Microsoft Graph スターター プロジェクト](https://github.com/microsoftgraph/ios-objectivec-connect-sample)。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="9dfcd-123">このテンプレートには、コードを追加するクラスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="9dfcd-124">このプロジェクトを取得するには、この場所からサンプル プロジェクトを複製するかダウンロードして、**starter-project** フォルダー内のワークスペース (**ios-objectivec-connect-sample.xcworkspace**) で作業します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="9dfcd-125">アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="9dfcd-125">Register the app</span></span>
 
1. <span data-ttu-id="9dfcd-126">個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="9dfcd-127">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="9dfcd-128">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="9dfcd-129">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="9dfcd-130">**[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="9dfcd-131">**[ネイティブ プラットフォーム]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="9dfcd-p106">クライアント ID をクリップボードにコピーします。サンプル アプリにこの値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="9dfcd-134">アプリ ID は、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="9dfcd-135">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="9dfcd-136">プロジェクトの依存関係のインポート</span><span class="sxs-lookup"><span data-stu-id="9dfcd-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="9dfcd-137">このリポジトリ ([Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-objectivec-connect-sample)) を複製します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="9dfcd-138">重要: プロジェクトのルートにあるサンプルではなく、starter-project フォルダーのサンプルを使用してください。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="9dfcd-p107">CocoaPods を使用して、Microsoft Graph SDK と認証の依存関係をインポートします。このサンプル アプリには、プロジェクトに pod を取り込む podfile が既に含まれています。**ターミナル** アプリでフォルダー **starter-project** に移動し、**ターミナル**から以下を実行します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="9dfcd-p108">pod がプロジェクトにインポートされたことの確認が表示されます。詳細については、「[CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="9dfcd-144">キーチェーンの共有の有効化</span><span class="sxs-lookup"><span data-stu-id="9dfcd-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="9dfcd-p109">Xcode8 には、キーチェーンのグループを追加する必要があります。これを行わないと、アプリがキーチェーンにアクセスできなくなります。キーチェーン グループを追加するには:</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="9dfcd-p110">Xcode のプロジェクト マネージャーのパネルで、プロジェクトを選択します (⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="9dfcd-149">**iOS-ObjectiveC-Connect-Sample** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="9dfcd-150">[機能] タブで **[キーチェーンを共有]** を有効にします。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="9dfcd-151">**com.microsoft.ios-objectivec-connect-sample** をキーチェーン グループに追加します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="9dfcd-152">Microsoft Graph での認証</span><span class="sxs-lookup"><span data-stu-id="9dfcd-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="9dfcd-153">UI のワークフローを見直すため、アプリはユーザーに認証を実行させます。こうすると指定されたユーザーにメールを送信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-153">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user.</span></span> <span data-ttu-id="9dfcd-154">Microsoft Graph サービスに対して要求を行うには、適切な OAuth 2.0 ベアラー トークンを使用して HTTPS 要求を認証できる認証プロバイダーを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-154">To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="9dfcd-155">サンプル プロジェクトには、既にスタブ アウトされていた **Authentication.swift** という認証構造があります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-155">In the sample project there's an authentication structure already stubbed out called **Authentication.swift.**</span></span> <span data-ttu-id="9dfcd-156">Microsoft Graph API を呼び出すためのアクセス トークンを要求および取得する関数を追加します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-156">We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="9dfcd-157">Xcode プロジェクト ワークスペース (**Graph-iOS-Swift-Connect.xcworkspace**) を開き、構造の拡張ファイル **Authentication.swift** を開きます。その拡張で次のコードを検索します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-157">Open the Xcode project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the structure extension file **Authentication.swift** Find the following code in that extension.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph. 
     If a user has previously signed in before and not disconnected, silent log in
     will take place. 
     If not, authentication will ask for credentials
     */
    func connectToGraph(withClientId clientId: String,
                                     scopes: [String],
                                     completion:@escaping (_ error: MSGraphError?) -> Void) {
    
        // Set client ID
        NXOAuth2AuthenticationProvider.setClientId(clientId, scopes: scopes)
        
        // Try silent log in. This will attempt to sign in if there is a previous successful
        // sign in user information.
        if NXOAuth2AuthenticationProvider.sharedAuth().loginSilent() == true {
            completion(nil)
        }
        // Otherwise, present log in controller.
        else {
            NXOAuth2AuthenticationProvider.sharedAuth()
                .login(with: nil) { (error: Error?) in
                    
                    if let nserror = error {
                        completion(MSGraphError.nsErrorType(error: nserror as NSError))
                    }
                    else {
                        completion(nil)
                    }
            }
        }
    }
  ```


2. <span data-ttu-id="9dfcd-158">**ConnectViewController.swift** からこのメソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-158">We'll call this method from **ConnectViewController.swift**.</span></span> <span data-ttu-id="9dfcd-159">このコントローラーはアプリが読み込む既定のビューであり、**[Connect]** という 1 つのボタンをユーザーがタップすると認証プロセスが開始します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-159">This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process.</span></span> <span data-ttu-id="9dfcd-160">このメソッドは、**スコープ**という 1 つのパラメーターを使用します。以下で、スコープの詳細について説明します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-160">This method takes in one parameter, the **scopes**, we'll discuss scopes in more detail below.</span></span> <span data-ttu-id="9dfcd-161">次のアクションを **ConnectViewController.swift** に追加します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-161">Add the following action to **ConnectViewController.swift**.</span></span>

  ```swift
  // MARK: Authentication
  private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        
        let clientId = ApplicationConstants.clientId
        let scopes = ApplicationConstants.scopes
        
        authentication.connectToGraph(withClientId: clientId, scopes: scopes) {
            (error) in
            
            defer {self.loadingUI(show: false)}
            
            if let graphError = error {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
            }
            else {
                self.performSegue(withIdentifier: "showSendMail", sender: nil)
            }
        }
    }
  }

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="9dfcd-162">Microsoft Graph を使用してメールを送信する</span><span class="sxs-lookup"><span data-stu-id="9dfcd-162">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="9dfcd-163">認証できるようにプロジェクトを構成したら、次のタスクでは認証されたユーザーのメール アドレス、表示名、プロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-163">After configuring the project to be able to authenticate, the next tasks are getting the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="9dfcd-164">サンプルがこれらの値を取得した後、プロフィール写真を OneDrive にアップロードし、写真の共有 URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-164">After the sample gets these values it uploads the profile picture to OneDrive and gets the sharing Url of the picture.</span></span> <span data-ttu-id="9dfcd-165">最後に、Microsoft Graph API を使用してユーザーにメールを送信します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-165">Finally, it sends a mail to a user using the Microsoft Graph API.</span></span> 

<span data-ttu-id="9dfcd-166">既定では、ログインしているユーザーが受信者ですが、他の任意の受信者に変更することができます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-166">By default the logged in user will be the recipient, but you have the ability to change it to any other recipient.</span></span> <span data-ttu-id="9dfcd-167">ここで操作するコードは、**SendMailViewController.swift** クラスに属しています。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-167">The code we'll work with here is in the class **SendMailViewController.swift.**</span></span> <span data-ttu-id="9dfcd-168">UI を表す他のコードや、Microsoft Graph サービスからユーザー プロファイル情報を取得するヘルパー メソッドがあることがわかります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-168">You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service.</span></span> <span data-ttu-id="9dfcd-169">ここでは、メール メッセージの作成とそのメッセージの送信を行うメソッドに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-169">We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="9dfcd-170">**SendMailViewController.swift** を開きます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-170">Open **SendMailViewController.swift.**</span></span>  <span data-ttu-id="9dfcd-171">その後、クラスからヘルパー メソッドを作成するメールの本文を検索します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-171">and find the mail body creating helper method in the class:</span></span>

  ```swift
    /**
     Creates sample email message
     
     - parameter emailAddress: recipient email address
     
     - returns: MSGraphMessage object with given recipient. The body is created from EmailBody.html
     */
    func createSampleMessage(to emailAddress: String, picLink pictureUrl: String) -> MSGraphMessage? {
        let message = MSGraphMessage()
        
        // set recipients
        
        let _ = self.userPicture
        let toRecipient = MSGraphRecipient()
        let msEmailAddress = MSGraphEmailAddress()
        msEmailAddress.address = emailAddress
        toRecipient.emailAddress = msEmailAddress
        let toRecipientList = [toRecipient]
        message.toRecipients = toRecipientList
        message.subject = NSLocalizedString("MAIL_SUBJECT", comment: "")
        let messageBody = MSGraphItemBody()
        messageBody.contentType = MSGraphBodyType.html()
        guard let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html") else {return nil}
        messageBody.content = try! String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
        messageBody.content = messageBody.content.replacingOccurrences(of: "a href=%s", with: ("a href=" + pictureUrl))
        message.body = messageBody

        if let unwrappedImage = self.userPicture {
            let fileAttachment = MSGraphFileAttachment()
            let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
            fileAttachment.contentType = "image/png"
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment"
            fileAttachment.contentBytes = data?.base64EncodedString()
            fileAttachment.name = "me.png"
            message.attachments.append(fileAttachment)
        }
        return message
    }

  ```
2. <span data-ttu-id="9dfcd-172">ユーザー情報とプロフィール写真を取得し、OneDrive に写真をアップロードするには、次のヘルパー メソッドを検索します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-172">find the following helper methods for getting user information, getting a profile photograph, and uploading the photograph to OneDrive:</span></span>

  ```swift
      /**
     Fetches user information such as mail and display name
     */
    func getUserInfo() {
        self.sendButton.isEnabled = false
        self.statusTextView.text = NSLocalizedString("LOADING_USER_INFO", comment: "")
        
        self.graphClient.me().request().getWithCompletion {
            (user: MSGraphUser?, error: Error?) in
            if let graphError = error {
                print(NSLocalizedString("ERROR", comment: ""), graphError)
                DispatchQueue.main.async(execute: {
                    self.statusTextView.text = NSLocalizedString("GRAPH_ERROR", comment: "")
                })
            }
            else {
                guard let userInfo = user else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_FAILURE", comment: "")
                    })
                    return
                }
                DispatchQueue.main.async(execute: {
                    self.emailTextField.text = userInfo.mail
                    
                    if let displayName = userInfo.displayName {
                        self.headerLabel.text = "Hi " + displayName
                    }
                    else {
                        self.headerLabel.text = NSString(format: NSLocalizedString("HI_USER", comment: "") as NSString, "") as String
                    }
                    
                    self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_SUCCESS", comment: "")
                    self.sendButton.isEnabled = true
                })
            }
        }
    }
    
    /**
     Uploads the user's profile picture (obtained via the Graph API) to the user's OneDrive drive. The OneDrive sharing url is
     returned in the completion handler.
    */
    func uploadPictureToOneDrive(uploadFile image: UIImage?, with completion: @escaping (_ result: GraphResult<String, NSError>) ->Void) {
        
        var webUrl: String = ""
        guard let unwrappedImage = image else {
            return
        }
        let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
        self.graphClient
            .me()
            .drive()
            .root()
            .children()
            .driveItem("me.png")
            .contentRequest()
            .upload(from: data, completion: {
                (driveItem: MSGraphDriveItem?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("UPLOAD_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return

                } else {
                    webUrl = (driveItem?.webUrl)!
                    completion(.success(webUrl))
                }
            })
    }


    /**
     Gets the user's profile picture. Returns the picture as a UIImage via completion handler
    */
    func getUserPicture(forUser upn: String, with completion: @escaping (_ result: GraphResult<UIImage, NSError>) -> Void) {
        
        //Asynchronous Graph call. Closure is invoked after getUserPicture completes. Requires @escaping attribute
        self.graphClient.me().photoValue().download {
            (url: URL?, response: URLResponse?, error: Error?) in
            
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return
                }
                guard let picUrl = url else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "User profile picture is nil")
                    })
                    return
                }
                print(picUrl)
            
                let picData = NSData(contentsOf: picUrl)
                let picImage = UIImage(data: picData! as Data)
            
                if let validPic = picImage {
                    completion(.success(validPic))
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "Picture data is invalid")
                    })
                }
            }
    }

  ```

3. <span data-ttu-id="9dfcd-173">次のメール送信メソッドをクラスで検索します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-173">Find the following send mail method in the class.</span></span>  

  ```swift
    @IBAction func sendMail(_ sender: AnyObject) {
        guard let toEmail = self.emailTextField.text else {return}
        guard let picUrl = self.userPictureUrl else {return}
        if let message = self.createSampleMessage(to: toEmail, picLink: picUrl) {
            
            let requestBuilder = graphClient.me().sendMail(with: message, saveToSentItems: false)
            let mailRequest = requestBuilder?.request()
            
            _ = mailRequest?.execute(completion: {
                (response: [AnyHashable: Any]?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("SEND_FAILURE", comment: "")
                    })
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.descriptionLabel.text = "Check your inbox. You have a new message :)"
                        self.statusTextView.text = NSLocalizedString("SEND_SUCCESS", comment: "")
                    })
                }
            })
        }
    }

  ```


## <a name="run-the-app"></a><span data-ttu-id="9dfcd-174">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="9dfcd-174">Run the app</span></span>
1. <span data-ttu-id="9dfcd-175">サンプルを実行する前に、「**アプリの登録**」セクションの登録プロセスで受け取ったクライアント ID を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-175">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="9dfcd-176">**ApplicationConstants.swift** を開きます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-176">Open **ApplicationConstants.swift** .</span></span> <span data-ttu-id="9dfcd-177">登録プロセスで受け取った ClientID をファイルの最上部に追加できることがわかります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-177">You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  

  ```swift
struct ApplicationConstants {
    static let clientId = "Enter_Client_Id_Here"
    static let scopes   = ["openid", "profile", "Mail.ReadWrite","mail.send","Files.ReadWrite","User.ReadBasic.All"]
}


  ```

> <span data-ttu-id="9dfcd-p117">注:次のアクセス許可の適用範囲がこのプロジェクトに対して構成されていることが分かります。: **"https://graph.microsoft.com/Mail.Send"、 "https://graph.microsoft.com/User.Read"、 "offline_access"**。このプロジェクトで使用されるサービス呼び出し、メール アカウントへのメールの送信、および一部のプロファイル情報 (表示名、メール アドレス) の取得では、アプリが適切に実行するためにこれらのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p117">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="9dfcd-180">サンプルを実行し、**[Connect]**をタップして、個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-180">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="9dfcd-p118">**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-p118">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9dfcd-183">次の手順</span><span class="sxs-lookup"><span data-stu-id="9dfcd-183">Next steps</span></span>
- <span data-ttu-id="9dfcd-184">[Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-184">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="9dfcd-185">[Microsoft Graph iOS オブジェクティブ C スニペット サンプル](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample)に、REST 操作と SDK 操作の両方に共通する操作の例があります。</span><span class="sxs-lookup"><span data-stu-id="9dfcd-185">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="9dfcd-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="9dfcd-186">See also</span></span>
- [<span data-ttu-id="9dfcd-187">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="9dfcd-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="9dfcd-188">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="9dfcd-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/)
