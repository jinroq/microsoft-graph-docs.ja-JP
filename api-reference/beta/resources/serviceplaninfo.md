---
title: servicePlanInfo リソースの種類
description: 購読している SKU に関連付けられているサービス プランに関する情報が含まれています。subscribedSku エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。
ms.openlocfilehash: 86246de74caef6bf0c778f5b6b38e185841394b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071871"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="13504-104">servicePlanInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13504-104">servicePlanInfo resource type</span></span>

> <span data-ttu-id="13504-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13504-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13504-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13504-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13504-p103">購読している SKU に関連付けられているサービス プランに関する情報が含まれています。[subscribedSku](subscribedsku.md) エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="13504-p103">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="13504-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13504-109">Properties</span></span>
| <span data-ttu-id="13504-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13504-110">Property</span></span>     | <span data-ttu-id="13504-111">型</span><span class="sxs-lookup"><span data-stu-id="13504-111">Type</span></span>   |<span data-ttu-id="13504-112">説明</span><span class="sxs-lookup"><span data-stu-id="13504-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13504-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="13504-113">servicePlanId</span></span>|<span data-ttu-id="13504-114">Guid</span><span class="sxs-lookup"><span data-stu-id="13504-114">Guid</span></span>|<span data-ttu-id="13504-115">サービス プランの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="13504-115">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="13504-116">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="13504-116">servicePlanName</span></span>|<span data-ttu-id="13504-117">String</span><span class="sxs-lookup"><span data-stu-id="13504-117">String</span></span>|<span data-ttu-id="13504-118">サービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="13504-118">The name of the service plan.</span></span>|
|<span data-ttu-id="13504-119">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="13504-119">provisioningStatus</span></span>|<span data-ttu-id="13504-120">String</span><span class="sxs-lookup"><span data-stu-id="13504-120">String</span></span>|<span data-ttu-id="13504-p104">サービス プランのプロビジョニング状況。可能な値:</span><span class="sxs-lookup"><span data-stu-id="13504-p104">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="13504-123">Success - サービスは完全にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="13504-123">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="13504-124">Disabled - サービスは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="13504-124">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="13504-125">PendingInput - サービスはまだプロビジョニングされていません。サービスの確認を待っています。</span><span class="sxs-lookup"><span data-stu-id="13504-125">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="13504-126">"PendingActivation"のサービスは、プロビジョニングでは、(たとえば、Intune_O365 ・ サービス ・ プラン) を管理者が明示的な有効化が必要です。</span><span class="sxs-lookup"><span data-stu-id="13504-126">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="13504-127">PendingProvisioning - Microsoft では製品の SKU に新しいサービスを追加していますが、テナント側でまだアクティブ化されていません。</span><span class="sxs-lookup"><span data-stu-id="13504-127">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="13504-128">appliesTo</span><span class="sxs-lookup"><span data-stu-id="13504-128">appliesTo</span></span>|<span data-ttu-id="13504-129">String</span><span class="sxs-lookup"><span data-stu-id="13504-129">String</span></span>|<span data-ttu-id="13504-p105">サービス プランを割り当てることができるオブジェクト。可能な値:</span><span class="sxs-lookup"><span data-stu-id="13504-p105">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="13504-132">User - サービス プランを個別のユーザーに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="13504-132">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="13504-133">Company - サービス プランをテナント全体に割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="13504-133">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13504-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13504-134">JSON representation</span></span>

<span data-ttu-id="13504-135">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="13504-135">Here is a JSON representation of the resource</span></span>

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
