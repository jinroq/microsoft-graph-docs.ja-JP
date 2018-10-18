# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a>Objectve C iOS アプリで Microsoft Graph を使ってみる

> **エンタープライズのお客様向けにアプリを作成していますか?** エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。 

> **すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。

この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[iOS (SDK) 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-objectivec-connect-sample)内のコードを説明し、Microsoft Graph を使用するアプリで実装する必要のある主要な概念について説明します。[iOS 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios) を使用して Microsoft Graph にアクセスする方法を説明します。

作成するアプリのバージョンを、この GitHub リポジトリからダウンロードすることができます。

* [Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

次の画像は、作成するアプリを示しています。

![Connect のサンプル チュートリアル。アプリにおける接続とメールの送信を示します](./images/iOSConnectWalkthrough.png)


ワークフローは、Microsoft Graph への接続/認証を行い、職場または個人用アカウントでサインインし、最後に受信者に向けてメールを送信する、というものです。

**アプリを作成してみたくありませんか。**「[Microsoft Graph クイック スタート](https://graph.microsoft.io/en-us/getting-started)」を使用すれば、すばやく稼働させることができます。

## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

* Apple 社の [Xcode](https://developer.apple.com/xcode/downloads/)
* 依存関係マネージャーとしての [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) のインストール。
* [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)
* [iOS 用 Microsoft Graph スターター プロジェクト](https://github.com/microsoftgraph/ios-objectivec-connect-sample)。 このテンプレートには、コードを追加するクラスが含まれています。 このプロジェクトを取得するには、この場所からサンプル プロジェクトを複製するかダウンロードして、**starter-project** フォルダー内のワークスペース (**ios-objectivec-connect-sample.xcworkspace**) で作業します。

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

1. このリポジトリ ([Microsoft Graph SDK を使用した iOS 用 Office 365 Connect サンプル](https://github.com/microsoftgraph/ios-objectivec-connect-sample)) を複製します。 
>重要: プロジェクトのルートにあるサンプルではなく、starter-project フォルダーのサンプルを使用してください。

2. CocoaPods を使用して、Microsoft Graph SDK と認証の依存関係をインポートします。このサンプル アプリには、プロジェクトに pod を取り込む podfile が既に含まれています。**ターミナル** アプリでフォルダー **starter-project** に移動し、**ターミナル**から以下を実行します。

        pod install

   pod がプロジェクトにインポートされたことの確認が表示されます。詳細については、「[CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)」をご覧ください。


## <a name="enable-keychain-sharing"></a>キーチェーンの共有の有効化
 
Xcode8 には、キーチェーンのグループを追加する必要があります。これを行わないと、アプリがキーチェーンにアクセスできなくなります。キーチェーン グループを追加するには:
 
1. Xcode のプロジェクト マネージャーのパネルで、プロジェクトを選択します (⌘ + 1)。
 
2. **iOS-ObjectiveC-Connect-Sample** を選択します。
 
3. [機能] タブで **[キーチェーンを共有]** を有効にします。
 
4. **com.microsoft.ios-objectivec-connect-sample** をキーチェーン グループに追加します。
 

## <a name="authenticating-with-microsoft-graph"></a>Microsoft Graph での認証

UI のワークフローを見直すため、アプリはユーザーに認証を実行させます。こうすると指定されたユーザーにメールを送信できるようになります。Microsoft Graph サービスに対して要求を実行するには、適切な OAuth 2.0 ベアラー トークンを使用して HTTPS 要求を認証できる認証プロバイダーを指定する必要があります。サンプル プロジェクトには、既にスタブ アウトされていた **AuthenticationProvider.m** という認証クラスがあります。Microsoft Graph API を呼び出すためのアクセス トークンを要求および取得する関数を追加します。 

1. **starter-project** フォルダー内の Xcode プロジェクト ワークスペース (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) を開き、**Authentication** フォルダーに移動して、ファイルの **AuthenticationProvider.m.** を開きます。 そのクラスに次のコードを追加します。

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

2. 次にヘッダー ファイルにメソッドを追加します。ファイル **AuthenticationProvider.h** を開き、このクラスに次のコードを追加します。
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. 最後に、**ConnectViewController.m** からこのメソッドを呼び出します。このコントローラーはアプリが読み込む既定のビューであり、**[Connect]** という 1 つのボタンがあり、ユーザーがこれをタップすると認証プロセスが開始します。このメソッドには **Client ID** と **scopes** という 2 つのパラメーターを指定します。これらについては以下の部分で詳しく説明します。次の処理を **ConnectViewController.m** に追加します。

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

## <a name="send-an-email-with-microsoft-graph"></a>Microsoft Graph を使用して電子メールを送信する

認証できるようにプロジェクトを構成したら、次のタスクは、Microsoft Graph API を使用してユーザーにメールを送信することです。既定では、ログインしているユーザーが受信者ですが、他の任意の受信者に変更することができます。ここで操作するコードは **Controllers** フォルダーと **SendMailViewController.m** クラスにあります。ここには、UI を表す他のコードや、Microsoft Graph サービスからユーザー プロファイル情報を取得するヘルパー メソッドも入っています。メール メッセージの作成とそのメッセージの送信を行うメソッドに焦点を当てます。

1. Controllers フォルダー内の **SendMailViewController.m** を開いて、**viewDidLoad** メソッドの `self.graphClient = [MSGraphClient client]` の後に次のコードを追加します。 `self.graphClient = [MSGraphClient client]`
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

1. Controllers フォルダー内の **SendMailViewController.m** を開いて、 このクラスに次のヘルパー メソッドを追加します。
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
3. **SendMailViewController.m** を開きます。このクラスに次のメソッドを追加します。
**uploadPictureToOneDrive** によって、[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) の情報からの [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) のプロフィール画像がアップロードされ、サンプルによって送信される電子メールの本文に埋め込まれる Web 共有 URL が返されます。

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
4. **SendMailViewController.m** を開き、このクラスに次のメソッドを追加します。 
[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) のプロフィール画像がある場合、**getUserPicture** によってその画像が返されます。
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
3. **SendMailViewcontroller.m** を開き、このクラスに次のメソッドを追加します。
このメソッドでは、認証されたユーザーを示す [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) リソースを取得し、ユーザーのプロフィール画像を取得して電子メールを送信するために必要なフィールドをキャッシュします。
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
3. **SendMailViewController.m** を開きます。このクラスに次の送信メール メソッドを追加します。
**getSampleMessage** によって、デモのために使用する HTML 形式のサンプル メールの下書きが作成されます。 すると、次のメソッド (**sendMail**) がそのメッセージを受け取り、それを送信するための要求を実行します。 この場合も、既定の受信者はサインインしているユーザーです。


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



## <a name="run-the-app"></a>アプリの実行
1. サンプルを実行する前に、セクション「**アプリの登録**」で登録プロセスから受け取ったクライアント ID を指定する必要があります。**Application** フォルダー内の **AuthenticationConstants.m** を開きます。登録プロセスから受け取った ClientID をファイルの最上部に追加できることがわかります。  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

>注: 次のアクセス許可の適用範囲がこのプロジェクトに対して構成されていることがわかります: **"https://graph.microsoft.com/Mail.Send"、"https://graph.microsoft.com/User.Read"、"offline_access"**。このプロジェクトで使用されるサービス呼び出し、メール アカウントへのメールの送信、および一部のプロファイル情報 (表示名、メール アドレス) の取得では、アプリが適切に実行するためにこれらのアクセス許可が必要です。

2. サンプルを実行し、**[Connect]** をタップして、個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。

3. **[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。

## <a name="next-steps"></a>次の手順
- [Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。
- [Microsoft Graph iOS オブジェクティブ C スニペット サンプル](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample)に、REST 操作と SDK 操作の両方に共通する操作の例があります。

## <a name="see-also"></a>関連項目
- [iOS 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [Azure AD v2.0 のプロトコル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 のトークン](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
