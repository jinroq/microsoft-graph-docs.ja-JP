# <a name="get-started-with-microsoft-graph-and-rest"></a><span data-ttu-id="9053e-101">Microsoft Graph および REST 入門</span><span class="sxs-lookup"><span data-stu-id="9053e-101">Get started with Microsoft Graph and REST</span></span>

<span data-ttu-id="9053e-p101">この記事では、Azure AD v2.0 エンドポイントからアクセス トークンを取得し、REST 呼び出しを使用して Microsoft Graph を呼び出すために必要なタスクについて説明します。電子メール メッセージの認証と取得のためにアプリが使用する要求と応答を、順を追って説明します。</span><span class="sxs-lookup"><span data-stu-id="9053e-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph using REST calls. It describes the sequence of requests and responses that an app uses to authenticate and retrieve email messages.</span></span>

<span data-ttu-id="9053e-104">最初に、Azure Active Directory (Azure AD) にアプリを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9053e-104">First, you need register your app with Azure Active Directory (Azure AD).</span></span> 

## <a name="register-the-application"></a><span data-ttu-id="9053e-105">アプリケーションの登録</span><span class="sxs-lookup"><span data-stu-id="9053e-105">Register the application</span></span>

<span data-ttu-id="9053e-106">現在、Azure AD にアプリを登録するには 2 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="9053e-106">There are currently two options to register your app with Azure AD.</span></span>

  - <span data-ttu-id="9053e-107">アプリを登録して、個人用 (Microsoft) ID と職場および学校 (Azure AD) アカウントの両方で機能する Azure AD v2.0 エンドポイントを使用する。</span><span class="sxs-lookup"><span data-stu-id="9053e-107">Register an app to use the Azure AD v2.0 endpoint that works for both personal (Microsoft) identities and work and school (Azure AD) accounts.</span></span>
  - <span data-ttu-id="9053e-108">アプリを登録して、職場および学校アカウントのみをサポートする Azure AD エンドポイントを使用する。</span><span class="sxs-lookup"><span data-stu-id="9053e-108">Register an app to use the Azure AD endpoint that supports work and school accounts only.</span></span>

<span data-ttu-id="9053e-p102">この記事では、v2.0 での登録を前提にしていますので、[アプリケーション登録ポータル](https://apps.dev.microsoft.com/)でアプリを登録します。「[Microsoft Graph アプリケーションを Azure AD v2.0 エンドポイントに登録する](../concepts/auth_register_app_v2.md)」の手順に従って、アプリを登録します。Azure AD エンドポイントの使用に関する詳細は、「[Azure AD を使用して認証する](../concepts/auth_v2_user.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9053e-p102">This article assumes a v2.0 registration, so you'll register your app on the [Application Registration Portal](https://apps.dev.microsoft.com/). Follow the instructions in [Register your Microsoft Graph application with the Azure AD v2.0 endpoint](../concepts/auth_register_app_v2.md) to register your app. For information about using the Azure AD endpoint, see [Authenticate using Azure AD](../concepts/auth_v2_user.md).</span></span>

> <span data-ttu-id="9053e-p103">v2.0 エンドポイントを使用する場合、いくつかの制限が適用されます。制限が適切であるかどうかを判断するには、「[v2.0 エンドポイントを使用する必要がありますか?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9053e-p103">Some limitations apply when using the v2.0 endpoint. To decide if it's right for you, see [Should I use the v2.0 endpoint?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="9053e-114">ユーザーの認証とアクセス トークンの取得</span><span class="sxs-lookup"><span data-stu-id="9053e-114">Authenticate the user and get an access token</span></span>

<span data-ttu-id="9053e-p104">この記事で説明されているアプリは、Azure AD v2.0 エンドポイントからアクセス トークンを取得するために標準の [OAuth 2.0 プロトコル](http://tools.ietf.org/html/rfc6749)に従って[認証コードの付与フロー](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/)を実装します。Azure AD v2.0 エンドポイントでサポートされているフローの完全なガイドは、「[v2.0 エンドポイントの種類](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9053e-p104">The app described in this article implements the [Authorization Code Grant flow](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) to get access tokens from the Azure AD v2.0 endpoint, following standard [OAuth 2.0 protocols](http://tools.ietf.org/html/rfc6749). For a complete guide to the flows supported in the Azure AD v2.0 endpoint see [Types of the v2.0 endpoint](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span></span>

<span data-ttu-id="9053e-117">認証コードの付与フローを使用して、最初に認証コードを取得してから、コードをアクセス トークンと交換します。</span><span class="sxs-lookup"><span data-stu-id="9053e-117">With the Authorization Code Grant flow, first you get an authorization code and then you exchange the code for an access token.</span></span>

### <a name="getting-an-authorization-code"></a><span data-ttu-id="9053e-118">認証コードの取得</span><span class="sxs-lookup"><span data-stu-id="9053e-118">Getting an authorization code</span></span>

<span data-ttu-id="9053e-p105">承認コードの付与フローでは、まず認証コードを取得します。ユーザーがサインインし、アプリが要求するアクセス許可に同意すると、コードが認証サーバーによってアプリに返されます。</span><span class="sxs-lookup"><span data-stu-id="9053e-p105">The first step in the Authorization Code Grant flow is to get an authorization code. The code is returned to the app by the authorization server when the user signs in and consents to the permissions requested by the app.</span></span>

<span data-ttu-id="9053e-p106">認証コードを要求するには、Azure AD v2.0 エンドポイントに GET 要求を送信します。この URL は、ユーザーがサインインし、同意できるようにブラウザーで開く必要があります。</span><span class="sxs-lookup"><span data-stu-id="9053e-p106">You request an authorization code by sending a GET request to the Azure AD v2.0 endpoint. This URL must be opened in a browser so that the user can sign in and provide consent.</span></span>

#### <a name="construct-the-request"></a><span data-ttu-id="9053e-123">要求の構築</span><span class="sxs-lookup"><span data-stu-id="9053e-123">Construct the request</span></span>

<span data-ttu-id="9053e-124">1- ベース URL から起動します。</span><span class="sxs-lookup"><span data-stu-id="9053e-124">1- Start with the base URL:</span></span>

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

<span data-ttu-id="9053e-p107">パス内の *tenant* セグメントは、アプリケーションにサインインできるユーザーを制御します。使用できる値は、*common*、*organizations*、*consumers*、および tenant の各識別子です。詳細については、「[プロトコル エンドポイント](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9053e-p107">The *tenant* segment in the path controls who can sign into the application. Allowed values are *common*, *organizations*, *consumers*, and tenant identifiers. For more information, see [Protocol endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span></span>

<span data-ttu-id="9053e-p108">2- ベース URL にクエリ パラメーターを追加します。これらは、アプリ、要求されたアクセス許可、および他の認証要求情報を識別するために使用されます。次の表に、いくつかの一般的なパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="9053e-p108">2- Append query parameters to the base URL. These are used to identify the app, the requested permissions, and other auth request information. The following table describes some common parameters.</span></span>

| <span data-ttu-id="9053e-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9053e-131">Parameter</span></span> | <span data-ttu-id="9053e-132">説明</span><span class="sxs-lookup"><span data-stu-id="9053e-132">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="9053e-133">client_id</span><span class="sxs-lookup"><span data-stu-id="9053e-133">client_id</span></span> | <span data-ttu-id="9053e-p109">アプリを登録すると生成されるアプリ ID です。これにより、どのアプリがログオンを要求しているかが Azure AD に通知されます。</span><span class="sxs-lookup"><span data-stu-id="9053e-p109">The app ID generated by registering the app. This lets Azure AD know which app is requesting the logon.</span></span> |
| <span data-ttu-id="9053e-136">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="9053e-136">redirect_uri</span></span> | <span data-ttu-id="9053e-p110">ユーザーがアプリに同意した後、Azure によってリダイレクトされる場所です。この値は、アプリを登録したときに使用された**リダイレクト URI** の値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="9053e-p110">The location that Azure will redirect to after the user has granted consent to the app. This value must correspond to the value of **Redirect URI** used when registering the app.</span></span> |
| <span data-ttu-id="9053e-139">response_type</span><span class="sxs-lookup"><span data-stu-id="9053e-139">response_type</span></span> | <span data-ttu-id="9053e-p111">アプリが想定している応答タイプです。この値は、認証コードの付与フローの `code` です。</span><span class="sxs-lookup"><span data-stu-id="9053e-p111">The type of response the app is expecting. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="9053e-142">scope</span><span class="sxs-lookup"><span data-stu-id="9053e-142">scope</span></span> | <span data-ttu-id="9053e-p112">アプリが要求している [Microsoft Graph のアクセス許可スコープ](./permissions_reference.md)をスペースで区切った一覧です。[シングル サインオン](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/)に対して [OpenId Connect スコープ](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes)を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="9053e-p112">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting. You can also specify [OpenId Connect scopes](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) for [single sign-on](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span></span>  |
| <span data-ttu-id="9053e-145">state</span><span class="sxs-lookup"><span data-stu-id="9053e-145">state</span></span> | <span data-ttu-id="9053e-146">トークン応答でも返され、検証に使用される要求に含まれている値です。</span><span class="sxs-lookup"><span data-stu-id="9053e-146">A value included in the request that will also be returned in the token response, used for validation.</span></span> |

<span data-ttu-id="9053e-147">たとえば、電子メールへの読み取りアクセスを要求するアプリケーションの要求 URL は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9053e-147">For example, the request URL for an application that requires read access to mail might look like the following.</span></span>

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

<span data-ttu-id="9053e-p113">3- ユーザーをログオン URL にリダイレクトします。ユーザーには、アプリ名が表示されているサインイン画面が表示されます。サインインすると、アプリが必要とするアクセス許可の一覧が表示され、許可するか拒否するかの確認を求められます。同意すると、ブラウザーは認証コードでリダイレクト URL にリダイレクトされ、次の例に示すように、クエリ文字列に認証コードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9053e-p113">3- Redirect the user to the logon URL. The user is presented with a sign in screen that displays the name of the app. After signing in, the user is presented with the list of the permissions the app requires and prompted to allow or deny. If the user consents, the browser redirects to the redirect URI with the authorization code and state in the query string, as shown in the following example.</span></span>

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

<span data-ttu-id="9053e-152">次の手順では、返された認証コードをアクセス トークンと交換します。</span><span class="sxs-lookup"><span data-stu-id="9053e-152">The next step is to exchange the authorization code returned for an access token.</span></span>

### <a name="getting-an-access-token"></a><span data-ttu-id="9053e-153">アクセス トークンの取得</span><span class="sxs-lookup"><span data-stu-id="9053e-153">Getting an access token</span></span>

<span data-ttu-id="9053e-154">アクセス トークンを取得するため、アプリはフォームでエンコードされたパラメーターに以下のパラメーターを付けてトークン要求 URL (例: `https://login.microsoftonline.com/common/oauth2/v2.0/token`) にポストします。</span><span class="sxs-lookup"><span data-stu-id="9053e-154">To get an access token, the app posts form-encoded parameters to the token request URL (for example, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) with the following parameters.</span></span>

| <span data-ttu-id="9053e-155">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9053e-155">Parameter</span></span> | <span data-ttu-id="9053e-156">説明</span><span class="sxs-lookup"><span data-stu-id="9053e-156">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="9053e-157">client_id</span><span class="sxs-lookup"><span data-stu-id="9053e-157">client_id</span></span> | <span data-ttu-id="9053e-158">アプリを登録すると生成されるアプリ ID です。</span><span class="sxs-lookup"><span data-stu-id="9053e-158">The app ID generated by registering the app.</span></span> |
| <span data-ttu-id="9053e-159">client_secret</span><span class="sxs-lookup"><span data-stu-id="9053e-159">client_secret</span></span> | <span data-ttu-id="9053e-160">アプリを登録するときに生成されるアプリ シークレットです。</span><span class="sxs-lookup"><span data-stu-id="9053e-160">The app secret generated when registering the app.</span></span> |
| <span data-ttu-id="9053e-161">code</span><span class="sxs-lookup"><span data-stu-id="9053e-161">code</span></span> | <span data-ttu-id="9053e-162">前の手順で取得した認証コードです。</span><span class="sxs-lookup"><span data-stu-id="9053e-162">The authorization code obtained in the prior step.</span></span> |
| <span data-ttu-id="9053e-163">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="9053e-163">redirect_uri</span></span> | <span data-ttu-id="9053e-164">この値は、認証コード要求で使用した値と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9053e-164">This value must be the same as the value used in the authorization code request.</span></span> |
| <span data-ttu-id="9053e-165">grant_type</span><span class="sxs-lookup"><span data-stu-id="9053e-165">grant_type</span></span> | <span data-ttu-id="9053e-p114">アプリが使用している付与の種類です。この値は、認証コードの付与フローの `code` です。</span><span class="sxs-lookup"><span data-stu-id="9053e-p114">The type of grant the app is using. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="9053e-168">scope</span><span class="sxs-lookup"><span data-stu-id="9053e-168">scope</span></span> | <span data-ttu-id="9053e-169">アプリが要求している [Microsoft Graph のアクセス許可スコープ](./permissions_reference.md)をスペースで区切った一覧です。</span><span class="sxs-lookup"><span data-stu-id="9053e-169">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting.</span></span> |

<span data-ttu-id="9053e-170">前の手順のコードを使用する、アプリケーションの要求 URL は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9053e-170">The request URL for our application, using the code from the previous step, looks like the following.</span></span>

```
POST https://login.microsoftonline.com/common/oauth2/v2.0/token
Content-Type: application/x-www-form-urlencoded

{
  grant_type=authorization_code
  &code=AwABAAAA...cZZ6IgAA
  &redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
  &resource=https%3A%2F%2Fgraph.microsoft.com%2F
  &scope=mail.read
  &client\_id=<app ID>
  &client\_secret=<app SECRET>
}
```

<span data-ttu-id="9053e-171">サーバーはアクセス トークンを含む JSON ペイロードで応答します。</span><span class="sxs-lookup"><span data-stu-id="9053e-171">The server responds with a JSON payload which includes the access token.</span></span>

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "token_type":"Bearer",
  "expires_in":"3600",
  "access_token":"eyJ0eXAi...b66LoPVA",
  "scope":"https://graph.microsoft.com/mail.read",
  ...
}
```

<span data-ttu-id="9053e-p115">アクセス トークンは JSON ペイロードの `access_token` フィールドにあります。アプリが API に REST 呼び出しを行うときに、アプリはこの値を認証ヘッダーの設定で使用します。</span><span class="sxs-lookup"><span data-stu-id="9053e-p115">The access token is found in the `access_token` field of the JSON payload. The app uses this value to set the Authorization header when making REST calls to the API.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="9053e-174">Microsoft Graph を呼び出す</span><span class="sxs-lookup"><span data-stu-id="9053e-174">Call Microsoft Graph</span></span>

<span data-ttu-id="9053e-p116">アクセス トークンを取得すると、Microsoft Graph を呼び出す準備ができます。このサンプル アプリはメッセージを取得するため、`https://graph.microsoft.com/v1.0/me/messages` エンドポイントに対する HTTP GET 要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="9053e-p116">After the app has an access token, it's ready to call Microsoft Graph. Because this sample app is retrieving messages, it will use an HTTP GET request to the `https://graph.microsoft.com/v1.0/me/messages` endpoint.</span></span>

### <a name="refine-the-request"></a><span data-ttu-id="9053e-177">要求を絞り込む</span><span class="sxs-lookup"><span data-stu-id="9053e-177">Refine the request</span></span>

<span data-ttu-id="9053e-p117">アプリでは、OData クエリ パラメーターを使用して GET 要求の動作を制御できます。アプリがこれらのパラメーターを使用して返される結果の数と、各項目に返されるフィールドの数を制限することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9053e-p117">Apps can control the behavior of GET requests by using OData query parameters. We recommend that apps use these parameters to limit the number of results that are returned and to limit the fields that are returned for each item.</span></span> 

<span data-ttu-id="9053e-p118">サンプル アプリでは、表にメッセージの件名、送信者、メッセージを受信した日時が表示されます。表には最大 25 行が表示され、最新の受信メッセージが上位にくるように並べ替えられます。アプリでは、次のクエリ パラメーターを使用してこれらの結果を取得します。</span><span class="sxs-lookup"><span data-stu-id="9053e-p118">This sample app will display messages in a table that shows the subject, sender, and the date and time the message was received. The table displays a maximum of 25 rows and is sorted so that the most recently received message is at the top. The app uses the following query parameters to get these results.</span></span>

- <span data-ttu-id="9053e-183">`$select` - `subject`、`sender`、および `dateTimeReceived` の各フィールドのみを指定します。</span><span class="sxs-lookup"><span data-stu-id="9053e-183">`$select` - Specifies only the `subject`, `sender`, and `dateTimeReceived` fields.</span></span>
- <span data-ttu-id="9053e-184">`$top` -最大で 25 項目を指定します。</span><span class="sxs-lookup"><span data-stu-id="9053e-184">`$top` - Specifies a maximum of 25 items.</span></span>
- <span data-ttu-id="9053e-185">`$orderby` - `dateTimeReceived` フィールドに基づいて結果を並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="9053e-185">`$orderby` - Sorts the results by the `dateTimeReceived` field.</span></span>

<span data-ttu-id="9053e-186">これにより、次の要求が行われます。</span><span class="sxs-lookup"><span data-stu-id="9053e-186">This results in the following request.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

<span data-ttu-id="9053e-p119">これで、Microsoft Graph を呼び出す方法が理解できたため、API リファレンスを使用して、アプリで必要なその他の呼び出しを作成することができます。ただしアプリでは、呼び出しを行うための適切なアクセス許可をアプリ登録で設定する必要がある点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="9053e-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9053e-189">次の手順</span><span class="sxs-lookup"><span data-stu-id="9053e-189">Next steps</span></span>
- <span data-ttu-id="9053e-190">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用してさらに REST API を試してみる。</span><span class="sxs-lookup"><span data-stu-id="9053e-190">Try out more of the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="9053e-191">関連項目</span><span class="sxs-lookup"><span data-stu-id="9053e-191">See also</span></span>
- [<span data-ttu-id="9053e-192">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="9053e-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="9053e-193">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="9053e-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
