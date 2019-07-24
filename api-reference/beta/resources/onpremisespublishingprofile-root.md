---
title: オンプレミスの発行プロファイル
description: さまざまな Azure サービス (たとえば、Azue Active Directory Connect パススルー認証、Workday to Azure AD ユーザープロビジョニング) は、企業ネットワークの外部からさまざまな社内リソースへの条件付きアクセスを許可します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b0e975d932226adfa2c455baaa396c1d580f6ff
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841333"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="2976a-103">オンプレミスの発行プロファイル</span><span class="sxs-lookup"><span data-stu-id="2976a-103">On-premises publishing profiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2976a-104">さまざまな Azure サービス (たとえば、Azue Active Directory Connect パススルー認証、Workday to Azure AD ユーザープロビジョニング) は、企業ネットワークの外部からさまざまな社内リソースへの条件付きアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="2976a-104">Various Azure services (for example, Azue Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="2976a-105">テナント管理者によってインストールされた[社内エージェント](onpremisesagent.md)は、発行された特定の[リソース](publishedresource.md)への要求にアクセスしたり、処理したりするように構成できます。</span><span class="sxs-lookup"><span data-stu-id="2976a-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="2976a-106">[エージェントグループ](onpremisesagentgroup.md)を使用すると、テナント管理者は特定のエージェントを割り当てて、発行された特定の社内リソースを提供できます。</span><span class="sxs-lookup"><span data-stu-id="2976a-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="2976a-107">テナント管理者は、複数のエージェントをまとめてグループ化し、発行された各リソースをグループに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="2976a-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="2976a-108">同じオンプレミスの発行タイプのエンティティセット全体が[onPremisesPublishingProfile](onpremisespublishingprofile.md)によって表されます。</span><span class="sxs-lookup"><span data-stu-id="2976a-108">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="2976a-109">テナント管理者は、各**onPremisesPublishingProfile**に対して、エージェントが更新を受信したり、エージェントに対して更新プログラムを適用したりできる[時間枠](updatewindow.md)を構成できます。</span><span class="sxs-lookup"><span data-stu-id="2976a-109">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="2976a-110">**OnPremisesPublishingProfile**に指定された[updater 構成](hybridagentupdaterconfiguration.md)は、その**onPremisesPublishingProfile**内のすべてのエージェントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2976a-110">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="2976a-111">関連項目</span><span class="sxs-lookup"><span data-stu-id="2976a-111">See also</span></span>

- [<span data-ttu-id="2976a-112">オンプレミスのエージェント</span><span class="sxs-lookup"><span data-stu-id="2976a-112">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="2976a-113">オンプレミスエージェントグループ</span><span class="sxs-lookup"><span data-stu-id="2976a-113">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="2976a-114">オンプレミスの発行プロファイル</span><span class="sxs-lookup"><span data-stu-id="2976a-114">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="2976a-115">発行済みリソース</span><span class="sxs-lookup"><span data-stu-id="2976a-115">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
