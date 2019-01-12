---
title: 国内クラウドの展開
description: Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国内クラウド バージョンは、Microsoft エンタープライズ クラウド サービスの物理的および論理的ネットワークの独立したインスタンスで、特定の国の地理的な境界内に限定され、ローカル スタッフによって運営されます。 詳細については、「Microsoft National Clouds」 (Microsoft の国内クラウド) を参照してください。
localization_priority: Priority
ms.openlocfilehash: b22fce675bc97d0f22833d89dab01afd18e06032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840419"
---
# <a name="national-cloud-deployments"></a><span data-ttu-id="e59a8-105">国内クラウドの展開</span><span class="sxs-lookup"><span data-stu-id="e59a8-105">National cloud deployments</span></span>


<span data-ttu-id="e59a8-106">Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-106">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="e59a8-107">これらの国内クラウド バージョンは、Microsoft エンタープライズ クラウド サービスとは物理的および論理的に独立したネットワーク インスタンスで、特定の国の地理的な境界内に限定され、現地スタッフによって運営されます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-107">These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel.</span></span> <span data-ttu-id="e59a8-108">詳細については、「[Microsoft の国内クラウド](https://www.microsoft.com/ja-JP/TrustCenter/CloudServices/NationalCloud)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e59a8-108">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/ja-JP/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="e59a8-109">現在の国内クラウドは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e59a8-109">Current national clouds include:</span></span>

- <span data-ttu-id="e59a8-110">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e59a8-110">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="e59a8-111">Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="e59a8-111">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="e59a8-112">21Vianet が中国で運用している Azure と Office 365</span><span class="sxs-lookup"><span data-stu-id="e59a8-112">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="e59a8-113">この記事では、Microsoft Graph のさまざまな国内クラウドの展開と、各展開において開発者が利用できる機能について示します。</span><span class="sxs-lookup"><span data-stu-id="e59a8-113">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="e59a8-114">Microsoft Graph と Microsoft Graph Explorer のサービス ルート エンドポイント</span><span class="sxs-lookup"><span data-stu-id="e59a8-114">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="e59a8-115">次の表に、各国内クラウドの Microsoft Graph と Microsoft Graph Explorer のサービス ルート エンドポイントを示します。</span><span class="sxs-lookup"><span data-stu-id="e59a8-115">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="e59a8-116">国内クラウド</span><span class="sxs-lookup"><span data-stu-id="e59a8-116">National Cloud</span></span> | <span data-ttu-id="e59a8-117">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e59a8-117">Microsoft Graph</span></span> | <span data-ttu-id="e59a8-118">Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="e59a8-118">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="e59a8-119">21Vianet によって運営されている Microsoft Graph China</span><span class="sxs-lookup"><span data-stu-id="e59a8-119">Microsoft Graph China operated by 21Vianet</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="e59a8-120">Microsoft Graph Germany</span><span class="sxs-lookup"><span data-stu-id="e59a8-120">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="e59a8-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59a8-121">Not supported.</span></span> |
| <span data-ttu-id="e59a8-122">米国政府機関向け Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e59a8-122">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="e59a8-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59a8-123">Not supported.</span></span> |
| <span data-ttu-id="e59a8-124">Microsoft Graph グローバル サービス</span><span class="sxs-lookup"><span data-stu-id="e59a8-124">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="e59a8-125">**メモ**: アプリから組織のデータへは、国内クラウド エンドポイント経由でのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-125">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="e59a8-126">つまり、特定の国内クラウドに登録されたテナント内のデータにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-126">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="e59a8-127">Microsoft Graph を介して個人用 Microsoft アカウントに関連付けられているコンシューマー データにアクセスを試みるアプリには、グローバル サービス (https://graph.microsoft.com) を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e59a8-127">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="e59a8-128">国内クラウドの展開用に獲得したアクセス トークンは、グローバル サイト用に獲得したアクセス トークンと交換して使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="e59a8-128">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="e59a8-129">Azure AD の OpenID Connect と OAuth2.0 のエンドポイント</span><span class="sxs-lookup"><span data-stu-id="e59a8-129">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="e59a8-130">次の表に、国内クラウドごとに Microsoft Graph を呼び出すためのトークンを獲得するときに使用される Azure Active Directory (Azure AD) エンドポイントのベース URL をまとめます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-130">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="e59a8-131">国内クラウド</span><span class="sxs-lookup"><span data-stu-id="e59a8-131">National Cloud</span></span> | <span data-ttu-id="e59a8-132">Azure AD ルート エンドポイント</span><span class="sxs-lookup"><span data-stu-id="e59a8-132">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="e59a8-133">21Vianet によって運営されている Azure AD China</span><span class="sxs-lookup"><span data-stu-id="e59a8-133">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="e59a8-134">Azure AD Germany</span><span class="sxs-lookup"><span data-stu-id="e59a8-134">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="e59a8-135">米国政府機関向け Azure AD</span><span class="sxs-lookup"><span data-stu-id="e59a8-135">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="e59a8-136">Azure AD (グローバル サービス)</span><span class="sxs-lookup"><span data-stu-id="e59a8-136">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="e59a8-p104">Azure AD 承認またはトークン エンドポイントへの要求は、該当する地域特有のベース URL を使用します。たとえば、ドイツの場合:</span><span class="sxs-lookup"><span data-stu-id="e59a8-p104">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="e59a8-139">承認の共通エンドポイントは、https://login.microsoftonline.de/common/oauth2/authorize です。</span><span class="sxs-lookup"><span data-stu-id="e59a8-139">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="e59a8-140">トークンの共通エンドポイントは、https://login.microsoftonline.de/common/oauth2/token です。</span><span class="sxs-lookup"><span data-stu-id="e59a8-140">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="e59a8-p105">テナント特有のエンドポイントは、前述の URL の「common」の部分を、テナント ID またはテナントの検証済みドメインに置き換えて構成できます。共通エンドポイントまたはテナント特有のエンドポイントのどちらを使用するかは、アプリの要件と、トークンを取得するために使用している認証フローによって異なります。Azure AD のアクセス トークンと Microsoft Graph について詳しくは、「[認証トークンの取得](./auth-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e59a8-p105">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth-overview.md).</span></span>

> <span data-ttu-id="e59a8-144">**注:** [Azure AD v2.0 認証エンドポイントとトークン エンドポイント](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview/)はグローバル サービスでのみ使用できます。国内クラウド展開での使用はまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59a8-144">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="e59a8-145">サポートされている機能</span><span class="sxs-lookup"><span data-stu-id="e59a8-145">Supported features</span></span>

<span data-ttu-id="e59a8-146">次の Microsoft Graph 機能が、注記されている場所を除くすべての国内クラウド展開で (`/v1.0` エンドポイント上で) 通常利用できます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-146">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="e59a8-147">ユーザー</span><span class="sxs-lookup"><span data-stu-id="e59a8-147">Users</span></span>
* <span data-ttu-id="e59a8-148">グループ</span><span class="sxs-lookup"><span data-stu-id="e59a8-148">Groups</span></span>
* <span data-ttu-id="e59a8-149">Excel (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)</span><span class="sxs-lookup"><span data-stu-id="e59a8-149">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e59a8-150">OneDrive (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)</span><span class="sxs-lookup"><span data-stu-id="e59a8-150">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e59a8-151">Outlook メール</span><span class="sxs-lookup"><span data-stu-id="e59a8-151">Outlook Mail</span></span>
* <span data-ttu-id="e59a8-152">Outlook カレンダー</span><span class="sxs-lookup"><span data-stu-id="e59a8-152">Outlook Calendar</span></span>
* <span data-ttu-id="e59a8-153">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="e59a8-153">Personal Contacts</span></span> 
* <span data-ttu-id="e59a8-154">SharePointl (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)</span><span class="sxs-lookup"><span data-stu-id="e59a8-154">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e59a8-155">デルタ クエリ (各国内クラウド展開のさまざまなリソースにおいてサポートが異なります)。</span><span class="sxs-lookup"><span data-stu-id="e59a8-155">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="e59a8-156">Webhook (各国内クラウド展開のさまざまなリソースにおいてサポートが異なります)。</span><span class="sxs-lookup"><span data-stu-id="e59a8-156">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="e59a8-157">次の Microsoft Graph 追加機能が、注記されている場所を除くすべての国内クラウド展開で通常、プレビュー段階として (`/beta` エンドポイント上で) 利用できます。</span><span class="sxs-lookup"><span data-stu-id="e59a8-157">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="e59a8-158">組織の連絡先</span><span class="sxs-lookup"><span data-stu-id="e59a8-158">Organizational Contacts</span></span>
* <span data-ttu-id="e59a8-159">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e59a8-159">Applications</span></span>
* <span data-ttu-id="e59a8-160">サービス プリンシパル</span><span class="sxs-lookup"><span data-stu-id="e59a8-160">Service Principals</span></span>

<span data-ttu-id="e59a8-161">次の Microsoft Graph 機能に関しては、国内クラウド展開ではまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59a8-161">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="e59a8-162">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="e59a8-162">Microsoft Planner</span></span>
* <span data-ttu-id="e59a8-163">ディレクトリ スキーマの拡張</span><span class="sxs-lookup"><span data-stu-id="e59a8-163">Directory schema extensions</span></span>
* <span data-ttu-id="e59a8-164">オープン型の拡張機能</span><span class="sxs-lookup"><span data-stu-id="e59a8-164">Open type extensions</span></span>
