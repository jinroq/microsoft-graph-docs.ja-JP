# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="56bd3-101">Swift iOS アプリで Microsoft Graph を使ってみる</span><span class="sxs-lookup"><span data-stu-id="56bd3-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="56bd3-p101">**エンタープライズのお客様向けにアプリを作成していますか?** エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="56bd3-p102">**すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="56bd3-p103">この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[iOS (REST) 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)内のコードを説明し、Microsoft Graph を使用するアプリで実装する主要な概念について説明します。非同期の **Promise チェーン** パターンで REST 操作を使用して Microsoft Graph にアクセスする方法を説明します。サンプル内の Promise は、[mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPods を使用して実装されています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the **Microsoft Graph SDK for iOS**.</span></span> 

<span data-ttu-id="56bd3-111">このサンプルは、**Xcode 9.2** と **Swift 3.2** を使用して作成されています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-111">The sample was created using **XCode 9.2** and **Swift 3.2**.</span></span>

<span data-ttu-id="56bd3-112">作成するアプリのバージョンを、この GitHub リポジトリからダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-112">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="56bd3-113">Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル</span><span class="sxs-lookup"><span data-stu-id="56bd3-113">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

<span data-ttu-id="56bd3-114">次の画像は、作成するアプリを示しています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-114">The following image shows the app you'll create.</span></span>

![Connect のサンプル チュートリアル。アプリにおける接続とメールの送信を示します](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="56bd3-116">ワークフローは、サンプルを認証および承認して Microsoft Graph リソースにアクセスし、職場または個人用のアカウントでサインインし、最後に受信者に向けてメールを送信する、というものです。</span><span class="sxs-lookup"><span data-stu-id="56bd3-116">The workflow authenticates and authorizes the sample to access  Microsoft Graph resources, signs in with your work or personal account, and finally sends a mail to a recipient.</span></span>

<span data-ttu-id="56bd3-p104">**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://developer.microsoft.com/ja-JP/graph/quick-start)」を使用すれば、すばやく稼働させることができます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/ja-JP/graph/quick-start) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56bd3-119">前提条件</span><span class="sxs-lookup"><span data-stu-id="56bd3-119">Prerequisites</span></span>

<span data-ttu-id="56bd3-120">開始するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="56bd3-120">To get started, you'll need:</span></span> 

* <span data-ttu-id="56bd3-121">Apple 社の [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="56bd3-121">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="56bd3-122">依存関係マネージャーとしての [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) のインストール。</span><span class="sxs-lookup"><span data-stu-id="56bd3-122">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="56bd3-123">**MSAL** ライブラリをインポートしてビルドするための [Carthage](https://github.com/Carthage/Carthage) のインストール。</span><span class="sxs-lookup"><span data-stu-id="56bd3-123">Installation of [Carthage](https://github.com/Carthage/Carthage) to import and build the **MSAL** library.</span></span>
* <span data-ttu-id="56bd3-124">[PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) CocoaPods のインストール。</span><span class="sxs-lookup"><span data-stu-id="56bd3-124">Installation of the [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod.</span></span> 
* <span data-ttu-id="56bd3-125">[Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="56bd3-125">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)</span></span>

## <a name="register-the-app"></a><span data-ttu-id="56bd3-126">アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="56bd3-126">Register the app</span></span>
 
1. <span data-ttu-id="56bd3-127">個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="56bd3-127">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="56bd3-128">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-128">Select **Add an app**.</span></span>
3. <span data-ttu-id="56bd3-129">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-129">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="56bd3-130">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-130">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="56bd3-131">**[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-131">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="56bd3-132">**[ネイティブ プラットフォーム]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-132">Select **Native platform**.</span></span>
6. <span data-ttu-id="56bd3-p105">クライアント ID をクリップボードにコピーします。サンプル アプリにこの値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p105">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="56bd3-135">アプリ ID は、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="56bd3-135">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="56bd3-136">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-136">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="56bd3-137">プロジェクトの依存関係のインポート</span><span class="sxs-lookup"><span data-stu-id="56bd3-137">Importing the project dependencies</span></span>

1. <span data-ttu-id="56bd3-138">このリポジトリ ([Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)) を複製します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-138">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span></span> 


2. <span data-ttu-id="56bd3-139">CocoaPods を使用して PromiseKit の依存関係をインポートします。</span><span class="sxs-lookup"><span data-stu-id="56bd3-139">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies:</span></span> <span data-ttu-id="56bd3-140">このサンプル アプリには、プロジェクトに pod を取り込む podfile が既に含まれています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-140">This sample app already contains a podfile that will get the pods into the project.</span></span> <span data-ttu-id="56bd3-141">**ターミナル** アプリでプロジェクトのルート フォルダーに移動し、**ターミナル**から以下を実行します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-141">Navigate to the root folder of the project in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="56bd3-p107">pod がプロジェクトにインポートされたことの確認が表示されます。詳細については、「[CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p107">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>

## <a name="install-the-msal-authentication-framework"></a><span data-ttu-id="56bd3-144">MSAL 認証フレームワークのインストール</span><span class="sxs-lookup"><span data-stu-id="56bd3-144">Install the MSAL authentication framework</span></span>

<span data-ttu-id="56bd3-145">MSAL のプレビュー バージョンは、Carthage を使用してヘッダー ファイルとシンボル ファイルとして配布されています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-145">The preview version of MSAL is distributed as header and symbol files using Carthage.</span></span> <span data-ttu-id="56bd3-146">プロジェクトに MSAL をインストールするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-146">To install MSAL in the project, do these steps:</span></span>

1. <span data-ttu-id="56bd3-147">Bash ターミナルを開き、アプリのルート フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-147">Open the Bash terminal and go to the app root folder.</span></span>
2. <span data-ttu-id="56bd3-148">**cartfile** を作成します。`echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` をターミナルにコピーして、このコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-148">Create a **cartfile**: Copy `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile`  into the terminal and run the command.</span></span>
3. <span data-ttu-id="56bd3-149">MSAL ライブラリを構築します。`carthage update` をターミナルにコピーして、このコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-149">Build the MSAL library: Copy `carthage update` into the terminal and run the command.</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="56bd3-150">キーチェーンの共有の有効化</span><span class="sxs-lookup"><span data-stu-id="56bd3-150">Enable keychain sharing</span></span>
 
<span data-ttu-id="56bd3-p109">Xcode8 には、キーチェーンのグループを追加する必要があります。これを行わないと、アプリがキーチェーンにアクセスできなくなります。キーチェーン グループを追加するには:</span><span class="sxs-lookup"><span data-stu-id="56bd3-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="56bd3-153">Xcode のプロジェクト マネージャーのパネルで、プロジェクトを選択します </span><span class="sxs-lookup"><span data-stu-id="56bd3-153">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span> <span data-ttu-id="56bd3-154">(⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="56bd3-154">(⌘ + 1).</span></span>
 
2. <span data-ttu-id="56bd3-155">**O365-iOS-Microsoft-Graph-Connect-swift** ターゲットを選択します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-155">Select the **O365-iOS-Microsoft-Graph-Connect-swift** target.</span></span>

3. <span data-ttu-id="56bd3-156">**[General]** タブの **[Signing]** セクションで、**[Automatically manage signing]** がオンになっており、有効な署名証明書があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-156">On the **General** tab and **Signing** section, verify that **Automatically manage signing** is checked and you have a valid signing certificate.</span></span>
 
3. <span data-ttu-id="56bd3-157">**[Capabilities]** タブで、**[Keychain Sharing]** を有効にします。</span><span class="sxs-lookup"><span data-stu-id="56bd3-157">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="56bd3-158">**com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** がキーチェーン グループのリストに含まれていない場合は、これを追加します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-158">If **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** is not in the list of Keychain Groups, add it.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="56bd3-159">Microsoft Graph での認証</span><span class="sxs-lookup"><span data-stu-id="56bd3-159">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="56bd3-160">UI のワークフローは次のようになっています。まず、アプリがユーザーに認証を要求します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-160">The UI workflow is as follows: The app asks the user to authenticate.</span></span> <span data-ttu-id="56bd3-161">認証後、ユーザーは他のユーザーにメールを送信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="56bd3-161">After authentication, the user can send a mail to another user.</span></span> <span data-ttu-id="56bd3-162">Microsoft Graph に対して要求を行うため、このサンプルは **MSAL** 認証ライブラリを使用して、適切な OAuth 2.0 ベアラー トークンによって HTTPS 要求を認証します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-162">To make requests against Microsoft Graph, the sample uses the **MSAL** authentication library to authenticate HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="56bd3-163">サンプル プロジェクトでは、**AuthenticationClass.swift** </span><span class="sxs-lookup"><span data-stu-id="56bd3-163">In the sample project the **AuthenticationClass.swift.**</span></span> <span data-ttu-id="56bd3-164">クラスが **MSAL** ライブラリをインポートし、Microsoft Graph の REST 操作に必要なアクセス トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-164">class imports the **MSAL** library and acquires the access token needed for Microsoft Graph REST operations.</span></span>

1. <span data-ttu-id="56bd3-165">**Xcode** プロジェクト ワークスペース (**Graph-iOS-Swift-Connect.xcworkspace**) を開き、クラス ファイル **AuthenticationClass.swift** を開きます。そのクラスで次のコードを検索します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-165">Open the Xcode project workspace (Graph-iOS-Swift-Connect.xcworkspace), and open the structure extension file Authentication.swift Find the following code in that extension.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph.
     If a user has previously signed in before and not disconnected, silent log in
     will take place.
     If not, authentication will ask for credentials
     */
    func connectToGraph(scopes: [String],
                        completion:@escaping (_ error: ApplicationConstants.MSGraphError?, _ accessToken: String) -> Bool)  {
        do {
            if let initError = self.lastInitError {
                if initError.lengthOfBytes(using: String.Encoding.ascii) > 1 {
                    throw NSError.init(domain: initError, code: 0, userInfo: nil)
                }
            }
            // We check to see if we have a current logged in user. If we don't, then we need to sign someone in.
            // We throw an interactionRequired so that we trigger the interactive signin.
            if  try authenticationProvider.users().isEmpty {
                throw NSError.init(domain: "MSALErrorDomain", code: MSALErrorCode.interactionRequired.rawValue, userInfo: nil)
            } else {
                // Acquire a token for an existing user silently
                try authenticationProvider.acquireTokenSilent(forScopes: scopes, user: authenticationProvider.users().first) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        _ = completion(nil, self.accessToken);
                    } else {
                        //"Could not acquire token silently: \(error ?? "No error information" as! Error )"
                       var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            }
        }  catch let error as NSError {
            // interactionRequired means we need to ask the user to sign-in. This usually happens
            // when the user's Refresh Token is expired or if the user has changed their password
            // among other possible reasons.
            if error.code == MSALErrorCode.interactionRequired.rawValue {
                authenticationProvider.acquireToken(forScopes: scopes) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        var _ = completion(nil, self.accessToken);
                    } else  {
                        var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            } else {
                var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);

            }
        } catch {
            // This is the catch all error.
            var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);
        }
    }

  ```


2. <span data-ttu-id="56bd3-166">**ConnectViewController.swift** から **connectToGraph** 関数を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-166">We'll call the **connectToGraph** function from **ConnectViewController.swift**.</span></span> <span data-ttu-id="56bd3-167">このコントローラーはアプリが読み込む既定のビューであり、ユーザーがタップすると認証が開始される **[Connect]** というボタン 1 つを含んでいます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-167">This controller is the default view that the app loads with a single button named **Connect** that the user taps to start authenticating.</span></span> 

  ```swift
// MARK: Authentication
private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        let scopes = ApplicationConstants.kScopes
        AuthenticationClass.sharedInstance?.connectToGraph( scopes: scopes) {
            (result: ApplicationConstants.MSGraphError?, accessToken: String) -> Bool  in
            defer {self.loadingUI(show: false)}
            if let graphError = result {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.userInfo)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
                return false
            }
            else {
                // run on main thread!!
                DispatchQueue.main.async {
                    self.performSegue(withIdentifier: "sendMail", sender: nil)
                }
                return true
            }
        }
    }
}

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="56bd3-168">Microsoft Graph を使用してメールを送信する</span><span class="sxs-lookup"><span data-stu-id="56bd3-168">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="56bd3-169">ユーザーを Microsoft Graph に接続した後、このサンプルは認証されたユーザーのメール アドレス、表示名、およびプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-169">After connecting the user to Microsoft Graph, the sample gets the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="56bd3-170">次に、ユーザーの OneDrive のルート フォルダーにプロフィール写真をアップロードし、OneDrive に写真の共有 URL を要求します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-170">The sample uploads the profile photo to the user's OneDrive root folder and asks OneDrive for the sharing Url of the picture.</span></span> <span data-ttu-id="56bd3-171">最後に、取得したメール アドレスにメール メッセージを送信する REST 要求を Microsoft Graph に送信します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-171">Finally, the sample posts a REST request to Microsoft Graph to send a mail message to the provided email address.</span></span> 

<span data-ttu-id="56bd3-172">メッセージの本文には、写真の共有リンクと、写真自体が添付された画像ファイルとして含まれています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-172">The message body contains the picture sharing link and the picture itself as an attached image file.</span></span> <span data-ttu-id="56bd3-173">既定の受信者は認証されたユーザーですが、サンプルではこのユーザーが他のユーザーのメール アドレスを入力できるようになっています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-173">The default recipient is the authenticated user, but the sample allows the user to provide the email address of any other user.</span></span> 

<span data-ttu-id="56bd3-174">ここで操作するコードは、**SendMailViewController_WithPromise.swift** クラスに属しています。</span><span class="sxs-lookup"><span data-stu-id="56bd3-174">The code we'll work with here is in the class **SendMailViewController.swift.**</span></span> <span data-ttu-id="56bd3-175">`viewDidLoad()` 関数は `self.emailTextField.text` の値を読み取ってメール受信者のメール アドレスを取得し、**Promise チェーン**を開始して認証されたユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-175">The `viewDidLoad()` function reads the `self.emailTextField.text` value to get the mail recipient's email address and then starts a **promise chain** to get the authenticated user's profile picture.</span></span> <span data-ttu-id="56bd3-176">PromisePromise が拒否される場合は、`sendMailButton` が有効になっていません。</span><span class="sxs-lookup"><span data-stu-id="56bd3-176">If the promise is rejected, the `sendMailButton` is not enabled.</span></span>

1. <span data-ttu-id="56bd3-177">**SendMailViewController_WithPromise.swift** を開き、</span><span class="sxs-lookup"><span data-stu-id="56bd3-177">Open **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="56bd3-178">`viewDidLoad` 関数を見つけます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-178">and find the `viewDidLoad` function.</span></span> <span data-ttu-id="56bd3-179">`self.userPictureWork` 関数は Promise チェーンを開始するために呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-179">The `self.userPictureWork` function is called to start the promise chain.</span></span>

   ```swift
    override func viewDidLoad() {
        super.viewDidLoad()
        //Get user state values before creating mail message to be sent
        do
        {
            try self.userName = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].name!
            try self.emailTextField.text = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].displayableId
            self.userEmailAddress = self.emailTextField.text
            self.headerLabel.text = "Hi, \(self.userName! )"
            
            updateUI(showActivityIndicator: true, statusText: "Getting picture", sendMail: true)

            //Important: Break out of async promise chain by declaring result returns Void
            _ = self.userPictureWork().then{
                result -> Void in
                    self.userPictureUrl = (result[1] as! String)
                    self.userProfilePicture = (result[0] as! UIImage)
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)

            }.catch{err -> Void  in
                self.updateUI(showActivityIndicator: false, statusText: "", sendMail: false)

            }
        } catch _ as NSError{
            self.updateUI(showActivityIndicator: false,
                          statusText: "Error getting user profile picture.", sendMail: false)
        }
    }
  
   ```

   

1. <span data-ttu-id="56bd3-180">クラス内にあるメール要求作成のヘルパー関数を見つけます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-180">Find the mail request creation helper function in the class:</span></span>

   ```swift
    /**
     Prepare mail content by loading the JSON request payload template and HTML message body template from resources and replacing placeholders in the templates with appropriate values.
     */
    func mailContent() -> Data? {
        if let emailFilePath = Bundle.main.path(forResource: "EmailPostContent", ofType: "json"),
            let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html")
        {
            do {
                // Prepare upload content
                let emailContent = try String(contentsOfFile: emailFilePath, encoding: String.Encoding.utf8)
                let emailBodyRaw = try String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
                // Request doesn't accept a single quotation mark("), so change it to the acceptable form (\")
                var emailValidBody: String;
                emailValidBody = emailBodyRaw.replacingOccurrences(of: "\"", with: "\\\"")
                emailValidBody = emailValidBody.replacingOccurrences(of: "a href=%s", with: ("a href=" + self.userPictureUrl!))
                let imageData: NSData = UIImagePNGRepresentation(self.userProfilePicture!)! as NSData;
                let emailPostContent = emailContent.replacingOccurrences(of: "<EMAIL>", with: self.emailTextField.text!)
                    .replacingOccurrences(of: "<CONTENTTYPE>", with: "HTML")
                    .replacingOccurrences(of: "<CONTENT>", with: emailValidBody)
                    .replacingOccurrences(of: "<ODATA.TYPE>", with: "#microsoft.graph.fileAttachment")
                    .replacingOccurrences(of: "<IMAGE.TYPE>", with: "image\\/png")
                    .replacingOccurrences(of: "<CONTENTBYTES>", with: imageData.base64EncodedString())
                    .replacingOccurrences(of: "<NAME>", with: "me.png")
                // Return JSON payload with mail body as HTML string and attached picture as a file attachment of type NSData
                return emailPostContent.data(using: String.Encoding.utf8)
            }
            catch {
                // Error handling in case file loading fails.
                return nil
            }
        }
        // Error handling in case files aren't present.
        return nil
    }

   ```
2. <span data-ttu-id="56bd3-181">ユーザーのプロフィール写真を取得し、その写真を OneDrive にアップロードして、写真の共有リンクを要求する次のヘルパー関数を見つけます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-181">Find the following helper functions for getting the user's profile picture,  uploading the photograph to OneDrive, and requesting a sharing link for the picture:</span></span>

   ```swift
    /**
      Async func. Get user's profile photo, upload photo to OneDrive, and get sharing link
     - returns:
        Promise<UIImage>. The user's profile picture
     */
    func getUserPicture()->Promise<UIImage?>{
        return Promise{ fulfill, reject in
            let urlRequest = self.buildRequest(operation: "GET", resource: "photo/$value") as URLRequest
            let task = URLSession.shared.dataTask(with:urlRequest){ data , res , err in
                if let err:Error = err {
                    print(err.localizedDescription)
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return fulfill(self.getDefaultPicture())
                }
                if let data = data {
                    if let userImage: UIImage = UIImage(data:data) {
                        self.userProfilePicture = userImage
                        return fulfill(userImage)
                    } else {
                        return reject("no image" as! Error)
                    }
                } else {
                    return fulfill(self.getDefaultPicture())
                }
            }
            task.resume()
        }
    }
    
    /**
     Async func. Uploads a UIImage object to the signed in user's OneDrive root folder
     - Returns:
        A Promise encapsulating an array of AnyObject. Element 0 contains the user profile photo obtained in the previous chained async call
        Element 1 contains the web sharing URL of the photo in OneDrive as a String
     - Parameters:
     - UIImage: The image to upload to OneDrive
     */
    func uploadPicture(photo: UIImage) -> Promise<[AnyObject]> {
        return Promise<[AnyObject]>{ fulfill, reject in
            let uploadRequestUrl = self.buildRequest(operation: "PUT", resource: "drive/root:/me.jpg:/content", content: UIImageJPEGRepresentation(photo, 1.0)!) as URLRequest
            let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                if let err = err{
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return reject(HTTPError.InvalidRequest)
                }
                //data can be serialized to a DriveItem object
                //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                var itemId: String = "";
                if let responseContent = data {
                    itemId = self.getValueFromResponse(json: responseContent, key: "id" )
                    var returnValues = [AnyObject]();
                    returnValues.append(photo as AnyObject)
                    returnValues.append(itemId as AnyObject)
                    return fulfill(returnValues)
                }
            }
            task.resume()
        }
    }

    /**
     Async func. Requests a new sharing link for the OneDrive item specified by the item id.
     - returns:
     - Promise<String: AnyObject>. The new sharing link and the image wrapped in a Promise
     */
    func createSharingLink(itemId: String, image: UIImage) ->Promise<[AnyObject]>{
        return Promise<[AnyObject]>{ fulfill, reject in
            //Create Data object for the JSON payload
            if let sharingLinkFilePath = Bundle.main.path(forResource: "CreateSharingLink", ofType: "json")
            {
                do {
                    let sharingLinkcontent = try String(contentsOfFile: sharingLinkFilePath, encoding: String.Encoding.utf8)
                    let jsonPayload: Data = sharingLinkcontent.data(using: String.Encoding.utf8)!
                    let uploadRequestUrl = self.buildRequest(
                        operation: "POST", resource: "drive/items/"+itemId+"/createLink", content: jsonPayload) as URLRequest
                    let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                        if let err = err{
                            return reject(err)
                        }
                        if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                            return reject(HTTPError.InvalidRequest)
                        }
                        //data can be serialized to a DriveItem object
                        //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                        var sharingLink: String = "";
                        if let responseContent = data {
                            do {
                                let resultJson = try JSONSerialization.jsonObject(
                                    with: responseContent, options: []) as? [String:AnyObject]
                                sharingLink = (OneDriveFileLink.init(json:resultJson!)?.webUrl)!

                            } catch let error as NSError {
                                print(error)
                            }
                            var returnValues = [AnyObject]();
                            returnValues.append(image as AnyObject)
                            returnValues.append(sharingLink as AnyObject)
                            return fulfill(returnValues)
                        }
                    }
                    task.resume()

                }
            }
        }
   ```

3. <span data-ttu-id="56bd3-182">クラス内にある次のメール送信関数を見つけます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-182">Find the following send mail method in the class.</span></span>  
 
   ```swift
    /**
     POSTS a new message to the sendmail resource
     - parameters:
        - Data: The body of the message
     */
    func sendMailRESTWithContent(_ content: Data) {
        let _ = self.sendCRUDMessage(resource: "microsoft.graph.sendmail",
                                     operation: "POST",
                                     content: content)
    }
    
    /**
     Send a create, read, update, delete (CRUD) message.
     Create= POST, Update= PUT, Delete= DELETE.
     Read= GET. Use sendGETMessage(resource: String) to read Graph contents
     - returns:
     JSON response as Data
     - parameters:
        - String: The REST resource receiving the CRUD request
        - String: the REST operation requested
        - Data: The json (as Data) representing the values to update
     */
    func sendCRUDMessage(resource: String, operation:String, content: Data)->Data  {
        var returnData: Data;
        returnData = Data.init();
        if  (self.connectToGraph()){
            if (operation == "GET") {
                return self.sendGETMessage(resource: resource)
            }
            let request = self.buildRequest(operation: operation, resource: resource, content:content);
            let task = URLSession.shared.dataTask(with:request as URLRequest, completionHandler:{ data, res, err in
                if let err = err{
                    self.updateUI(showActivityIndicator: false,
                             statusText: "Error assembling the mail content." + err.localizedDescription, sendMail: false)
                }
                let nttpError = self.checkResult(result: res!)
                if (nttpError != HTTPError.NoError) {
                    self.updateUI(showActivityIndicator: false,
                                  statusText: "Error sending the mail.", sendMail: false)
                }
                else {
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)
                }
            }) // let task
             task.resume()
        }
        return returnData;
    }

   ```


## <a name="run-the-app"></a><span data-ttu-id="56bd3-183">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="56bd3-183">Run the app</span></span>
1. <span data-ttu-id="56bd3-184">サンプルを実行する前に、「**アプリの登録**」セクションの登録プロセスで受け取ったクライアント ID を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="56bd3-184">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="56bd3-185">ソース コードとして **Info.plist** を開きます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-185">Open **Info.plist** as source code.</span></span> 

   - <span data-ttu-id="56bd3-186">`ENTER_CLIENT_ID_HERE` を、登録プロセスで受け取った **ClientID** に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-186">Replace  `ENTER_CLIENT_ID_HERE` with the **ClientID** from the registration process.</span></span> <span data-ttu-id="56bd3-187">`msal` を置き換えないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="56bd3-187">Be sure that `msal` is not replaced.</span></span> <span data-ttu-id="56bd3-188">文字列を置換した後、配列の文字列値は `msal48d31887-5fad-4d73-a9f5-3c356e68a038` のようになります。GUID の部分は**ユーザーの**クライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="56bd3-188">After you replace the string, the array string value looks like `msal48d31887-5fad-4d73-a9f5-3c356e68a038` where the GUID portion is **your** client Id:</span></span>  

   <span data-ttu-id="56bd3-189">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-189">For example,</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msalENTER_CLIENT_ID_HERE</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

     <span data-ttu-id="56bd3-190">これは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="56bd3-190">becomes...</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msal48d31887-5fad-4d73-a9f5-3c356e68a038</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

> <span data-ttu-id="56bd3-191">**注:** このプロジェクトに対して次のアクセス許可の適用範囲が構成されていることがわかります。`["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]`</span><span class="sxs-lookup"><span data-stu-id="56bd3-191">Note: You'll notice that the following permission scopes have been configured for this project: "https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"`["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]`.</span></span> <span data-ttu-id="56bd3-192">このプロジェクトで使用されるサービス呼び出し、メール アカウントへのメールの送信、および一部のプロファイル情報 (表示名、メール アドレス) の取得、およびユーザーの OneDrive ルートへの書き込みでは、アプリがアクセス許可エラーなしで動作するためにこれらのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="56bd3-192">The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="56bd3-193">サンプルを実行し、**[Connect]** をタップして、個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。</span><span class="sxs-lookup"><span data-stu-id="56bd3-193">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="56bd3-p120">**[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-p120">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="56bd3-196">次の手順</span><span class="sxs-lookup"><span data-stu-id="56bd3-196">Next steps</span></span>
- <span data-ttu-id="56bd3-197">[Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="56bd3-197">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="56bd3-198">[Microsoft Graph iOS Objective C スニペット サンプル](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample)に、SDK 操作の一般的な操作の例があります。</span><span class="sxs-lookup"><span data-stu-id="56bd3-198">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="56bd3-199">関連項目</span><span class="sxs-lookup"><span data-stu-id="56bd3-199">See also</span></span>
- [<span data-ttu-id="56bd3-200">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="56bd3-200">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="56bd3-201">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="56bd3-201">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/)
