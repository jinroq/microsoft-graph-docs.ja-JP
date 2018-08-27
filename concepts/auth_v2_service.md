# <a name="get-access-without-a-user"></a><span data-ttu-id="e7645-101">ユーザーなしでアクセスを取得</span><span class="sxs-lookup"><span data-stu-id="e7645-101">Get access without a user</span></span>

<span data-ttu-id="e7645-p101">一部のアプリでは、ユーザーの代わりに独自の ID を使用して Microsoft Graph を呼び出します。多くの場合、これらは、サインインしたユーザーが存在しないサーバー上で実行される、バックグラウンド サービスかデーモンです。この種のアプリの例として、夜間に起動して実行される電子メール アーカイブ サービスがあります。場合によっては、サインインしているユーザーが存在するアプリでも、独自の ID で Microsoft Graph を呼び出す必要があります。たとえば、サインインしたユーザーが所有している組織内の特権よりも高い特権を必要とする機能をアプリが使用する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7645-p101">Some apps call Microsoft Graph with their own identity and not on behalf of a user. In many cases, these are background services or daemons that run on a server without the presence of a signed-in user. An example of such an app might be an email archival service that wakes up and runs overnight. In some cases, apps that have a signed-in user present may also need to call Microsoft Graph under their own identity. For example, an app may need to use functionality that requires more elevated privileges in an organization than those carried by the signed-in user.</span></span>  

<span data-ttu-id="e7645-p102">独自の ID で Microsoft Graph を呼び出すアプリは、OAuth 2.0 クライアント資格情報の付与フローを使用して、Azure AD からアクセス トークンを取得します。このトピックでは、サービスを構成し、OAuth クライアント資格情報の付与フローを使用して、アクセス トークンを取得する基本的な手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7645-p102">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 client credentials grant flow to get access tokens from Azure AD. In this topic, we will walk through the basic steps to configure a service and use the OAuth client credentials grant flow to get an access token.</span></span> 

## <a name="authentication-and-authorization-steps"></a><span data-ttu-id="e7645-109">認証および承認の手順</span><span class="sxs-lookup"><span data-stu-id="e7645-109">Authentication and authorization steps</span></span>

<span data-ttu-id="e7645-110">サービスを構成し、サービスが独自の ID で Microsoft Graph を呼び出すために使用できる Azure AD v2.0 エンドポイントからトークンを取得するために必要となる、基本的な手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e7645-110">The basic steps required to configure a service and get a token from the Azure AD v2.0 endpoint that your service can use to call Microsoft Graph under its own identity are:</span></span>

1. <span data-ttu-id="e7645-111">アプリを登録する。</span><span class="sxs-lookup"><span data-stu-id="e7645-111">Register your app.</span></span>
2. <span data-ttu-id="e7645-112">アプリで Microsoft Graph のアクセス許可を構成する。</span><span class="sxs-lookup"><span data-stu-id="e7645-112">Configure permissions for Microsoft Graph on your app.</span></span>
3. <span data-ttu-id="e7645-113">管理者の同意を取得する。</span><span class="sxs-lookup"><span data-stu-id="e7645-113">Get administrator consent.</span></span>
4. <span data-ttu-id="e7645-114">アクセス トークンを取得する。</span><span class="sxs-lookup"><span data-stu-id="e7645-114">Get an access token.</span></span>
5. <span data-ttu-id="e7645-115">アクセス トークンを使用して、Microsoft Graph を呼び出す。</span><span class="sxs-lookup"><span data-stu-id="e7645-115">Use the access token to call Microsoft Graph.</span></span>

## <a name="1-register-your-app"></a><span data-ttu-id="e7645-116">1.アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="e7645-116">1. Register your app</span></span>

<span data-ttu-id="e7645-p103">Azure v2.0 エンドポイントで認証するには、まずアプリを [Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/) で登録する必要があります。アプリを登録するには、Microsoft アカウントのほか、職場または学校のアカウントを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p103">To authenticate with the Azure v2.0 endpoint, you must first register your app at the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/). You can use either a Microsoft account or a work or school account to register your app.</span></span> 

<span data-ttu-id="e7645-p104">次のスクリーンショットは、バックグラウンド サービス用に構成された Web アプリの登録を示しています。![サービス アプリの登録](./images/v2-service-registration.png)</span><span class="sxs-lookup"><span data-stu-id="e7645-p104">The following screenshot shows a web app registration that has been configured for a background service. ![Service app registration](./images/v2-service-registration.png)</span></span>

<span data-ttu-id="e7645-121">独自の ID で Microsoft Graph を呼び出すサービスの場合は、Web プラットフォーム用のアプリを登録して、次の値をコピーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7645-121">For a service that will call Microsoft Graph under its own identity, you need to register your app for the Web platform and copy the following values:</span></span>

- <span data-ttu-id="e7645-122">アプリ登録ポータルによって割り当てられたアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="e7645-122">The Application ID assigned by the app registration portal.</span></span>
- <span data-ttu-id="e7645-123">アプリケーション シークレット。パスワードか、公開鍵/秘密鍵のペア (証明書) のいずれか。</span><span class="sxs-lookup"><span data-stu-id="e7645-123">An Application Secret, either a password or a public/private key pair (certificate).</span></span>
- <span data-ttu-id="e7645-124">Azure AD からトークンの応答を受け取るためのサービスのリダイレクト URL。</span><span class="sxs-lookup"><span data-stu-id="e7645-124">A Redirect URL for your service to receive token responses from Azure AD.</span></span>
- <span data-ttu-id="e7645-125">アプリに管理者の同意を要求する機能が実装されている場合は、サービスが管理者の同意の応答を受信するためのリダイレクト URL。</span><span class="sxs-lookup"><span data-stu-id="e7645-125">A Redirect URL for your service to receive admin consent responses if your app implements functionality to request administrator consent.</span></span>  

<span data-ttu-id="e7645-126">Microsoft アプリ登録ポータルを使用してアプリを構成する手順については、「[アプリを登録する](./auth_register_app_v2.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-126">For steps on how to configure an app using the Microsoft App Registration Portal, see [Register your app](./auth_register_app_v2.md).</span></span>

<span data-ttu-id="e7645-127">OAuth 2.0 クライアント資格情報の付与フローでは、Azure AD によって割り当てられたアプリケーション ID と、ポータルを使用して作成したアプリケーション シークレットを使用して、アプリが Azure AD v2.0 `/token` エンドポイントで直接認証されます。</span><span class="sxs-lookup"><span data-stu-id="e7645-127">With the OAuth 2.0 client credentials grant flow, your app authenticates directly at the Azure AD v2.0 `/token` endpoint using the Application ID assigned by Azure AD and the Application Secret that you create using the portal.</span></span> 

## <a name="2-configure-permissions-for-microsoft-graph"></a><span data-ttu-id="e7645-128">2.Microsoft Graph のアクセス許可を構成する</span><span class="sxs-lookup"><span data-stu-id="e7645-128">2. Configure permissions for Microsoft Graph</span></span>

<span data-ttu-id="e7645-p105">独自の ID で Microsoft Graph を呼び出すアプリの場合、Microsoft Graph はアプリケーションのアクセス許可を公開します。(Microsoft Graph は、ユーザーに代わって Microsoft Graph を呼び出すアプリの委任されたアクセス許可も公開します。)アプリに必要なアプリケーションのアクセス許可は、アプリを登録する時点で事前に構成します。アプリケーションのアクセス許可には常に管理者の同意が必要です。管理者は、組織にアプリがインストールされるときに [Azure ポータル](https://portal.azure.com)を使用してこれらのアクセス許可に同意するか、構成済みのアクセス許可に管理者が同意することによりアプリでサインアップ エクスペリエンスを提供することができます。管理者の同意が Azure AD によって記録されると、アプリは再度同意を要求する必要なしにトークンを要求できます。Microsoft Graph で使用できるアクセス許可の詳細については、「[アクセス許可のリファレンス](./permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-p105">For apps that call Microsoft Graph under their own identity, Microsoft Graph exposes application permissions. (Microsoft Graph also exposes delegated permissions for apps that call Microsoft Graph on behalf of a user.) You pre-configure the application permissions your app needs when you register your app. Application permissions always require administrator consent. An administrator can either consent to these permissions using the [Azure portal](https://portal.azure.com) when your app is installed in their organization, or you can provide a sign-up experience in your app through which administrators can consent to the permissions you configured. Once administrator consent is recorded by Azure AD, your app can request tokens without having to request consent again. For more detailed information about the permissions available with Microsoft Graph, see the [Permissions reference](./permissions_reference.md)</span></span>

<span data-ttu-id="e7645-135">[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)でアプリのアプリケーション アクセス許可を構成するには、**[Microsoft Graph]** の下で **[アプリケーションのアクセス許可]** の隣にある **[追加]** を選択し、**[アクセス許可の選択]** ダイアログでアプリに必要なアクセス許可を選択します。</span><span class="sxs-lookup"><span data-stu-id="e7645-135">To configure application permissions for your app in the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/): under **Microsoft Graph**, choose **Add** next to **Application Permissions** and then select the permissions your app requires in the **Select Permissions** dialog.</span></span>

<span data-ttu-id="e7645-136">次のスクリーンショットは、Microsoft Graph のアプリケーションのアクセス許可に対する **[アクセス許可の選択]** ダイアログを示しています。</span><span class="sxs-lookup"><span data-stu-id="e7645-136">The following screenshot shows the **Select Permissions** dialog for Microsoft Graph application permissions.</span></span> 

![Microsoft Graph のアプリケーションのアクセス許可に対する [アクセス許可の選択] ダイアログ。](./images/v2-application-permissions.png)

> <span data-ttu-id="e7645-p106">**注**:アプリで必要になるアクセス許可の、最低限の権限セットを構成することをお勧めします。これにより、アクセス許可の長大なリストに同意を求めるものよりも快適なエクスペリエンスを管理者に提供できます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p106">**Note**: We recommend configuring the least privileged set of permissions required by your app. This provides a much more comfortable experience for administrators than having to consent to a long list of permissions.</span></span>

## <a name="3-get-administrator-consent"></a><span data-ttu-id="e7645-140">3.管理者の同意を取得する</span><span class="sxs-lookup"><span data-stu-id="e7645-140">3. Get administrator consent</span></span>

<span data-ttu-id="e7645-141">管理者に任せて [Azure ポータル](https://portal.azure.com)でアプリケーションに必要なアクセス許可を付与することができます。ただし、多くの場合、Azure AD v2.0 `/adminconsent` エンドポイントを使用して管理者にサインアップ エクスペリエンスを提供するほうが優れた選択肢になります。</span><span class="sxs-lookup"><span data-stu-id="e7645-141">You can rely on an administrator to grant the permissions your app needs at the [Azure portal](https://portal.azure.com); however, often, a better option is to provide a sign-up experience for administrators by using the Azure AD v2.0 `/adminconsent` endpoint.</span></span> 

> <span data-ttu-id="e7645-142">**重要**:構成済みのアクセス許可に変更を加える場合は常に、管理者の同意プロセスも繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7645-142">**Important**: Any time you make a change to the configured permissions, you must also repeat the Admin Consent process.</span></span> <span data-ttu-id="e7645-143">アプリ登録ポータルで行われた変更は、テナント管理者が同意を再適用するまで反映されません。</span><span class="sxs-lookup"><span data-stu-id="e7645-143">Changes made in the app registration portal will not be reflected until consent has been reapplied by the tenant's administrator.</span></span>

### <a name="request"></a><span data-ttu-id="e7645-144">要求</span><span class="sxs-lookup"><span data-stu-id="e7645-144">Request</span></span>

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=http://localhost/myapp/permissions
```

| <span data-ttu-id="e7645-145">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7645-145">Parameter</span></span>     | <span data-ttu-id="e7645-146">条件</span><span class="sxs-lookup"><span data-stu-id="e7645-146">Condition</span></span>   | <span data-ttu-id="e7645-147">説明</span><span class="sxs-lookup"><span data-stu-id="e7645-147">Description</span></span> 
|:--------------|:------------|:------------
| <span data-ttu-id="e7645-148">テナント</span><span class="sxs-lookup"><span data-stu-id="e7645-148">tenant</span></span>        | <span data-ttu-id="e7645-149">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-149">Required</span></span>    | <span data-ttu-id="e7645-p108">アクセス許可の要求元のディレクトリ テナント。これは、GUID またはフレンドリ名の形式で指定できます。ユーザーが所属しているテナントがわからないときに、そのユーザーを任意のテナントでサインインさせる場合は、`common` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e7645-p108">The directory tenant that you want to request permission from. This can be in GUID or friendly name format. If you don't know which tenant the user belongs to and you want to let them sign in with any tenant, use `common`.</span></span> 
| <span data-ttu-id="e7645-153">client_id</span><span class="sxs-lookup"><span data-stu-id="e7645-153">client_id</span></span>     | <span data-ttu-id="e7645-154">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-154">Required</span></span>    | <span data-ttu-id="e7645-155">[アプリケーション登録ポータル](https://apps.dev.microsoft.com/)でアプリに割り当てられたアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="e7645-155">The Application ID that the [Application Registration Portal](https://apps.dev.microsoft.com/) assigned to your app.</span></span> 
| <span data-ttu-id="e7645-156">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="e7645-156">redirect_uri</span></span>  | <span data-ttu-id="e7645-157">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-157">Required</span></span>    | <span data-ttu-id="e7645-p109">アプリが処理するために応答を送信するリダイレクト URI。URL でエンコードされている必要があることを除き、ポータルに登録したリダイレクト URI のいずれかに完全に一致する必要があります。また追加のパス セグメントを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p109">The redirect URI where you want the response to be sent for your app to handle. It must exactly match one of the redirect URIs that you registered in the portal, except that it must be URL encoded, and it can have additional path segments.</span></span> 
| <span data-ttu-id="e7645-160">ステート</span><span class="sxs-lookup"><span data-stu-id="e7645-160">state</span></span>         | <span data-ttu-id="e7645-161">推奨</span><span class="sxs-lookup"><span data-stu-id="e7645-161">Recommended</span></span> | <span data-ttu-id="e7645-p110">トークン応答でも返される、要求に含まれている値。任意のコンテンツの文字列にすることができます。state は、使用していたページまたはビューなど、認証要求が発生する前の、アプリでのユーザーの状態に関する情報をエンコードするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p110">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span> 

### <a name="administrator-consent-experience"></a><span data-ttu-id="e7645-165">管理者の同意エクスペリエンス</span><span class="sxs-lookup"><span data-stu-id="e7645-165">Administrator consent experience</span></span>

<span data-ttu-id="e7645-p111">エンドポイントへの要求では、Azure AD はテナント管理者のみがサインインして要求を完了できるように強制します。管理者は、アプリ登録ポータルでユーザーがアプリに対して要求したすべてのアプリケーションのアクセス許可を承認するよう求められます。`/adminconsent`</span><span class="sxs-lookup"><span data-stu-id="e7645-p111">With requests to the `/adminconsent` endpoint, Azure AD enforces that only a tenant administrator can sign in to complete the request. The administrator will be asked to approve all the application permissions that you have requested for your app in the app registration portal.</span></span> 

<span data-ttu-id="e7645-168">Azure AD が管理者に提示する同意ダイアログの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7645-168">The following is an example of the consent dialog that Azure AD presents to the administrator:</span></span>

![管理者の同意ダイアログ。](./images/admin-consent.png)

### <a name="response"></a><span data-ttu-id="e7645-170">応答</span><span class="sxs-lookup"><span data-stu-id="e7645-170">Response</span></span>

<span data-ttu-id="e7645-171">管理者がアプリケーションのアクセス許可を承認した場合、成功応答は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="e7645-171">If the administrator approves the permissions for your application, the successful response looks like this:</span></span>

```
// Line breaks are for legibility only.

GET http://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| <span data-ttu-id="e7645-172">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7645-172">Parameter</span></span>     | <span data-ttu-id="e7645-173">説明</span><span class="sxs-lookup"><span data-stu-id="e7645-173">Description</span></span> 
|:--------------|:------------
| <span data-ttu-id="e7645-174">テナント</span><span class="sxs-lookup"><span data-stu-id="e7645-174">tenant</span></span>        | <span data-ttu-id="e7645-175">要求されたアクセス許可をアプリケーションに付与したディレクトリ テナント (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="e7645-175">The directory tenant that granted your application the permissions that it requested, in GUID format.</span></span> 
| <span data-ttu-id="e7645-176">状態</span><span class="sxs-lookup"><span data-stu-id="e7645-176">state</span></span>         | <span data-ttu-id="e7645-p112">トークン応答でも返される、要求に含まれている値。任意のコンテンツの文字列にすることができます。state は、使用していたページまたはビューなど、認証要求が発生する前の、アプリでのユーザーの状態に関する情報をエンコードするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p112">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span> 
| <span data-ttu-id="e7645-180">admin_consent</span><span class="sxs-lookup"><span data-stu-id="e7645-180">admin_consent</span></span> | <span data-ttu-id="e7645-181">**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="e7645-181">Set to **true**.</span></span> 


> <span data-ttu-id="e7645-p113">**お試しください**:次の要求をブラウザーに貼り付けて、これを試してみることができます。Azure AD テナントのグローバル管理者としてサインインすると、アプリの管理者の同意ダイアログ ボックスが表示されます。(これは、前述の同意ダイアログ ボックスのスクリーンショットのアプリとは別のアプリになります。)</span><span class="sxs-lookup"><span data-stu-id="e7645-p113">**Try**: You can try this for yourself by pasting the following request in a browser. If you sign in as a Global administrator for an Azure AD tenant, you will be presented with the administrator consent dialog box for the app. (This will be a different app than that in the consent dialog box screenshot shown earlier.)</span></span>
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=http://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a><span data-ttu-id="e7645-185">4. アクセス トークンを取得する</span><span class="sxs-lookup"><span data-stu-id="e7645-185">4. Get an access token</span></span>

<span data-ttu-id="e7645-186">OAuth 2.0 クライアント資格情報の付与フローでは、アプリの登録時に保存したアプリケーション ID とアプリケーション シークレットの値を使用して、Azure AD v2.0 `/token` エンドポイントからアクセス トークンを直接要求します。</span><span class="sxs-lookup"><span data-stu-id="e7645-186">In the OAuth 2.0 client credentials grant flow, you use the Application ID and Application Secret values that you saved when you registered your app to request an access token directly from the Azure AD v2.0 `/token` endpoint.</span></span>

<span data-ttu-id="e7645-p114">トークン要求の `scope` パラメーターの値として `https://graph.microsoft.com/.default` を渡すことにより、事前構成済みのアクセス許可を指定します。詳細については、次のトークン要求の `scope` パラメーターの説明を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-p114">You specify the pre-configured permissions by passing `https://graph.microsoft.com/.default` as the value for the `scope` parameter in the token request. See the `scope` parameter description in the token request below for details.</span></span>

### <a name="token-request"></a><span data-ttu-id="e7645-189">トークン要求</span><span class="sxs-lookup"><span data-stu-id="e7645-189">Token request</span></span>

<span data-ttu-id="e7645-190">POST 要求を `/token` v2.0 エンドポイントに送信して、アクセス トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="e7645-190">You send a POST request to the `/token` v2.0 endpoint to acquire an access token:</span></span>

```
// Line breaks are for legibility only.

POST /{tenant}/oauth2/v2.0/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=535fb089-9ff3-47b6-9bfb-4f1264799865
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default
&client_secret=qWgdYAmab0YSkuL1qKv5bPX
&grant_type=client_credentials
```

| <span data-ttu-id="e7645-191">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7645-191">Parameter</span></span>     | <span data-ttu-id="e7645-192">条件</span><span class="sxs-lookup"><span data-stu-id="e7645-192">Condition</span></span> | <span data-ttu-id="e7645-193">説明</span><span class="sxs-lookup"><span data-stu-id="e7645-193">Description</span></span> 
|:--------------|:----------|:------------
| <span data-ttu-id="e7645-194">テナント</span><span class="sxs-lookup"><span data-stu-id="e7645-194">tenant</span></span>        | <span data-ttu-id="e7645-195">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-195">Required</span></span>  | <span data-ttu-id="e7645-p115">アクセス許可の要求元のディレクトリ テナント。これは、GUID またはフレンドリ名の形式で指定できます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p115">The directory tenant that you want to request permission from. This can be in GUID or friendly name format.</span></span> 
| <span data-ttu-id="e7645-198">client_id</span><span class="sxs-lookup"><span data-stu-id="e7645-198">client_id</span></span>     | <span data-ttu-id="e7645-199">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-199">Required</span></span>  | <span data-ttu-id="e7645-200">アプリの登録時に [Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com)が割り当てたアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="e7645-200">The Application ID that the [Microsoft App Registration Portal](https://apps.dev.microsoft.com) assigned when you registered your app.</span></span> 
| <span data-ttu-id="e7645-201">scope</span><span class="sxs-lookup"><span data-stu-id="e7645-201">scope</span></span>         | <span data-ttu-id="e7645-202">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-202">Required</span></span>  | <span data-ttu-id="e7645-p116">この要求で `scope` パラメーターに渡される値は、必要なリソースのリソース識別子 (アプリケーション ID の URI) である必要があります (`.default` サフィックス付き)。Microsoft Graph の場合、値は `https://graph.microsoft.com/.default` です。この値は、アプリに構成したすべてのアプリケーションのアクセス許可のうち、使用するリソースに関連付けられたアクセス許可のトークンを発行するように v2.0 エンドポイントに通知します。</span><span class="sxs-lookup"><span data-stu-id="e7645-p116">The value passed for the `scope` parameter in this request should be the resource identifier (Application ID URI) of the resource you want, affixed with the `.default` suffix. For Microsoft Graph, the value is `https://graph.microsoft.com/.default`. This value informs the v2.0 endpoint that of all the application permissions you have configured for your app, it should issue a token for the ones associated with the resource you want to use.</span></span> 
| <span data-ttu-id="e7645-206">client_secret</span><span class="sxs-lookup"><span data-stu-id="e7645-206">client_secret</span></span> | <span data-ttu-id="e7645-207">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-207">Required</span></span>  | <span data-ttu-id="e7645-208">アプリケーション登録ポータルでアプリ用に生成したアプリケーション シークレット。</span><span class="sxs-lookup"><span data-stu-id="e7645-208">The Application Secret that you generated for your app in the app registration portal.</span></span> 
| <span data-ttu-id="e7645-209">grant_type</span><span class="sxs-lookup"><span data-stu-id="e7645-209">grant_type</span></span>    | <span data-ttu-id="e7645-210">必須</span><span class="sxs-lookup"><span data-stu-id="e7645-210">Required</span></span>  | <span data-ttu-id="e7645-211">である必要があります。`client_credentials`</span><span class="sxs-lookup"><span data-stu-id="e7645-211">Must be `client_credentials`.</span></span> 

#### <a name="token-response"></a><span data-ttu-id="e7645-212">トークンの応答</span><span class="sxs-lookup"><span data-stu-id="e7645-212">Token response</span></span>

<span data-ttu-id="e7645-213">成功応答は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="e7645-213">A successful response looks like this:</span></span>

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| <span data-ttu-id="e7645-214">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7645-214">Parameter</span></span>     | <span data-ttu-id="e7645-215">説明</span><span class="sxs-lookup"><span data-stu-id="e7645-215">Description</span></span> 
|:--------------|:------------
| <span data-ttu-id="e7645-216">access_token</span><span class="sxs-lookup"><span data-stu-id="e7645-216">access_token</span></span>  | <span data-ttu-id="e7645-p117">要求されたアクセス トークン。アプリはこのトークンを Microsoft Graph の呼び出しで使用できます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p117">The requested access token. Your app can use this token in calls to Microsoft Graph.</span></span> 
| <span data-ttu-id="e7645-219">token_type</span><span class="sxs-lookup"><span data-stu-id="e7645-219">token_type</span></span>    | <span data-ttu-id="e7645-p118">トークンの種類の値を示します。Azure AD がサポートしている種類は `bearer` のみです。</span><span class="sxs-lookup"><span data-stu-id="e7645-p118">Indicates the token type value. The only type that Azure AD supports is `bearer`.</span></span> 
| <span data-ttu-id="e7645-222">expires_in</span><span class="sxs-lookup"><span data-stu-id="e7645-222">expires_in</span></span>    | <span data-ttu-id="e7645-223">アクセス トークンの有効期間 (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="e7645-223">How long the access token is valid (in seconds).</span></span> 

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a><span data-ttu-id="e7645-224">5.アクセス トークンを使用して、Microsoft Graph を呼び出す</span><span class="sxs-lookup"><span data-stu-id="e7645-224">5. Use the access token to call Microsoft Graph</span></span>

<span data-ttu-id="e7645-p119">アクセス トークンの取得後は、そのトークンを使用して (トークンを要求の `Authorization` ヘッダーに含める)、Microsoft Graph を呼び出すことができます。次の要求は、特定のユーザーのプロファイルを取得します。この API を呼び出すには、アプリに _User.Read.All_ アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7645-p119">After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of a specific user. Your app must have the _User.Read.All_ permission to call this API.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f 
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
<span data-ttu-id="e7645-228">正常な応答は次のようになります (一部の応答ヘッダーは削除されています)。</span><span class="sxs-lookup"><span data-stu-id="e7645-228">A successful response will look similar to this (some response headers have been removed):</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 309.0273
Date: Wed, 26 Apr 2017 19:53:49 GMT
Content-Length: 407
```

```json
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="supported-app-scenarios-and-resources"></a><span data-ttu-id="e7645-229">サポートされているアプリのシナリオとリソース</span><span class="sxs-lookup"><span data-stu-id="e7645-229">Supported app scenarios and resources</span></span>

<span data-ttu-id="e7645-230">独自の ID で Microsoft Graph を呼び出すアプリは、次に示す 2 つのカテゴリのいずれかに分類されます。</span><span class="sxs-lookup"><span data-stu-id="e7645-230">Apps that call Microsoft Graph under their own identity fall into one of two categories:</span></span>

- <span data-ttu-id="e7645-231">サインインしたユーザーが存在しないサーバーで実行されるバックグラウンド サービス (デーモン)。</span><span class="sxs-lookup"><span data-stu-id="e7645-231">Background services (daemons) that run on a server without a signed-in user.</span></span>
- <span data-ttu-id="e7645-232">サインインしたユーザーは存在するが、独自の ID でも Microsoft Graph を呼び出すアプリ (たとえば、ユーザーの特権よりも高い特権を必要とする機能を使用するため)。</span><span class="sxs-lookup"><span data-stu-id="e7645-232">Apps that have a signed-in user but also call Microsoft Graph with their own identity; for example, to use functionality that requires more elevated privileges than those of the user.</span></span>

<span data-ttu-id="e7645-p120">独自の ID で Microsoft Graph を呼び出すアプリは、OAuth 2.0 クライアント資格情報の付与を使用して Azure AD で認証し、トークンを取得します。v2.0 エンドポイントの場合は、次のリソースを使用して、このシナリオについてさらに詳しく調べることができます。</span><span class="sxs-lookup"><span data-stu-id="e7645-p120">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 client credentials grant to authenticate with Azure AD and get a token. For the v2.0 endpoint, you can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="e7645-235">エラーへの対応を含む、クライアント資格情報の付与フローの完全な処理については、「[Azure Active Directory v2.0 と OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-235">For a more complete treatment of the client credentials grant flow that also includes error responses, see [Azure Active Directory v2.0 and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds).</span></span> 
- <span data-ttu-id="e7645-236">サービスから Microsoft Graph を呼び出すサンプルについては、GitHub の「[v2.0 デーモンのサンプル](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-236">For a sample that calls Microsoft Graph from a service, see the [v2.0 daemon sample](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) on GitHub.</span></span>
- <span data-ttu-id="e7645-237">推奨される Azure AD v2.0 の認証ライブラリ (Microsoft およびサード パーティ) の詳細については、「[Azure Active Directory v2.0 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-237">For more information about recommended Microsoft and third-party authentication libraries for Azure AD v2.0, see [Azure Active Directory v2.0 authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).</span></span>

## <a name="azure-ad-endpoint-considerations"></a><span data-ttu-id="e7645-238">Azure AD エンドポイントに関して考慮すべき事項</span><span class="sxs-lookup"><span data-stu-id="e7645-238">Azure AD endpoint considerations</span></span>

<span data-ttu-id="e7645-239">Azure AD エンドポイントを使用している場合、アプリの構成方法と Azure AD へのサインイン方法にはいくつかの違いがあります。</span><span class="sxs-lookup"><span data-stu-id="e7645-239">If you are using the Azure AD endpoint, there are some differences in the way that you configure your app and the way that it signs in to Azure AD:</span></span>

- <span data-ttu-id="e7645-p121">アプリは [Azure ポータル](https://portal.azure.com)を使用して構成します。Azure ポータルでアプリを構成する方法の詳細については、「[Azure Active Directory とアプリケーションの統合：アプリケーションの追加](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-p121">You use the [Azure portal](https://portal.azure.com) to configure your app. For more information about configuring apps with the Azure portal, see [Integrating applications with Azure Active Directory: Adding an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)</span></span>
- <span data-ttu-id="e7645-242">アプリがマルチ テナント アプリの場合は、[Azure ポータル](https://portal.azure.com)でマルチ テナントとなるよう明示的に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7645-242">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant at the [Azure portal](https://portal.azure.com).</span></span>
- <span data-ttu-id="e7645-p122">管理者の同意エンドポイント (`/adminconsent`) はありません。その代わりに、同意要求に `prompt=admin_consent` パラメーターを追加することで、アプリは実行時に管理者の同意を要求できます。詳細については、「[Azure Active Directory とアプリケーションの統合](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications)」の「**実行時の Azure AD 同意フレームワークのトリガー**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-p122">There is no admin consent endpoint (`/adminconsent`), instead, your app can request administrator consent during runtime by adding the `prompt=admin_consent` parameter to an authorization request. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).</span></span>
- <span data-ttu-id="e7645-p123">承認とトークン要求のパラメーターは異なります。たとえば、Azure AD エンドポイント要求には、`scope` パラメーターはありません。その代わりに、`resource` パラメーターを使用して、承認 (管理者の同意用) またはトークンが要求されているリソース (`resource=https://graph.microsoft.com`) の URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7645-p123">The parameters in authorization and token requests are different. For example, there is no `scope` parameter in Azure AD endpoint requests; instead, the `resource` parameter is used to specify the URI of the resource (`resource=https://graph.microsoft.com`) that authorization (for administrator consent) or a token is being requested for.</span></span>

<span data-ttu-id="e7645-247">Azure AD エンドポイントの場合は、次のリソースを使用して、このシナリオについてさらに詳しく調べることができます。</span><span class="sxs-lookup"><span data-stu-id="e7645-247">For the Azure AD endpoint, you can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="e7645-248">クライアント資格情報の付与フローの概要、サンプル、詳細な処理へのクイック リンクについては、「[開発者のための Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)」の**作業の開始セクション**の**サービス間**を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-248">For quick links to an overview, samples, and a detailed treatment of the client credentials grant flow, see **Service-to-Service** in the **Getting Started section** in [Azure Active Directory for Developers](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide).</span></span>
- <span data-ttu-id="e7645-p124">Azure AD エンドポイントの場合は、Azure Active Directory 認証ライブラリ (ADAL) を使用して Azure AD からトークンを取得できます。ADAL は、.NET、iOS、Android、JavaScript、Java、および Node.js を含む、いくつかのプラットフォームで利用できます。Azure AD エンドポイント向けの ADAL と、その他の Microsoft 認証ライブラリの詳細については、「[Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7645-p124">For the Azure AD endpoint, you can use the Azure Active Directory Authentication Library (ADAL) to get tokens from Azure AD. ADAL is available for several platforms including .NET, iOS, Android, JavaScript, Java, and Node.js. For more information about ADAL and other Microsoft authentication libraries for the Azure AD endpoint, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> 

 
