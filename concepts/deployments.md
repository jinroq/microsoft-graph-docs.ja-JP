# <a name="national-cloud-deployments"></a><span data-ttu-id="beed5-101">国内クラウドの展開</span><span class="sxs-lookup"><span data-stu-id="beed5-101">National cloud deployments</span></span>


<span data-ttu-id="beed5-102">Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。</span><span class="sxs-lookup"><span data-stu-id="beed5-102">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="beed5-103">これらの国内クラウド バージョンは、Microsoft エンタープライズ クラウド サービスとは物理的および論理的に独立したネットワーク インスタンスで、特定の国の地理的な境界内に限定され、現地スタッフによって運営されます。</span><span class="sxs-lookup"><span data-stu-id="beed5-103">Microsoft cloud services are available in three separate national clouds. These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel. To learn more, see Microsoft National Clouds.</span></span> <span data-ttu-id="beed5-104">詳細については、「[Microsoft の国内クラウド](https://www.microsoft.com/ja-JP/TrustCenter/CloudServices/NationalCloud)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="beed5-104">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/ja-JP/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="beed5-105">現在の国内クラウドは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="beed5-105">Current national clouds include:</span></span>

- <span data-ttu-id="beed5-106">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="beed5-106">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="beed5-107">Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="beed5-107">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="beed5-108">21Vianet が中国で運用している Azure と Office 365</span><span class="sxs-lookup"><span data-stu-id="beed5-108">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="beed5-109">この記事では、Microsoft Graph のさまざまな国内クラウドの展開と、各展開において開発者が利用できる機能について示します。</span><span class="sxs-lookup"><span data-stu-id="beed5-109">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="beed5-110">Microsoft Graph と Microsoft Graph Explorer のサービス ルート エンドポイント</span><span class="sxs-lookup"><span data-stu-id="beed5-110">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="beed5-111">次の表に、各国内クラウドの Microsoft Graph と Microsoft Graph Explorer のサービス ルート エンドポイントを示します。</span><span class="sxs-lookup"><span data-stu-id="beed5-111">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="beed5-112">国内クラウド</span><span class="sxs-lookup"><span data-stu-id="beed5-112">National Cloud</span></span> | <span data-ttu-id="beed5-113">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="beed5-113">Microsoft Graph</span></span> | <span data-ttu-id="beed5-114">Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="beed5-114">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="beed5-115">21Vianet によって運営されている Microsoft Graph China</span><span class="sxs-lookup"><span data-stu-id="beed5-115">Microsoft Graph operated by 21Vianet in China</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="beed5-116">Microsoft Graph Germany</span><span class="sxs-lookup"><span data-stu-id="beed5-116">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="beed5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beed5-117">Not supported.</span></span> |
| <span data-ttu-id="beed5-118">米国政府機関向け Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="beed5-118">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="beed5-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beed5-119">Not supported.</span></span> |
| <span data-ttu-id="beed5-120">Microsoft Graph グローバル サービス</span><span class="sxs-lookup"><span data-stu-id="beed5-120">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="beed5-121">**メモ**: アプリから組織のデータへは、国内クラウド エンドポイント経由でのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="beed5-121">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="beed5-122">つまり、特定の国内クラウドに登録されたテナント内のデータにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="beed5-122">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="beed5-123">Microsoft Graph を介して個人用 Microsoft アカウントに関連付けられているコンシューマー データにアクセスを試みるアプリには、グローバル サービス (https://graph.microsoft.com) を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="beed5-123">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="beed5-124">国内クラウドの展開用に獲得したアクセス トークンは、グローバル サイト用に獲得したアクセス トークンと交換して使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="beed5-124">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="beed5-125">Azure AD の OpenID Connect と OAuth2.0 のエンドポイント</span><span class="sxs-lookup"><span data-stu-id="beed5-125">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="beed5-126">次の表に、国内クラウドごとに Microsoft Graph を呼び出すためのトークンを獲得するときに使用される Azure Active Directory (Azure AD) エンドポイントのベース URL をまとめます。</span><span class="sxs-lookup"><span data-stu-id="beed5-126">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="beed5-127">国内クラウド</span><span class="sxs-lookup"><span data-stu-id="beed5-127">National Cloud</span></span> | <span data-ttu-id="beed5-128">Azure AD ルート エンドポイント</span><span class="sxs-lookup"><span data-stu-id="beed5-128">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="beed5-129">21Vianet によって運営されている Azure AD China</span><span class="sxs-lookup"><span data-stu-id="beed5-129">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="beed5-130">Azure AD Germany</span><span class="sxs-lookup"><span data-stu-id="beed5-130">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="beed5-131">米国政府機関向け Azure AD</span><span class="sxs-lookup"><span data-stu-id="beed5-131">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="beed5-132">Azure AD (グローバル サービス)</span><span class="sxs-lookup"><span data-stu-id="beed5-132">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="beed5-p103">Azure AD 承認またはトークン エンドポイントへの要求は、該当する地域特有のベース URL を使用します。たとえば、ドイツの場合:</span><span class="sxs-lookup"><span data-stu-id="beed5-p103">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="beed5-135">承認の共通エンドポイントは、https://login.microsoftonline.de/common/oauth2/authorize です。</span><span class="sxs-lookup"><span data-stu-id="beed5-135">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="beed5-136">トークンの共通エンドポイントは、https://login.microsoftonline.de/common/oauth2/token です。</span><span class="sxs-lookup"><span data-stu-id="beed5-136">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="beed5-p104">テナント特有のエンドポイントは、前述の URL の「common」の部分を、テナント ID またはテナントの検証済みドメインに置き換えて構成できます。共通エンドポイントまたはテナント特有のエンドポイントのどちらを使用するかは、アプリの要件と、トークンを取得するために使用している認証フローによって異なります。Azure AD のアクセス トークンと Microsoft Graph について詳しくは、「[認証トークンの取得](./auth_overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="beed5-p104">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth_overview.md).</span></span>

> <span data-ttu-id="beed5-140">**注:** [Azure AD v2.0 認証エンドポイントとトークン エンドポイント](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview/)はグローバル サービスでのみ使用できます。国内クラウド展開での使用はまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beed5-140">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="beed5-141">サポートされている機能</span><span class="sxs-lookup"><span data-stu-id="beed5-141">Supported features</span></span>

<span data-ttu-id="beed5-142">次の Microsoft Graph 機能が、注記されている場所を除くすべての国内クラウド展開で (`/v1.0` エンドポイント上で) 通常利用できます。</span><span class="sxs-lookup"><span data-stu-id="beed5-142">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="beed5-143">ユーザー</span><span class="sxs-lookup"><span data-stu-id="beed5-143">Users</span></span>
* <span data-ttu-id="beed5-144">グループ</span><span class="sxs-lookup"><span data-stu-id="beed5-144">Groups</span></span>
* <span data-ttu-id="beed5-145">Excel (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)</span><span class="sxs-lookup"><span data-stu-id="beed5-145">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="beed5-146">OneDrive (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)</span><span class="sxs-lookup"><span data-stu-id="beed5-146">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="beed5-147">Outlook メール</span><span class="sxs-lookup"><span data-stu-id="beed5-147">Outlook Mail</span></span>
* <span data-ttu-id="beed5-148">Outlook カレンダー</span><span class="sxs-lookup"><span data-stu-id="beed5-148">Outlook Calendar</span></span>
* <span data-ttu-id="beed5-149">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="beed5-149">Personal Contacts</span></span> 
* <span data-ttu-id="beed5-150">SharePointl (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)</span><span class="sxs-lookup"><span data-stu-id="beed5-150">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="beed5-151">デルタ クエリ (各国内クラウド展開のさまざまなリソースにおいてサポートが異なります)。</span><span class="sxs-lookup"><span data-stu-id="beed5-151">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="beed5-152">Webhook (各国内クラウド展開のさまざまなリソースにおいてサポートが異なります)。</span><span class="sxs-lookup"><span data-stu-id="beed5-152">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="beed5-153">次の Microsoft Graph 追加機能が、注記されている場所を除くすべての国内クラウド展開で通常、プレビュー段階として (`/beta` エンドポイント上で) 利用できます。</span><span class="sxs-lookup"><span data-stu-id="beed5-153">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="beed5-154">組織の連絡先</span><span class="sxs-lookup"><span data-stu-id="beed5-154">Organizational Contacts</span></span>
* <span data-ttu-id="beed5-155">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="beed5-155">Applications</span></span>
* <span data-ttu-id="beed5-156">サービス プリンシパル</span><span class="sxs-lookup"><span data-stu-id="beed5-156">Service Principals</span></span>

<span data-ttu-id="beed5-157">次の Microsoft Graph 機能に関しては、国内クラウド展開ではまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beed5-157">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="beed5-158">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="beed5-158">Microsoft Planner</span></span>
* <span data-ttu-id="beed5-159">ディレクトリ スキーマの拡張</span><span class="sxs-lookup"><span data-stu-id="beed5-159">Directory schema extensions</span></span>
* <span data-ttu-id="beed5-160">オープン型の拡張機能</span><span class="sxs-lookup"><span data-stu-id="beed5-160">Open type extensions</span></span>
