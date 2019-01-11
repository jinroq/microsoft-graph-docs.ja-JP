---
title: Microsoft Graph セキュリティ API を使用する
description: Microsoft グラフ セキュリティ API は、統一されたインタ フェースとマイクロソフトとエコシステムのパートナーからのセキュリティ ソリューションと統合するためにスキーマを提供します。 これは、セキュリティ ・ オペレーションを合理化し、サイバー脅威の増加が防御よりのお客様を支援します。 Microsoft グラフ セキュリティ API は、集約された応答を取得するすべての onboarded セキュリティ プロバイダーにクエリを発行するフェデレーション セキュリティ集約サービスとして使用できます。 Microsoft グラフ セキュリティ API を使用してアプリケーションを構築します。
localization_priority: Priority
ms.openlocfilehash: 79a4af5f340bbaf8b8d93938e83a60b524f9be2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823801"
---
# <a name="use-the-microsoft-graph-security-api"></a><span data-ttu-id="73795-106">Microsoft Graph セキュリティ API を使用する</span><span class="sxs-lookup"><span data-stu-id="73795-106">Use the Microsoft Graph Security API</span></span>

<span data-ttu-id="73795-107">Microsoft グラフ セキュリティ API は、統一されたインタ フェースとマイクロソフトとエコシステムのパートナーからのセキュリティ ソリューションと統合するためにスキーマを提供します。</span><span class="sxs-lookup"><span data-stu-id="73795-107">The Microsoft Graph Security API provides a unified interface and schema to integrate with security solutions from Microsoft and ecosystem partners.</span></span> <span data-ttu-id="73795-108">これは、セキュリティ ・ オペレーションを合理化し、サイバー脅威の増加が防御よりのお客様を支援します。</span><span class="sxs-lookup"><span data-stu-id="73795-108">This empowers customers to streamline security operations and better defend against increasing cyber threats.</span></span> <span data-ttu-id="73795-109">Microsoft グラフ セキュリティ API は、集約された応答を取得するすべての onboarded セキュリティ プロバイダーにクエリを発行するフェデレーション セキュリティ集約サービスとして使用できます。</span><span class="sxs-lookup"><span data-stu-id="73795-109">The Microsoft Graph Security API can be used as a federated security aggregation service to submit queries to all onboarded security providers to get aggregated responses.</span></span> <span data-ttu-id="73795-110">Microsoft グラフ セキュリティ API を使用してアプリケーションを構築します。</span><span class="sxs-lookup"><span data-stu-id="73795-110">Use Microsoft Graph Security API to build applications that:</span></span>

- <span data-ttu-id="73795-111">統合し、複数のソースからのセキュリティの警告の相関関係</span><span class="sxs-lookup"><span data-stu-id="73795-111">Consolidate and correlate security alerts from multiple sources</span></span>
- <span data-ttu-id="73795-112">調査を通知するためにコンテキストのデータのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="73795-112">Unlock contextual data to inform investigations</span></span>
- <span data-ttu-id="73795-113">効率のセキュリティ ・ オペレーションを自動化します。</span><span class="sxs-lookup"><span data-stu-id="73795-113">Automate security operations for greater efficiency</span></span>
- <span data-ttu-id="73795-114">プロアクティブ リスク管理を有効にするセキュリティ ・ データの可視性を提供します。</span><span class="sxs-lookup"><span data-stu-id="73795-114">Provide visibility into security data to enable proactive risk management</span></span>

<span data-ttu-id="73795-115">Microsoft グラフ セキュリティ API には、次のキーのエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="73795-115">The Microsoft Graph Security API includes the following key entities.</span></span>

## <a name="alerts"></a><span data-ttu-id="73795-116">アラート</span><span class="sxs-lookup"><span data-stu-id="73795-116">Alerts</span></span>

<span data-ttu-id="73795-117">通知は、マイクロソフトまたはパートナーのセキュリティ ・ ソリューションが既に特定し、アクションの通知フラグが設定されているお客様のテナント内で潜在的なセキュリティ上の問題です。</span><span class="sxs-lookup"><span data-stu-id="73795-117">Alerts are potential security issues within a customer's tenant that Microsoft or partner security solutions have identified and are flagged for action or notification.</span></span> <span data-ttu-id="73795-118">Microsoft グラフのセキュリティの[警告](alert.md)のエンティティとを統合し、すべての統合されたソリューションのセキュリティの問題を合理化できます。</span><span class="sxs-lookup"><span data-stu-id="73795-118">With the Microsoft Graph Security [alerts](alert.md) entity, you can unify and streamline security  issues across all integrated solutions.</span></span> <span data-ttu-id="73795-119">これは、アプリケーションのアラートおよび脅威の保護とレスポンスを向上させるためにコンテキストを関連付けることもできます。</span><span class="sxs-lookup"><span data-stu-id="73795-119">This also enables applications to correlate alerts and context to improve threat protection and response.</span></span> <span data-ttu-id="73795-120">これらは、インシデントの解決方法を調査の時間と時間を減らすことでセキュリティの運用効率をアンロックします。</span><span class="sxs-lookup"><span data-stu-id="73795-120">These unlock security operational efficiencies by reducing investigation time and time to resolution for incidents.</span></span> <span data-ttu-id="73795-121">アラートの更新機能により、さまざまなセキュリティ製品およびサービスの[アラート](alert.md)のエンティティを更新することによって、Microsoft グラフ セキュリティ API と統合されている間、特定のアラートの状態を同期できます。</span><span class="sxs-lookup"><span data-stu-id="73795-121">With the alert update capability, you can sync the status of specific alerts across different security products and services that are integrated with the Microsoft Graph Security API by updating your [alerts](alert.md) entity.</span></span>

<span data-ttu-id="73795-122">グラフのセキュリティに統合されたソリューションの Microsoft 次のセキュリティ プロバイダーからのアラートが表示されます。</span><span class="sxs-lookup"><span data-stu-id="73795-122">Microsoft Graph Security-integrated solutions will receive alerts from the following security providers:</span></span>

- [<span data-ttu-id="73795-123">Azure のセキュリティ センター</span><span class="sxs-lookup"><span data-stu-id="73795-123">Azure Security Center</span></span>](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [<span data-ttu-id="73795-124">Azure Active Directory Id の保護</span><span class="sxs-lookup"><span data-stu-id="73795-124">Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [<span data-ttu-id="73795-125">マイクロソフト クラウド アプリケーションのセキュリティ</span><span class="sxs-lookup"><span data-stu-id="73795-125">Microsoft Cloud Application Security</span></span>](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [<span data-ttu-id="73795-126">Windows Defender の脅威保護の詳細</span><span class="sxs-lookup"><span data-stu-id="73795-126">Windows Defender Advanced Threat Protection</span></span>](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- <span data-ttu-id="73795-127">[Azure の情報の保護](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**(プレビュー)**</span><span class="sxs-lookup"><span data-stu-id="73795-127">[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(preview)**</span></span>
- <span data-ttu-id="73795-128">Microsoft Intune **(プライベート プレビュー)**</span><span class="sxs-lookup"><span data-stu-id="73795-128">Microsoft Intune **(private preview)**</span></span>
- <span data-ttu-id="73795-129">Office 365 は **(準備中)**</span><span class="sxs-lookup"><span data-stu-id="73795-129">Office 365 **(coming soon)**</span></span>
- <span data-ttu-id="73795-130">Azure の脅威保護の詳細 **(準備中)**</span><span class="sxs-lookup"><span data-stu-id="73795-130">Azure Advanced Threat Protection **(coming soon)**</span></span>
- <span data-ttu-id="73795-131">パートナー ・ ソリューション、パロアルトのネットワーク ・ アプリケーション ・ フレームワーク</span><span class="sxs-lookup"><span data-stu-id="73795-131">Partner solutions, such as Palo Alto Networks App Framework</span></span>

> <span data-ttu-id="73795-132">**注:** 新しいプロバイダーは、Microsoft のグラフのセキュリティ エコシステムの契約時では継続的にします。</span><span class="sxs-lookup"><span data-stu-id="73795-132">**Note:** New providers are continuously onboarding to the Microsoft Graph Security ecosystem.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="73795-133">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="73795-133">Common use cases</span></span>

<span data-ttu-id="73795-134">以下は、Microsoft グラフ セキュリティ API を使用するための最も一般的な要求の一部です。</span><span class="sxs-lookup"><span data-stu-id="73795-134">The following are some of the most popular requests for working with the Microsoft Graph Security API:</span></span>

| <span data-ttu-id="73795-135">**ユース ケース**</span><span class="sxs-lookup"><span data-stu-id="73795-135">**Use cases**</span></span>   | <span data-ttu-id="73795-136">**REST リソース**</span><span class="sxs-lookup"><span data-stu-id="73795-136">**REST resources**</span></span> | <span data-ttu-id="73795-137">**グラフのエクスプ ローラーで試してみよう**</span><span class="sxs-lookup"><span data-stu-id="73795-137">**Try it in Graph Explorer**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="73795-138">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="73795-138">List alerts</span></span> | [<span data-ttu-id="73795-139">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="73795-139">List alerts</span></span>](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| <span data-ttu-id="73795-140">アラートを更新します。</span><span class="sxs-lookup"><span data-stu-id="73795-140">Update alerts</span></span> | [<span data-ttu-id="73795-141">警告の更新</span><span class="sxs-lookup"><span data-stu-id="73795-141">Update alert</span></span>](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

<span data-ttu-id="73795-142">購読して、Microsoft のグラフのセキュリティ エンティティの更新に関する通知を受け取るには、Graph [webhooks](/graph/webhooks)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="73795-142">You can use Microsoft Graph [webhooks](/graph/webhooks) to subscribe to and receive notifications about updates to Microsoft Graph Security entities.</span></span>

## <a name="resources"></a><span data-ttu-id="73795-143">リソース</span><span class="sxs-lookup"><span data-stu-id="73795-143">Resources</span></span>

<span data-ttu-id="73795-144">コードされ、これらの Microsoft グラフ セキュリティ API のサンプル。</span><span class="sxs-lookup"><span data-stu-id="73795-144">Code and contribute to these Microsoft Graph Security API samples:</span></span>

- [<span data-ttu-id="73795-145">サンプルの ASP.NET (C#)</span><span class="sxs-lookup"><span data-stu-id="73795-145">ASP.NET (C#) sample</span></span>](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [<span data-ttu-id="73795-146">Python のサンプル</span><span class="sxs-lookup"><span data-stu-id="73795-146">Python sample</span></span>](https://github.com/microsoftgraph/python-security-rest-sample)
- [<span data-ttu-id="73795-147">Node.js (JavaScript) のサンプル</span><span class="sxs-lookup"><span data-stu-id="73795-147">Node.js (JavaScript) sample</span></span>](https://github.com/microsoftgraph/nodejs-security-sample)

<span data-ttu-id="73795-148">コミュニティに参加します。</span><span class="sxs-lookup"><span data-stu-id="73795-148">Engage with the community:</span></span>

- [<span data-ttu-id="73795-149">テクニカル コミュニティに参加します。</span><span class="sxs-lookup"><span data-stu-id="73795-149">Join the tech community</span></span>](https://aka.ms/graphsecuritycommunity)
- [<span data-ttu-id="73795-150">StackOverflow を説明します。</span><span class="sxs-lookup"><span data-stu-id="73795-150">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a><span data-ttu-id="73795-151">次のステップ</span><span class="sxs-lookup"><span data-stu-id="73795-151">Next steps</span></span>

<span data-ttu-id="73795-152">Microsoft グラフ セキュリティ API は、Microsoft およびパートナーからのさまざまなセキュリティ ソリューションと連携するための新しい方法を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="73795-152">The Microsoft Graph Security API can open up new ways for you to engage with different security solutions from Microsoft and partners.</span></span> <span data-ttu-id="73795-153">開始する次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="73795-153">Follow these steps to get started:</span></span>

- <span data-ttu-id="73795-154">[アラート](alert.md)にドリル ・ ダウンします。</span><span class="sxs-lookup"><span data-stu-id="73795-154">Drill down into [alerts](alert.md).</span></span>
- <span data-ttu-id="73795-155">
  [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。</span><span class="sxs-lookup"><span data-stu-id="73795-155">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> <span data-ttu-id="73795-156">[**サンプル クエリ**] は、**多くのサンプルを表示する**を選択し、セキュリティ カテゴリを**オン**に設定します。</span><span class="sxs-lookup"><span data-stu-id="73795-156">Under **Sample Queries**, choose **show more samples** and set the Security category to **on**.</span></span>
- <span data-ttu-id="73795-157">エンティティの変更[をサブスクライブして、受信通知](/graph/webhooks)を実行してください。</span><span class="sxs-lookup"><span data-stu-id="73795-157">Try [subscribing to and receiving notifications](/graph/webhooks) on entity changes.</span></span>

<span data-ttu-id="73795-p106">さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73795-p106">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
