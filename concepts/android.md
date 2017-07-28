# <a name="get-started-with-microsoft-graph-in-an-android-app"></a>Android アプリで Microsoft Graph を使ってみる

> **エンタープライズのお客様向けにアプリを作成していますか?**エンタープライズのお客様が、<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件付きのデバイスへのアクセス</a>のようなエンタープライズ モビリティ セキュリティの機能をオンにしている場合、アプリが動作しない可能性があります。その場合、気がつかないまま、お客様の側でエラーが発生してしまう可能性があります。 

> **すべてのエンタープライズのお客様**の**すべてのエンタープライズ シナリオ**をサポートするには、Azure AD エンドポイントを使用し、[Azure 管理ポータル](https://aka.ms/aadapplist)でアプリを管理する必要があります。詳細については、「[Azure AD か Azure AD v2.0 エンドポイントかを決定する](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。

この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、Microsoft Graph を呼び出すために必要なタスクについて説明します。ここでは、[Android 用接続サンプル](https://github.com/microsoftgraph/android-java-connect-sample)のビルドの手順と、Android 用アプリで Microsoft Graph を使用するために実施する主要な概念について説明します。またこの記事では、[Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) または未加工の REST 呼び出しを使用して Microsoft Graph にアクセスする方法についても説明します。

Android 用アプリで Microsoft Graph を使用するには、以下のスクリーンショットに示すような Microsoft のサインイン ページをユーザーに表示する必要があります。

![Android 上の Microsoft アカウントのサインイン ページ](images/AndroidConnect.png)

**アプリを作成してみたくありませんか。**この記事の基になっている [Android 用接続サンプル](https://github.com/microsoftgraph/android-java-connect-sample)をダウンロードすれば、すぐに始めることができます。


## <a name="prerequisites"></a>前提条件

開始するには、次のものが必要です。 

- [Microsoft アカウント](https://www.outlook.com/)か[職場または学校アカウント](http://dev.office.com/devprogram)
- Android Studio 2.0 以降のバージョン


## <a name="configure-a-new-project"></a>新規プロジェクトを構成する

[Android 用接続サンプル](https://github.com/microsoftgraph/android-java-connect-sample)をダウンロードしている場合は、この手順をスキップしてください。 

Android Studio で新しいプロジェクトを開始します。ほとんどのウィザードで既定値のままにしておきますが、次のオプションを選択するようにしてください。

* ターゲット Android デバイス - **携帯電話とタブレット**
    * 最小 SDK - **API 16:Android 4.1 (Jelly Bean)**
* モバイルにアクティビティを追加 - **基本的なアクティビティ**
 
これにより、Android プロジェクトにアクティビティとユーザーの認証に使用できるボタンが追加されます。


## <a name="register-the-application"></a>アプリケーションを登録する

接続サンプルをダウンロードした場合でも、新しいプロジェクトを作成した場合でも、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)でアプリを登録する必要があります。

Microsoft アプリ登録ポータルでアプリを登録します。これにより、アプリの構成に使用するアプリ ID が生成されます。

1. 個人用アカウント、あるいは職場または学校アカウントのいずれかを使用して、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。

2. **[アプリの追加]** を選択します。

>ヒント: [Android 用接続サンプル](https://github.com/microsoftgraph/android-java-connect-sample)をダウンロードし、その登録のみを行う場合は、**[作成]** ボタンを押す前に**[ガイド付きセットアップ]** のチェックを外してください。

3. アプリの名前を入力して、**[作成]** を選択します。 
    
    **ガイド付きセットアップ** のフローは次のようになります。
 
    a.**[モバイルおよびデスクトップ アプリ]** を選択して、作成するアプリの種類を定義します。

    b.**[Android]** を選択して、使用しているモバイル テクノロジを定義します。

    c.最初のトピックを確認し、終了したら、ページの最後にある**[セットアップ]** ボタンをクリックします。

    d.**[セットアップ]** の手順の説明に従って、MSAL ライブラリをアプリの build.gradle に追加します。

    e.**[ユーザー]** の手順の指示に従って、MSAL ロジックを新しいプロジェクトに追加します。

    f.**[構成]**ページで、ポータルによって独自のアプリケーション ID が作成されています。これを使用してアプリを構成します。

    ガイドなしのフローは次のようになります。

    登録ページが表示され、アプリのプロパティが一覧表示されます。

    a.アプリケーション ID をコピーします。これは、アプリの一意識別子です。 

    b.**[プラットフォームの追加]** および **[ネイティブ アプリケーション]** を選択します。

    > **注:**アプリケーション登録ポータルでは、値 *msalYOUR NEW APP ID://auth* のリダイレクト URI が表示されます。組み込みリダイレクト URI は使用しないでください。[Android 用接続サンプル](https://github.com/microsoftgraph/android-java-connect-sample)には、このリダイレクト URI を必要とする MSAL 認証ライブラリが実装されています。[サポートされているサード パーティ製ライブラリ](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries)または **ADAL** ライブラリを使用している場合は、組み込みのリダイレクト URI を使用する必要があります。

    ガイド付きセットアップのフローとガイドなしのフロー

    a.委任されたアクセス許可を追加します。**profile**、**Mail.ReadWrite**、**Mail.Send**、**Files.ReadWrite**、**User.ReadBasic.All** が必要になります。 
   
    b.**[保存]** を選択します。


## <a name="authenticate-the-user-and-get-an-access-token"></a>ユーザーの認証とアクセス トークンの取得

> **注:**アプリケーション登録ポータルから **[ガイド付きセットアップ]** のフローの指示に従って新しいアプリケーションを作成した場合は、これらの手順をスキップできます。Graph API の詳細については、「[Microsoft Graph SDK を使用して Microsoft Graph を呼び出す](#call-microsoft-graph-using-the-microsoft-graph-sdk)」に移動してください。

追加した MSAL と Microsoft Graph コードについては、「[Android 用接続サンプル](https://github.com/microsoftgraph/android-java-connect-sample)」で説明します。

### <a name="add-the-dependency-to-appbuildgradle"></a>app/build.gradle に依存関係を追加する

アプリのモジュールで `build.gradle` ファイルを開き、次の依存関係を検索します。

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'

```

### <a name="start-the-authentication-flow"></a>認証フローの開始

1. **AuthenticationManager** ファイルを開きます。**PublicClientApplication** オブジェクトの宣言を検索し、次に **getInstance** メソッドでインスタンスを検索します。

   ```java
    private static PublicClientApplication mPublicClientApplication;
    ....

    public static synchronized AuthenticationManager getInstance() {
        if (INSTANCE == null) {
            INSTANCE = new AuthenticationManager();
            if (mPublicClientApplication == null) {
                mPublicClientApplication = new PublicClientApplication(Connect.getInstance());
            }
        }
        return INSTANCE;
    }

   ```


2. **ConnectActivity** クラスで、**mConnectButton** のクリック イベントのイベント ハンドラーを検索します。**onClick** メソッドを検索して、関連するコードを確認します。
  
    **connect** メソッドは個人情報 (PII) のログ収集を有効にし、サンプルのヘルパー クラス **AuthenticationManager** のインスタンスを取得し、MSAL プラットフォームのオブジェクトのユーザー コレクションを取得します。ユーザーが存在しない場合、新しいユーザーは Azure AD の認証と承認フローに移動されます。それ以外の場合は、メッセージなしで認証トークンを取得します。

   ```java
    @Override
    public void onClick(View view) {
        ....
        connect();
    }

        private void connect() {

        if (mEnablePiiLogging) {
            Logger.getInstance().setEnablePII(true);
        } else {
            Logger.getInstance().setEnablePII(false);
        }

        AuthenticationManager mgr = AuthenticationManager.getInstance();

        List<User> users = null;

        try {
            users = mgr.getPublicClient().getUsers();

            if (users != null && users.size() == 1) {
                mUser = users.get(0);
                mgr.callAcquireTokenSilent(mUser, true, this);
            } else {
                mgr.callAcquireToken(
                        this,
                        this);
            }
        } catch (MsalClientException e) {
            Log.d(TAG, "MSAL Exception Generated while getting users: " + e.toString());

        } catch (IndexOutOfBoundsException e) {
            Log.d(TAG, "User at this position does not exist: " + e.toString());
        }
    }

   ```
3. ユーザーが認証ダイアログを閉じたときに Azure AD によって生成された Azure AD のリダイレクト応答を処理するイベント ハンドラーを検索します。このハンドラーは、**ConnectActivity** クラスにあります。

   ```java
       /**
     * Handles redirect response from https://login.microsoftonline.com/common and
     * notifies the MSAL library that the user has completed the authentication
     * dialog
     * @param requestCode
     * @param resultCode
     * @param data
     */
    @Override
    protected void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if (AuthenticationManager
                .getInstance()
                .getPublicClient() != null) {
            AuthenticationManager
                    .getInstance()
                    .getPublicClient()
                    .handleInteractiveRequestRedirect(requestCode, resultCode, data);
        }
    }

   ```    
3. Graph API の呼び出しで使用される認証トークンをキャッシュする、認証コールバック メソッドを検索します。

 

```java
    /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

```
    
接続サンプルのアプリでは、メインのアクティビティに **[接続]** ボタンがあります。初回使用時にボタンを押すと、デバイスのブラウザーを使用した認証ページがアプリに表示されます。次の手順は、認証サーバーがリダイレクト URI にコードを送信してアクセス トークンと交換する作業です。

### <a name="exchange-the-authorization-code-for-an-access-token"></a>認証コードとアクセス トークンの交換

アクセス トークンと交換できるコードが含まれている認証サーバーの応答をアプリが処理できるようにする必要があります。

1. Connect アプリがアプリケーション登録で構成されたリダイレクト URL への要求を処理できることを、Android システムに告げる必要があります。これを行うには、**AndroidManifest** ファイルを開き、次の子をプロジェクトの **\<application/\>** 要素に追加します。
    ```xml
        <uses-sdk tools:overrideLibrary="com.microsoft.identity.msal" />
        <application ...>
            ...
            <activity
                android:name="com.microsoft.identity.client.BrowserTabActivity">
                <intent-filter>
                    <action android:name="android.intent.action.VIEW" />
                    <category android:name="android.intent.category.DEFAULT" />
                    <category android:name="android.intent.category.BROWSABLE" />
                    <data android:scheme="msalENTER_YOUR_CLIENT_ID"
                        android:host="auth" />
                </intent-filter>
            </activity>
            <meta-data
                android:name="https://login.microsoftonline.com/common"
                android:value="authority string"/>
            <meta-data
                android:name="com.microsoft.identity.client.ClientId"
                android:value="ENTER_YOUR_CLIENT_ID"/>
        </application>
    ```
2. **MSAL**ライブラリは、登録ポータルによって割り当てられたアプリケーション ID にアクセスする必要があります。**MSAL ライブラリは、アプリケーション ID を「クライアント ID」として参照します**。これは、ライブラリのコンストラクターで渡したアプリケーション コンテキストからアプリケーション ID (クライアント ID) を取得します。 

   >注:コンストラクターに文字列パラメーターを渡すことにより、実行時にクライアント ID を提供することもできます。 

3. 認証サーバーが応答を送信すると、アクティビティが呼び出されます。認証サーバーからの応答で、アクセス トークンを要求します。**AuthenticationManager** に移動し、クラス内で次のコードを検索します。

   ```java
    /**
     * Authenticates the user and lets the user authorize the app for the requested permissions.
     * An authentication token is returned via the getAuthInteractiveCalback method
     * @param activity
     * @param authenticationCallback
     */
    public void connect(Activity activity, final MSALAuthenticationCallback authenticationCallback){
        mActivityCallback = authenticationCallback;
        mPublicClientApplication.acquireToken(
                activity, Constants.SCOPES, getAuthInteractiveCallback());
    }


     /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

     /**
     * Returns the access token obtained in authentication
     *
     * @return mAccessToken
     */
    public String getAccessToken() throws AuthenticatorException, IOException, OperationCanceledException {
        return  mAuthResult.getAccessToken();
    }

   ```


## <a name="call-microsoft-graph"></a>Microsoft Graph を呼び出す
[Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) または [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) を使用して、Microsoft Graph を呼び出すことができます。

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a>Microsoft Graph SDK を使用して Microsoft Graph を呼び出す
[Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) では、要求をビルドして Microsoft Graph からの結果を処理するクラスを作成できます。以下の手順に従って Microsoft Graph SDK を使用します。

1. アプリにインターネット アクセス許可を付与します。**AndroidManifest** ファイルを開き、マニフェスト要素に次の子を追加します。
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

    ```

2. Microsoft Graph SDK および GSON に依存関係を追加します。
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. **uthenticateRequest** ヘルパー メソッドを使用して、新しい要求に認証トークンを追加します。このメソッドは同じメソッドを Microsoft Graph 認証の **IAuthenticationProvider** インターフェイスから実装します
    
   ```java
    /**
     * Appends an access token obtained from the {@link AuthenticationManager} class to the
     * Authorization header of the request.
     * @param request
     */
    @Override
    public void authenticateRequest(IHttpRequest request)  {
        try {
            request.addHeader("Authorization", "Bearer "
                    + AuthenticationManager.getInstance()
                    .getAccessToken());
            // This header has been added to identify this sample in the Microsoft Graph service.
            // If you're using this code for your project please remove the following line.
            request.addHeader("SampleID", "android-java-connect-sample");
        } catch (AuthenticatorException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        }  catch (OperationCanceledException e) {
            e.printStackTrace();
        } catch (NullPointerException e) {
            e.printStackTrace();
        }
    }
   ```

4. 下書き電子メールを作成し、**GraphServiceController** ヘルパー クラスから次のヘルパー メソッドを使用して送信します。

   ```java
    /**
     * Creates a draft email message using the Microsoft Graph API on Office 365. The mail is sent
     * from the address of the signed in user.
     *
     * @param senderPreferredName The mail senders principal user name (email addr)
     * @param emailAddress        The recipient email address.
     * @param subject             The subject to use in the mail message.
     * @param body                The body of the message.
     * @param callback            The callback method to invoke on completion of the POST request
     */
    public void createDraftMail(
            final String senderPreferredName,
            final String emailAddress,
            final String subject,
            final String body,
            ICallback<Message> callback
    ) {
        try {
            // create the email message
            Message message = createMessage(subject, body, emailAddress);
            mGraphServiceClient
                    .getMe()
                    .getMessages()
                    .buildRequest()
                    .post(message, callback);

        } catch (Exception ex) {
            showException(ex, "exception on send mail","Send mail failed", "The send mail method failed");
        }
    }

        /**
     * Creates a new Message object 
     */
    Message createMessage(
            String subject,
            String body,
            String address) {

        if (address == null || address.isEmpty()) {
            throw new IllegalArgumentException("The address parameter can't be null or empty.");
        } else {
            // perform a simple validation of the email address
            String addressParts[] = address.split("@");
            if (addressParts.length != 2 || addressParts[0].length() == 0 || addressParts[1].indexOf('.') == -1) {
                throw new IllegalArgumentException(
                        String.format("The address parameter must be a valid email address {0}", address)
                );
            }
        }
        Message message = new Message();
        EmailAddress emailAddress = new EmailAddress();
        emailAddress.address = address;
        Recipient recipient = new Recipient();
        recipient.emailAddress = emailAddress;
        message.toRecipients = Collections.singletonList(recipient);
        ItemBody itemBody = new ItemBody();
        itemBody.content = body;
        itemBody.contentType = BodyType.html;
        message.body = itemBody;
        message.subject = subject;
        return message;
    }
    /**
     * Sends a draft message to the specified recipients
     *
     * @param messageId String. The id of the message to send
     * @param callback
     */
    public void sendDraftMessage(String messageId,
                                 ICallback<Void> callback) {
        try {

            mGraphServiceClient
                    .getMe()
                    .getMessages(messageId)
                    .getSend()
                    .buildRequest()
                    .post(callback);

        } catch (Exception ex) {
            showException(ex, "exception on send draft message ","Send draft mail failed", "The send draft mail method failed");
        }
    }

   ```
### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a>Microsoft Graph REST API を使用して Microsoft Graph を呼び出す
[Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) は 1 つの REST API エンドポイントを介して複数の API を Microsoft クラウド サービスから公開するものです。以下の手順に従って、REST API を使用します。

1. アプリにインターネット アクセス許可を付与します。**AndroidManifest** ファイルを開き、マニフェスト要素に次の子を追加します。
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. Volley HTTP ライブラリへの依存関係を追加します。

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. 行 `String accessToken = tokenResponse.accessToken;` を次のコードに置き換えます。**\<YOUR_EMAIL_ADDRESS\>** とマークされているプレースホルダーに電子メール アドレスを挿入します。
   ```java
    final String accessToken = tokenResponse.accessToken;

    final RequestQueue queue = Volley.newRequestQueue(getApplicationContext());
    String url ="https://graph.microsoft.com/v1.0/me/sendMail";
    final String body = "{" +
        "  Message: {" +
        "    subject: 'Sent using the Microsoft Graph REST API'," +
        "    body: {" +
        "      contentType: 'text'," +
        "      content: 'This is the email body'" +
        "    }," +
        "    toRecipients: [" +
        "      {" +
        "        emailAddress: {" +
        "          address: '<YOUR_EMAIL_ADDRESS>'" +
        "        }" +
        "      }" +
        "    ]}" +
        "}";

    final StringRequest stringRequest = new StringRequest(Request.Method.POST, url,
        new Response.Listener<String>() {
            @Override
            public void onResponse(String response) {
                Log.d("Response", response);
            }
        },
        new Response.ErrorListener() {
            @Override
            public void onErrorResponse(VolleyError error) {
                Log.d("ERROR","error => " + error.getMessage());
            }
        }
    ) {
        @Override
        public Map<String, String> getHeaders() throws AuthFailureError {
            Map<String,String> params = new HashMap<>();
            params.put("Authorization", "Bearer " + accessToken);
            params.put("Content-Length", String.valueOf(body.getBytes().length));
            return params;
        }
        @Override
        public String getBodyContentType() {
            return "application/json";
        }
        @Override
        public byte[] getBody() throws AuthFailureError {
            return body.getBytes();
        }
    };

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            queue.add(stringRequest);
        }
    });
   ```

## <a name="run-the-app"></a>アプリの実行
Android アプリを試す準備ができました。

1. Android エミュレーターを起動するか、物理デバイスをコンピューターに接続します。
2. Android Studio で、Shift キーを押しながら F10 キーを押してアプリを実行します。
3. 配置ダイアログ ボックスから、Android のエミュレーターまたはデバイスを選択します。
4. メインのアクティビティ内のフローティング アクション ボタンをタップします。
5. 個人用あるいは職場または学校アカウントでサインインし、要求されたアクセス許可を付与します。
6. アプリの選択ダイアログで、アプリをタップして続行します。

["Microsoft Graph を呼び出す"](#call-microsoft-graph)で構成した電子メール アドレスの受信トレイを確認します。アプリへのサインインに使用したアカウントからのメールを受信しているはずです。

## <a name="next-steps"></a>次の手順
- [Microsoft Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を試してみましょう。
- [Android 用のスニペットのサンプル](https://github.com/microsoftgraph/android-java-snippets-sample)で一般的な操作の例を見つけるか、GitHub で別の [Android サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android)を探します。


## <a name="see-also"></a>関連項目
- [Android 用 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [ユーザーの代わりにアクセスを取得](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [ユーザーなしでアクセスを取得](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)