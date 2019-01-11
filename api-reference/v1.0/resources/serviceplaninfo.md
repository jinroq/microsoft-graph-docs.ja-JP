---
title: servicePlanInfo リソースの種類
description: 購読している SKU に関連付けられているサービス プランに関する情報が含まれています。subscribedSku エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 837170881c7c093d26c5b59662e20e87b399a029
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845452"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="9ad6c-104">servicePlanInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ad6c-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="9ad6c-p102">購読している SKU に関連付けられているサービス プランに関する情報が含まれています。[subscribedSku](subscribedsku.md) エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="9ad6c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ad6c-107">Properties</span></span>
| <span data-ttu-id="9ad6c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ad6c-108">Property</span></span>     | <span data-ttu-id="9ad6c-109">種類</span><span class="sxs-lookup"><span data-stu-id="9ad6c-109">Type</span></span>   |<span data-ttu-id="9ad6c-110">説明</span><span class="sxs-lookup"><span data-stu-id="9ad6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ad6c-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="9ad6c-111">servicePlanId</span></span>|<span data-ttu-id="9ad6c-112">Guid</span><span class="sxs-lookup"><span data-stu-id="9ad6c-112">Guid</span></span>|<span data-ttu-id="9ad6c-113">サービス プランの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="9ad6c-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="9ad6c-114">servicePlanName</span></span>|<span data-ttu-id="9ad6c-115">String</span><span class="sxs-lookup"><span data-stu-id="9ad6c-115">String</span></span>|<span data-ttu-id="9ad6c-116">サービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-116">The name of the service plan.</span></span>|
|<span data-ttu-id="9ad6c-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="9ad6c-117">provisioningStatus</span></span>|<span data-ttu-id="9ad6c-118">String</span><span class="sxs-lookup"><span data-stu-id="9ad6c-118">String</span></span>|<span data-ttu-id="9ad6c-p103">サービス プランのプロビジョニング状況。可能な値:</span><span class="sxs-lookup"><span data-stu-id="9ad6c-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="9ad6c-121">Success - サービスは完全にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="9ad6c-122">Disabled - サービスは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="9ad6c-123">PendingInput - サービスはまだプロビジョニングされていません。サービスの確認を待っています。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="9ad6c-124">PendingActivation - サービスはプロビジョニングされていますが、管理者による明示的なアクティブ化が必要です (Intune_O365 サービスプランなど)</span><span class="sxs-lookup"><span data-stu-id="9ad6c-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="9ad6c-125">PendingProvisioning - Microsoft では製品の SKU に新しいサービスを追加していますが、テナント側でまだアクティブ化されていません。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="9ad6c-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="9ad6c-126">appliesTo</span></span>|<span data-ttu-id="9ad6c-127">String</span><span class="sxs-lookup"><span data-stu-id="9ad6c-127">String</span></span>|<span data-ttu-id="9ad6c-p104">サービス プランを割り当てることができるオブジェクト。可能な値:</span><span class="sxs-lookup"><span data-stu-id="9ad6c-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="9ad6c-130">User - サービス プランを個別のユーザーに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="9ad6c-131">Company - サービス プランをテナント全体に割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="9ad6c-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ad6c-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ad6c-132">JSON representation</span></span>

<span data-ttu-id="9ad6c-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9ad6c-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
