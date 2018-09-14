# <a name="use-the-microsoft-graph-security-api"></a><span data-ttu-id="4379f-101">Microsoft Graph API を使用</span><span class="sxs-lookup"><span data-stu-id="4379f-101">Use the Microsoft Graph API</span></span>

<span data-ttu-id="4379f-102">Microsoft グラフ セキュリティ API は、統一されたインタ フェースとマイクロソフトとエコシステムのパートナーからのセキュリティ ソリューションと統合するためにスキーマを提供します。</span><span class="sxs-lookup"><span data-stu-id="4379f-102">The Microsoft Graph Security API provides a unified interface and schema to integrate with security solutions from Microsoft and ecosystem partners.</span></span> <span data-ttu-id="4379f-103">これは、セキュリティ ・ オペレーションを合理化し、サイバー脅威の増加が防御よりのお客様を支援します。</span><span class="sxs-lookup"><span data-stu-id="4379f-103">This empowers customers to streamline security operations and better defend against increasing cyber threats.</span></span> <span data-ttu-id="4379f-104">Microsoft Graph Security APIをフェデレーションセキュリティ集約サービスとして使用して、すべてのオンボードセキュリティプロバイダにクエリを送信し、集計応答を取得できます。</span><span class="sxs-lookup"><span data-stu-id="4379f-104">The Microsoft Graph Security API can be used as a federated security aggregation service to submit queries to all onboarded security providers to get aggregated responses.</span></span> <span data-ttu-id="4379f-105">Microsoft Graph Security APIを使用して、次のようなアプリケーションを構築します。</span><span class="sxs-lookup"><span data-stu-id="4379f-105">Use Microsoft Graph Security API to build applications that:</span></span>

- <span data-ttu-id="4379f-106">統合し、複数のソースからのセキュリティの警告の相関関係</span><span class="sxs-lookup"><span data-stu-id="4379f-106">Consolidate and correlate security alerts from multiple sources</span></span>
- <span data-ttu-id="4379f-107">コンテキストデータのロックを解除して調査を通知</span><span class="sxs-lookup"><span data-stu-id="4379f-107">Unlock contextual data to inform investigations</span></span>
- <span data-ttu-id="4379f-108">セキュリティ操作を自動化して効率を高める</span><span class="sxs-lookup"><span data-stu-id="4379f-108">Automate security operations for greater efficiency</span></span>
- <span data-ttu-id="4379f-109">積極的なリスク管理を可能にするセキュリティデータの可視性を提供</span><span class="sxs-lookup"><span data-stu-id="4379f-109">Provide visibility into security data to enable proactive risk management</span></span>

<span data-ttu-id="4379f-110">Microsoft Graph Security APIには、次のキーエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4379f-110">The Microsoft Graph Security API includes the following key entities.</span></span>

## <a name="alerts"></a><span data-ttu-id="4379f-111">アラート</span><span class="sxs-lookup"><span data-stu-id="4379f-111">Alerts</span></span>

<span data-ttu-id="4379f-112">通知は、マイクロソフトまたはパートナーのセキュリティ ・ ソリューションが既に特定し、アクションの通知フラグが設定されているお客様のテナント内で潜在的なセキュリティ上の問題です。</span><span class="sxs-lookup"><span data-stu-id="4379f-112">Alerts are potential security issues within a customer's tenant that Microsoft or partner security solutions have identified and are flagged for action or notification.</span></span> <span data-ttu-id="4379f-113">Microsoft Graph Security [ アラート](alert.md) エンティティを使用すると、統合されたすべてのソリューションでセキュリティの問題を統一し、合理化することができます。</span><span class="sxs-lookup"><span data-stu-id="4379f-113">With the Microsoft Graph Security [alerts](alert.md) entity, you can unify and streamline security  issues across all integrated solutions.</span></span> <span data-ttu-id="4379f-114">これは、アプリケーションのアラートおよび脅威の保護とレスポンスを向上させるためにコンテキストを関連付けることもできます。</span><span class="sxs-lookup"><span data-stu-id="4379f-114">This also enables applications to correlate alerts and context to improve threat protection and response.</span></span> <span data-ttu-id="4379f-115">これらは、インシデントの解決方法を調査の時間と時間を減らすことでセキュリティの運用効率をアンロックします。</span><span class="sxs-lookup"><span data-stu-id="4379f-115">These unlock security operational efficiencies by reducing investigation time and time to resolution for incidents.</span></span> <span data-ttu-id="4379f-116">アラートの更新機能により、さまざまなセキュリティ製品およびサービスの [アラート](alert.md) のエンティティを更新することによって、Microsoft グラフ セキュリティ API と統合されている間、特定のアラートの状態を同期できます。</span><span class="sxs-lookup"><span data-stu-id="4379f-116">With the alert update capability, you can sync the status of specific alerts across different security products and services that are integrated with the Microsoft Graph Security API by updating your [alerts](alert.md) entity.</span></span>

<span data-ttu-id="4379f-117">Microsoft Graph Security統合ソリューションは、次のセキュリティプロバイダからアラートを受信します。</span><span class="sxs-lookup"><span data-stu-id="4379f-117">Microsoft Graph Security-integrated solutions will receive alerts from the following security providers:</span></span>

- <span data-ttu-id="4379f-118">Azure のセキュリティ センター</span><span class="sxs-lookup"><span data-stu-id="4379f-118">Azure AD Identity Protection, Azure Security Center</span></span>
- <span data-ttu-id="4379f-119">Azure Active Directory Id の保護</span><span class="sxs-lookup"><span data-stu-id="4379f-119">Azure Active Directory Identity Protection</span></span>
- <span data-ttu-id="4379f-120">Azure 情報保護</span><span class="sxs-lookup"><span data-stu-id="4379f-120">Azure Information Protection</span></span>
- <span data-ttu-id="4379f-121">Microsoftクラウドアプリケーションのセキュリティ</span><span class="sxs-lookup"><span data-stu-id="4379f-121">Microsoft Cloud Security Policy</span></span>
- <span data-ttu-id="4379f-122">Windows Defender 高度な脅威からの保護</span><span class="sxs-lookup"><span data-stu-id="4379f-122">Windows Defender Advanced Threat Protection</span></span>
- <span data-ttu-id="4379f-123">Microsoft Intune (プライベート プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4379f-123">Microsoft Intune (private preview)</span></span>
- <span data-ttu-id="4379f-124">Office 365 (準備中)</span><span class="sxs-lookup"><span data-stu-id="4379f-124">Office 365 (coming soon)</span></span>
- <span data-ttu-id="4379f-125">Palo Alto Networks App Frameworkなどのパートナーソリューション</span><span class="sxs-lookup"><span data-stu-id="4379f-125">Partner solutions, such as Palo Alto Networks App Framework</span></span>

> <span data-ttu-id="4379f-126">**注:** 新しいプロバイダーは、Microsoft のグラフのセキュリティ エコシステムの契約時では継続的にします。</span><span class="sxs-lookup"><span data-stu-id="4379f-126">**Note:** New providers are continuously onboarding to the Microsoft Graph Security ecosystem.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="4379f-127">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="4379f-127">Common use cases</span></span>

<span data-ttu-id="4379f-128">以下は、Microsoft Graph Security APIを使用するための最も一般的な要求の一部です。</span><span class="sxs-lookup"><span data-stu-id="4379f-128">The following are some of the most popular requests for working with the Microsoft Graph Security API:</span></span>

| <span data-ttu-id="4379f-129">**ユース ケース**</span><span class="sxs-lookup"><span data-stu-id="4379f-129">**Use cases**</span></span>   | <span data-ttu-id="4379f-130">**REST リソース**</span><span class="sxs-lookup"><span data-stu-id="4379f-130">**REST resources**</span></span> | <span data-ttu-id="4379f-131">**Graph エクスプローラーで試す**</span><span class="sxs-lookup"><span data-stu-id="4379f-131">**Try in Graph Explorer**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4379f-132">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="4379f-132">List alerts</span></span> | [<span data-ttu-id="4379f-133">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="4379f-133">List alerts</span></span>](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| <span data-ttu-id="4379f-134">通知を更新</span><span class="sxs-lookup"><span data-stu-id="4379f-134">Update alerts</span></span> | [<span data-ttu-id="4379f-135">警告の更新</span><span class="sxs-lookup"><span data-stu-id="4379f-135">Update alert</span></span>](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

<span data-ttu-id="4379f-136">購読して、Microsoft のグラフのセキュリティ エンティティの更新に関する通知を受け取るには、Graph [webhooks](../../../concepts/webhooks.md) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4379f-136">You can use Microsoft Graph [webhooks](../../../concepts/webhooks.md) to subscribe to and receive notifications about updates to Microsoft Graph Security entities.</span></span>

## <a name="resources"></a><span data-ttu-id="4379f-137">リソース</span><span class="sxs-lookup"><span data-stu-id="4379f-137">Resources</span></span>

<span data-ttu-id="4379f-138">コードを作成し、これらのMicrosoft Graph Security APIサンプルに寄稿：</span><span class="sxs-lookup"><span data-stu-id="4379f-138">Code and contribute to these Microsoft Graph Security API samples:</span></span>

- [<span data-ttu-id="4379f-139">ASP.NET (C#) のサンプル</span><span class="sxs-lookup"><span data-stu-id="4379f-139">ASP.NET (C#) sample</span></span>](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [<span data-ttu-id="4379f-140">Python のサンプル</span><span class="sxs-lookup"><span data-stu-id="4379f-140">Python Sample</span></span>](https://github.com/microsoftgraph/python-security-rest-sample)
- [<span data-ttu-id="4379f-141">Node.js (JavaScript) のサンプル</span><span class="sxs-lookup"><span data-stu-id="4379f-141">Node.js (JavaScript) sample</span></span>](https://github.com/microsoftgraph/nodejs-security-sample)

<span data-ttu-id="4379f-142">コミュニティに参加。</span><span class="sxs-lookup"><span data-stu-id="4379f-142">Engage with the community:</span></span>

- [<span data-ttu-id="4379f-143">技術コミュニティーに参加</span><span class="sxs-lookup"><span data-stu-id="4379f-143">Join the tech community</span></span>](https://aka.ms/graphsecuritycommunity)
- [<span data-ttu-id="4379f-144">StackOverflow を説明</span><span class="sxs-lookup"><span data-stu-id="4379f-144">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a><span data-ttu-id="4379f-145">次の手順</span><span class="sxs-lookup"><span data-stu-id="4379f-145">Next steps</span></span>

<span data-ttu-id="4379f-146">Microsoft グラフ セキュリティ API は、Microsoft およびパートナーからのさまざまなセキュリティ ソリューションと連携するための新しい方法を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="4379f-146">The Microsoft Graph Security API can open up new ways for you to engage with different security solutions from Microsoft and partners.</span></span> <span data-ttu-id="4379f-147">開始するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="4379f-147">Follow these steps to get started:</span></span>

- <span data-ttu-id="4379f-148"> [アラート](alert.md)にドリル ・ ダウンします。</span><span class="sxs-lookup"><span data-stu-id="4379f-148">Drill down into [alerts](alert.md).</span></span>
- <span data-ttu-id="4379f-149">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。</span><span class="sxs-lookup"><span data-stu-id="4379f-149">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> <span data-ttu-id="4379f-150">[ **サンプル クエリ**] は、 **多くのサンプルを表示する** を選択し、セキュリティ カテゴリを **オン**に設定します。</span><span class="sxs-lookup"><span data-stu-id="4379f-150">Under **Sample Queries**, choose **show more samples** and set the Security category to **on**.</span></span>
- <span data-ttu-id="4379f-151">エンティティの変更 [を購読して、受信通知](../../../concepts/webhooks.md) を実行してください。</span><span class="sxs-lookup"><span data-stu-id="4379f-151">Try [subscribing to and receiving notifications](../../../concepts/webhooks.md) on entity changes.</span></span>

<span data-ttu-id="4379f-p105">さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4379f-p105">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
