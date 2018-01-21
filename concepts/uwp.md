# <a name="get-started-with-microsoft-graph-in-a-universal-windows-10-app"></a>ユニバーサル Windows 10 アプリで Microsoft Graph を使ってみる

> **エンタープライズのお客様向けにアプリを作成していますか?**エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。 

> **すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。

この記事では、[Azure AD v2.0 エンドポイント](https://developer.microsoft.com/ja-JP/graph/docs/concepts/converged_auth)からアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[UWP 用 Microsoft Graph Connect サンプル (ライブラリ)](https://github.com/microsoftgraph/uwp-csharp-connect-sample) のサンプル内のコードを説明し、Microsoft Graph を使用するアプリで実装する必要のある主要な概念について説明します。

**アプリを作成してみたいですか。**[Microsoft Graph クイック スタート](https://developer.microsoft.com/graph/quick-start)を使用してすぐに使い始めるか、またはこの記事で取り扱っている [UWP 用 Microsoft Graph Connect サンプル (ライブラリ)](https://github.com/microsoftgraph/uwp-csharp-connect-sample) をダウンロードしてください。[REST バージョンのサンプル](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample)も利用できます。

## <a name="sample-user-interface"></a>サンプル ユーザー インターフェイス

サンプルには、上部のコマンド バー、**[接続]** ボタン､**[メールの送信]** ボタン、およびサインイン ユーザーの電子メールアドレスが自動入力された編集可能なテキスト ボックスで構成される非常にシンプルなユーザー インターフェイスが含まれています。

**[メールの送信]** ボタンは、ユーザーが接続されていないときは無効になります。

![[接続] ボタンが有効になっていて、[メールの送信] ボタンが無効になっていることを示す画面](images/SignedOut.png)

ユーザーが接続されている場合、上部のコマンド バーに [切断] ボタンが表示されます。

![接続されたユーザーの電子メール アドレスと [メールの送信] ボタンが有効になっていることを示す画面](images/SignedIn.png)

すべてのサンプルの UI 文字列は、Assets フォルダー内の Resources.resw ファイルに格納されています。

## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

- [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)
- Visual Studio 2017 
- [UWP 用 Microsoft Graph スターター プロジェクト (ライブラリ)](https://github.com/microsoftgraph/uwp-csharp-connect-sample/tree/master/starter)。両方のテンプレートには、コードを追加する空のクラスが含まれています。また、リソース文字列も含まれています。このプロジェクトを取得するには、[UWP 用 Microsoft Graph Connect のサンプル (ライブラリ)](https://github.com/microsoftgraph/uwp-csharp-connect-sample) を複製またはダウンロードして、**starter** フォルダー内のソリューションを開きます。


## <a name="register-the-app"></a>アプリを登録する
 
1. 個人用アカウントか職場または学校アカウントのいずれかを使用して、[アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。
2. **[アプリの追加]** を選択します。
3. アプリの名前を入力して、**[アプリケーションの作成]** を選択します。
    
    登録ページが表示され、アプリのプロパティが一覧表示されます。
 
4. **[プラットフォーム]** で、**[プラットフォームの追加]** を選択します。
5. **[ネイティブ アプリケーション]** を選択します。
6. クライアント ID (アプリ ID) とリダイレクト URI の値の両方をクリップボードにコピーします。サンプル アプリにこれらの値を入力する必要があります。

    アプリ ID は、アプリの一意識別子です。リダイレクト URI は、各アプリケーションに対して Windows 10 で提供される一意の URI であり、その URI に送信されたメッセージだけがそのアプリケーションに送信されます。 

7. **[保存]** を選びます。

## <a name="configure-the-project"></a>プロジェクトを構成する

1. Visual Studio でスターター プロジェクトのソリューション ファイルを開きます。
2. プロジェクトの **App.xaml** ファイルを開き、`Application.Resources` ノードを見つけます。アプリケーション ID とリダイレクト URI のプレースホルダーを、登録したアプリの対応する値に置き換えます。


```xml
    <Application.Resources>
        <!-- Add your Client Id here. -->
        <x:String x:Key="ida:ClientID">ENTER_YOUR_CLIENT_ID</x:String>
        <!-- Add your Redirect URI here. -->
        <x:String x:Key="ida:ReturnUrl">ENTER_YOUR_REDIRECT_URI</x:String>
    </Application.Resources>
```

## <a name="send-an-email-with-microsoft-graph"></a>Microsoft Graph を使用して電子メールを送信する

スターター プロジェクトの MailHelper.cs ファイルを開きます。このファイルには、電子メールを作成して送信するコードが含まれています。それは、POST 要求を作成して **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** エンドポイントに送信する単一のメソッド (``ComposeAndSendMailAsync``) で構成されています。 

``ComposeAndSendMailAsync`` メソッドは、MainPage.xaml.cs ファイルによって渡される 3 つの文字列値 (``subject``、``bodyContent``、``recipients``) を取得します。``subject`` および ``bodyContent`` の文字列は、その他のすべての UI 文字列とともに Resources.resw ファイルに格納されます。``recipients`` の文字列はアプリのインターフェイスにあるアドレス ボックスのものです。 

``ComposeAndSendMailAsync`` メソッド内の最初のタスクでは、Microsoft Graph から現在のユーザーの写真を取得します。この行は、`GetCurrentUserPhotoStreamAsync` メソッドを呼び出します。

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

完全な `GetCurrentUserPhotoStreamAsync` メソッドは、次のようになります。

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

ユーザーが写真を持っていない場合、このロジックでは、プロジェクトに含まれている別のイメージ ファイルを取得します。

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                StorageFile file = await Windows.ApplicationModel.Package.Current.InstalledLocation.GetFileAsync("test.jpg");
                photoStream = (await file.OpenReadAsync()).AsStreamForRead();
            }
```

イメージ ストリームができたため、`UploadFileToOneDriveAsync` メソッドを呼び出してファイルを OneDrive にアップロードできます。

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

完全な `UploadFileToOneDriveAsync` メソッドは、次のようになります。

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

このストリームは、次のメッセージとともに渡すことができる `MessageAttachmentsCollectionPage` オブジェクトの作成にも使用できます。

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

`GetSharingLinkAsync` メソッドを呼び出して、新しくアップロードした OneDrive ファイルの共有リンクを取得できます。`bodyContent` 文字列には、共有リンクのプレースホルダーが含まれています。

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

完全な `GetSharingLinkAsync` メソッドは、次のようになります。

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

複数のアドレスを渡すことができるため、次は、``recipients`` 文字列を一連の `EmailAddress` オブジェクトに分割します。それは、`Recipients` オブジェクトの一覧を作成するために使用され、そのオブジェクトは要求の POST 本文に入れて渡されます。

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

最後に、`Message` オブジェクトを作成し、`GraphServiceClient` を使用して **me/microsoft.graph.SendMail** エンドポイントに送信します。``bodyContent`` の文字列は HTML 文書であるため、要求によって HTML に **ContentType** 値が設定されます。

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

完全なクラスは、次のようになります。

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

 
これで、Microsoft Graph と対話するために必要な、アプリの登録、ユーザーの認証、および要求の作成の手順が完了しました。 

## <a name="run-the-app"></a>アプリの実行
1. F5 キーを押して、アプリを構築して実行します。 

2. 個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。

3. **[メールの送信]** ボタンを選びます。メールが送信されると、ボタンの下に成功メッセージが表示されます。このメール メッセージには添付ファイルとして写真が含まれており、OneDrive にアップロードされたファイルへの共有リンクも提示されます。

## <a name="next-steps"></a>次の手順
- [Graph エクスプローラー](https://developer.microsoft.com/ja-JP/graph/graph-explorer)を使用して REST API を試してみます。
- [Microsoft Graph UWP スニペット サンプル (SDK)](https://github.com/microsoftgraph/uwp-csharp-snippets-sample) と [Microsoft Graph UWP スニペット サンプル (REST)](https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample) での REST と SDK の両方の操作に共通する操作の例を検索するか、GitHub で他の [UWP サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp)を探索します。

## <a name="see-also"></a>関連項目
- [Microsoft Graph .NET クライアント ライブラリ](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Azure AD v2.0 のプロトコル](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 のトークン](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-tokens/)

