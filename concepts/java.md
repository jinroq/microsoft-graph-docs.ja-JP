# <a name="get-started-with-microsoft-graph-in-a-java-app"></a>Java アプリで Microsoft Graph を使ってみる

この記事では、[console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample) を使用して、Java コンソール アプリケーションから Microsoft Graph 経由でメールを送信する方法について順を追って説明します。 この記事では、Microsoft Graph API を使用できるようにするために、Java アプリに追加する必要のあるコードについて説明します。 このアプリは、[Java 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-java) を使用して Microsoft Graph にアクセスします。

## <a name="choose-an-authentication-library"></a>認証ライブラリの選択

Microsoft Graph では OAuth 2.0 および Open ID Connect 標準を採用しているので、多彩なオープン ソース OAuth 2 Java ライブラリから選択できます。 Azure AD チームは、Java 用の単純な OAuth2 ライブラリである [ScribeJava](https://github.com/scribejava/scribejava) の使用をお勧めします。

以下のサンプルは、クライアント承認シナリオ、ユーザー、OAuth 2 対応エンドポイントで選択するのに適した、認証コードの付与フローを実装します。 運用サーバー間 Java アプリケーションでは、クライアント資格情報の認証フローが使用されます。 **ScribeJava** は、これらの認証フローを両方とも処理します。 以下のサンプルは、登録、認証、実行をしやすくするため、最も簡単なフローでデモンストレーションします。

アプリは、Microsoft Graph で呼び出しを行う前に、Azure Active Directory (Azure AD) からアクセス トークンを取得する必要があります。 このトークンは、Microsoft Graph に対する各呼び出しの HTTP 認証ヘッダー内に存在する必要があります。 [IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java) を実装すると、各呼び出しに対するヘッダーの挿入とトークンの追加を **Microsoft Graph SDK** が処理します。 **ScribeJava** は認証とアクセス トークンの取得を処理します。 アプリは、**IAuthenticationProvider** インターフェイス経由で Microsoft Graph SDK にアクセス トークンを提供します。

## <a name="install-and-run-the-sample"></a>サンプルのインストールと実行

サンプル アプリをインストールして設定するには、GitHub の **console-java-connect-sample** リポジトリにある「[Readme](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md)」ドキュメントの手順を実行します。 リポジトリを複製する次のコマンドを使用して、サンプルを複製し、お気に入りの Java IDE でコードを順を追って確認できます。

```
git@github.com:microsoftgraph/console-java-connect-sample.git
```

[コンソール Java 接続アプリを登録する](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app)際に、委任されたスコープ (アクセス許可) をサンプルに割り当てます。 スコープは、必ず次の図に示すように設定します。

![Java 接続コンソール サンプルのアクセス許可](../concepts/images/console-java-connnect-sample-permissions.JPG)

アプリケーションを登録し、そのアプリケーション登録で入手する**アプリケーション ID** に合わせて[サンプルを構成する](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app)と、サンプルをビルドして実行できるようになります。

## <a name="console-java-connect-code"></a>コンソール Java 接続コード 

サンプルのロジック フローを確認する前に、「[サンプル プロジェクトの構造](#sample-project-structure)」を概観してください。 それが済んでから、以下に示すサンプルのロジックの説明に移るようにお勧めします。


   
### <a name="walk-through-the-code"></a>コードの概観
まず、サンプル コードの全体像を説明し、次にメール メッセージの作成と送信に関する詳細を説明します。

#### <a name="the-user-experience"></a>ユーザー エクスペリエンス

この項では、アプリケーションの起動ロジックを説明し、ユーザーがサンプルを実行すると表示されるサンプル出力について説明します。

[PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) の **main** 静的メソッドが、**PublicClient** のインスタンスを作成し、サインインと認証プロセスを開始します。  

[AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) は、ユーザーを Microsoft Graph に接続する際に使用されるシングルトン インスタンスを提供します。 **AuthenticationManager** が、**アクセス トークン**を文字列プロパティとして公開します。 ユーザーが認証され、要求された Microsoft Graph リソースにアクセスする許可をサンプルに付与すると、このアクセス トークンが **Azure AD** によって返されます。 

**PublicClient.startSendMail** メソッドが、次の手順を実行します。

- [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java) クラスの新しいインスタンスを作成します。 
- サンプル コンソール オブジェクトがユーザーに表示するプロンプトのパーソナル設定を行えるように、**GraphSendMail.getMeUser()** を呼び出して、現在のユーザーの **Azure AD** プロファイルを返します。 
- コンソールに次のように表示されます。

   `Hello, Laura Steele. Would you like to send an email to yourself or someone else?`

   `Enter the address to which you'd like to send a message. If you enter nothing, the message will go to your address`

- ユーザーの入力を処理する **GraphSendMail.sendMail** メソッドを呼び出します。 メール アドレスが入力された場合、**sendMail** はそのアドレスにメッセージを送信します。 入力されなかった場合は、現在のユーザーにそのメッセージが送信されます。 

- 別のメールを送信するか、コンソール アプリを終了するかをユーザーに確認するプロンプトが表示されます。

   `Email sent!`

   `Want to send another message? Type 'y' for yes and any other key to exit.`

#### <a name="the-send-mail-logic"></a>メールの送信ロジック

メールの送信ロジックは次の手順で行われます。



1. **プロフィール画像の取得**:<br/> **GraphServiceController.getUserProfilePicture()** を呼び出して、サンプルにサインインしている **Azure AD** ユーザーのプロフィール画像を表すバイトの配列を取得します。

   **API 呼び出し**

```java
            photoStream = mGraphServiceClient
                    .me()
                    .photo()
                    .content()
                    .buildRequest()
                    .get();

```
2. **OneDrive への画像のアップロード**:
<br/>**GraphServiceController.uploadPictureToOneDrive(bytes)** を呼び出して、そのユーザーの OneDrive のルート フォルダーにあるプロフィール画像を POST します。 Microsoft Graph SDK の **DriveItem** オブジェクトが返されます。 

   **API 呼び出し**
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
3. **画像の OneDrive 共有リンクの取得**:<br/>**GraphServiceController.getPermissionSharingLink** を呼び出して、新しい共有リンクを作成します。 Microsoft Graph SDK の **Permission** オブジェクトが返されます。

   **API 呼び出し**
```java
            permission = mGraphServiceClient
                    .me()
                    .drive()
                    .items(id)
                    .createLink("view", "organization")
                    .buildRequest()
                    .post();

```
4. 前の手順で作成した共有リンクの **webUrl** で、**HTML テンプレートのアンカー タグの内容を置換**します。 
> **注:** アプリケーションから送信されたメッセージの本文は、[Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java) に静的な文字列として保存される HTML テンプレートとして生成されます。 送信時に、メッセージの本文には、サンプルがユーザーの OneDrive ルート フォルダーにアップロードする画像へのパブリック共有ハイパーリンクが含まれます。 
5. **下書きメッセージの作成**: <br/>**GraphServiceController.createDraftMail** を呼び出し、受信者のメール アドレス、件名のテキスト、および更新された HTML テンプレートを渡します。 下書きメッセージが作成され、ユーザーの下書きメッセージ フォルダーに POST されます。

   **API 呼び出し**
```java
            message = mGraphServiceClient
                    .me()
                    .messages()
                    .buildRequest()
                    .post(message);

```
6. **下書きメッセージへの画像添付**: <br/>**GraphServiceController.addPictureToDraftMessage** を呼び出し、下書きメッセージを取得して、オブジェクトの添付ファイルとしてメッセージに画像を追加します。

   **API 呼び出し**
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
7. **下書きメッセージの送信**:<br/>**GraphServiceController.sendDraftMessage** を呼び出し、更新した下書きメッセージを意図したユーザーに送信します。

   **API 呼び出し**
```java
            mGraphServiceClient
                    .me()
                    .mailFolders("Drafts")
                    .messages(messageId)
                    .send()
                    .buildRequest()
                    .post();

```



### <a name="sample-project-structure"></a>サンプル プロジェクトの構造

### <a name="connect-package"></a>接続パッケージ
このパッケージには、OAuth2 認証フロー ロジック、および更新対象の構成が含まれています。

- [AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java): このクラスは、認証コードの付与フローで使用する **ScribeJava** オブジェクトをインポートします。
- [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java): アプリの登録に関連した値を提供するパブリックの静的文字列と、アプリケーションが送信するメール メッセージのテンプレートを格納しています。
- [Debug.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java): パブリック デバッグ レベルのフラグです。 値を設定して、サンプル アプリのログの動作を変更します。
- [DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java): デバッグ レベル設定に従って、コンソールに情報を書き込むログ ユーティリティです。
- [IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java): **ScribeJava.getAccessToken** メソッドの非同期オーバーロードを呼び出す場合に使用するコールバック メソッドを定義します。
- [SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java): **Exception** の派生クラスで、Microsoft Graph 固有の例外情報をカプセル化します。 **GraphSendMail** パッケージのクラスは、この種類の例外をスローする場合があります。

### <a name="msgraph-package"></a>msgraph パッケージ

このパッケージには、Microsoft Graph で呼び出しを実行するロジックが含まれています。

- [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java): 呼び出しを **GraphServiceController** (Microsoft Graph API サンプル ヘルパー クラス) に連鎖して、画像が添付されたメール メッセージを作成および送信します。
- [GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java): Microsoft Graph SDK [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java) をインスタンス化し、Microsoft Graph エンドポイント上のすべての発信 API 呼び出しにアクセス トークンを追加します。

- [GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java): Microsoft Graph SDK を使用して、**GraphServiceClient** 上のすべての呼び出しを作成します。 次の呼び出しが作成されます。

   - **createDraftMail**: メール メッセージの下書きを作成し、下書きメッセージ フォルダーに保存します。
   - **sendNewMessageAsync**: メール メッセージを作成および送信します。
   - **addPictureToDraftMessage**: メッセージ ID で、下書きメッセージの添付ファイルを POST します。
   - **addAttachmentToDraftAsync**: 下書きメッセージに添付ファイルを追加します。
   - **sendDraftMessage**: 下書きフォルダーからメッセージを送信します。
   - **getDraftMessage**: メッセージ ID で、ユーザーのメッセージ コレクションからメッセージを取得します。
   - **getUser**: Microsoft Graph API エンドポイントで認証されるローカル ユーザーを取得します。
   - **getUserProfilePicture**: サインインしているユーザーのプロフィール画像を Microsoft Graph から取得します。
   - **uploadPictureToOneDrive**: 画像をバイト配列として、ユーザーの OneDrive ルート フォルダーにアップロードします。
   - **getPermissionSharingLink**: OneDrive に保存されている画像への公開共有リンクを作成するように OneDrive に要求します。

## <a name="other-microsoft-graph-samples"></a>Microsoft Graph の他のサンプル

ご覧になりたい特定のサンプルがある場合、[懸案事項を送信](https://github.com/microsoftgraph/console-java-connect-sample/issues)してお知らせください。 Java で構築する Microsoft Graph シナリオに対するお客様のフィードバックを大いに歓迎いたします。

Microsoft Graph API は、あらゆる種類の Microsoft データとの対話に使用できる、非常に強力な統合 API です。 [開発者ドキュメント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/overview)または [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) で、Microsoft Graph によってさらに行える事柄について確認してください。
