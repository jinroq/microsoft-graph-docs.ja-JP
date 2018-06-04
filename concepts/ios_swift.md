# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a>Swift iOS アプリで Microsoft Graph を使ってみる

> **エンタープライズのお客様向けにアプリを作成していますか?** エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。 

> **すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。

この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[iOS (REST) 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)内のコードを説明し、Microsoft Graph を使用するアプリで実装する主要な概念について説明します。非同期の **Promise チェーン** パターンで REST 操作を使用して Microsoft Graph にアクセスする方法を説明します。サンプル内の Promise は、[mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPods を使用して実装されています。 

このサンプルは、**Xcode 9.2** と **Swift 3.2** を使用して作成されています。

作成するアプリのバージョンを、この GitHub リポジトリからダウンロードすることができます。

* [Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

次の画像は、作成するアプリを示しています。

![Connect のサンプル チュートリアル。アプリにおける接続とメールの送信を示します](./images/iOSConnectWalkthrough.png)


ワークフローは、サンプルを認証および承認して Microsoft Graph リソースにアクセスし、職場または個人用のアカウントでサインインし、最後に受信者に向けてメールを送信する、というものです。

**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://developer.microsoft.com/ja-JP/graph/quick-start)」を使用すれば、すばやく稼働させることができます。

## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

* Apple 社の [Xcode](https://developer.apple.com/xcode/downloads/)
* 依存関係マネージャーとしての [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) のインストール。
* **MSAL** ライブラリをインポートしてビルドするための [Carthage](https://github.com/Carthage/Carthage) のインストール。
* [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) CocoaPods のインストール。 
* [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program-faq#account-types)

## <a name="register-the-app"></a>アプリを登録する
 
1. 個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。
2. **[アプリの追加]** を選択します。
3. アプリの名前を入力して、**[アプリケーションの作成]** を選択します。
    
    登録ページが表示され、アプリのプロパティが一覧表示されます。
 
4. **[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。
5. **[ネイティブ プラットフォーム]** を選択します。
6. クライアント ID をクリップボードにコピーします。サンプル アプリにこの値を入力する必要があります。

    アプリ ID は、アプリの一意識別子です。 

7. **[保存]** を選びます。

## <a name="importing-the-project-dependencies"></a>プロジェクトの依存関係のインポート

1. このリポジトリ ([Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)) を複製します。 


2. CocoaPods を使用して PromiseKit の依存関係をインポートします。 このサンプル アプリには、プロジェクトに pod を取り込む podfile が既に含まれています。 **ターミナル** アプリでプロジェクトのルート フォルダーに移動し、**ターミナル**から以下を実行します。

        pod install

   pod がプロジェクトにインポートされたことの確認が表示されます。詳細については、「[CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)」をご覧ください。

## <a name="install-the-msal-authentication-framework"></a>MSAL 認証フレームワークのインストール

MSAL のプレビュー バージョンは、Carthage を使用してヘッダー ファイルとシンボル ファイルとして配布されています。 プロジェクトに MSAL をインストールするには、次の手順を実行します。

1. Bash ターミナルを開き、アプリのルート フォルダーに移動します。
2. **cartfile** を作成します。`echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` をターミナルにコピーして、このコマンドを実行します。
3. MSAL ライブラリを構築します。`carthage update` をターミナルにコピーして、このコマンドを実行します。


## <a name="enable-keychain-sharing"></a>キーチェーンの共有の有効化
 
Xcode8 には、キーチェーンのグループを追加する必要があります。これを行わないと、アプリがキーチェーンにアクセスできなくなります。キーチェーン グループを追加するには:
 
1. Xcode のプロジェクト マネージャーのパネルで、プロジェクトを選択します  (⌘ + 1)。
 
2. **O365-iOS-Microsoft-Graph-Connect-swift** ターゲットを選択します。

3. **[General]** タブの **[Signing]** セクションで、**[Automatically manage signing]** がオンになっており、有効な署名証明書があることを確認します。
 
3. **[Capabilities]** タブで、**[Keychain Sharing]** を有効にします。
 
4. **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** がキーチェーン グループのリストに含まれていない場合は、これを追加します。

## <a name="authenticating-with-microsoft-graph"></a>Microsoft Graph での認証

UI のワークフローは次のようになっています。まず、アプリがユーザーに認証を要求します。 認証後、ユーザーは他のユーザーにメールを送信できるようになります。 Microsoft Graph に対して要求を行うため、このサンプルは **MSAL** 認証ライブラリを使用して、適切な OAuth 2.0 ベアラー トークンによって HTTPS 要求を認証します。 サンプル プロジェクトでは、**AuthenticationClass.swift**  クラスが **MSAL** ライブラリをインポートし、Microsoft Graph の REST 操作に必要なアクセス トークンを取得します。

1. **Xcode** プロジェクト ワークスペース (**Graph-iOS-Swift-Connect.xcworkspace**) を開き、クラス ファイル **AuthenticationClass.swift** を開きます。そのクラスで次のコードを検索します。


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


2. **ConnectViewController.swift** から **connectToGraph** 関数を呼び出します。 このコントローラーはアプリが読み込む既定のビューであり、ユーザーがタップすると認証が開始される **[Connect]** というボタン 1 つを含んでいます。 

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

## <a name="send-an-email-with-microsoft-graph"></a>Microsoft Graph を使用してメールを送信する

ユーザーを Microsoft Graph に接続した後、このサンプルは認証されたユーザーのメール アドレス、表示名、およびプロフィール写真を取得します。 次に、ユーザーの OneDrive のルート フォルダーにプロフィール写真をアップロードし、OneDrive に写真の共有 URL を要求します。 最後に、取得したメール アドレスにメール メッセージを送信する REST 要求を Microsoft Graph に送信します。 

メッセージの本文には、写真の共有リンクと、写真自体が添付された画像ファイルとして含まれています。 既定の受信者は認証されたユーザーですが、サンプルではこのユーザーが他のユーザーのメール アドレスを入力できるようになっています。 

ここで操作するコードは、**SendMailViewController_WithPromise.swift** クラスに属しています。 `viewDidLoad()` 関数は `self.emailTextField.text` の値を読み取ってメール受信者のメール アドレスを取得し、**Promise チェーン**を開始して認証されたユーザーのプロフィール写真を取得します。 PromisePromise が拒否される場合は、`sendMailButton` が有効になっていません。

1. **SendMailViewController_WithPromise.swift** を開き、 `viewDidLoad` 関数を見つけます。 `self.userPictureWork` 関数は Promise チェーンを開始するために呼び出されます。

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

   

1. クラス内にあるメール要求作成のヘルパー関数を見つけます。

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
2. ユーザーのプロフィール写真を取得し、その写真を OneDrive にアップロードして、写真の共有リンクを要求する次のヘルパー関数を見つけます。

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

3. クラス内にある次のメール送信関数を見つけます。  
 
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


## <a name="run-the-app"></a>アプリの実行
1. サンプルを実行する前に、「**アプリの登録**」セクションの登録プロセスで受け取ったクライアント ID を指定する必要があります。 ソース コードとして **Info.plist** を開きます。 

   - `ENTER_CLIENT_ID_HERE` を、登録プロセスで受け取った **ClientID** に置き換えます。 `msal` を置き換えないようにしてください。 文字列を置換した後、配列の文字列値は `msal48d31887-5fad-4d73-a9f5-3c356e68a038` のようになります。GUID の部分は**ユーザーの**クライアント ID です。  

   次に例を示します。 

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

     これは次のようになります。 

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

> **注:** このプロジェクトに対して次のアクセス許可の適用範囲が構成されていることがわかります。`["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` このプロジェクトで使用されるサービス呼び出し、メール アカウントへのメールの送信、および一部のプロファイル情報 (表示名、メール アドレス) の取得、およびユーザーの OneDrive ルートへの書き込みでは、アプリがアクセス許可エラーなしで動作するためにこれらのアクセス許可が必要です。

2. サンプルを実行し、**[Connect]** をタップして、個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。

3. **[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。

## <a name="next-steps"></a>次の手順
- [Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。
- [Microsoft Graph iOS Objective C スニペット サンプル](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample)に、SDK 操作の一般的な操作の例があります。

## <a name="see-also"></a>関連項目
- [Azure AD v2.0 のプロトコル](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 のトークン](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/)
