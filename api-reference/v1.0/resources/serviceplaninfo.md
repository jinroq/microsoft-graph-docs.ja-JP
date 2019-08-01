---
title: servicePlanInfo リソースの種類
description: 購読済み SKU に関連付けられているサービスプランに関する情報が含まれます。 SubscribedSku **** エンティティの serviceplans プロパティは、 **serviceplans info**のコレクションです。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5aa721ce300338e68ca284f4f4ed11b1f66faad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034385"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="a6651-104">servicePlanInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6651-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="a6651-105">購読済み SKU に関連付けられているサービスプランに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a6651-105">Contains information about a service plan associated with a subscribed SKU.</span></span> <span data-ttu-id="a6651-106">[SubscribedSku](subscribedsku.md)エンティティの**serviceplans**プロパティは、 **serviceplans info**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a6651-106">The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="a6651-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6651-107">Properties</span></span>
| <span data-ttu-id="a6651-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6651-108">Property</span></span>     | <span data-ttu-id="a6651-109">型</span><span class="sxs-lookup"><span data-stu-id="a6651-109">Type</span></span>   |<span data-ttu-id="a6651-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6651-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6651-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="a6651-111">servicePlanId</span></span>|<span data-ttu-id="a6651-112">Guid</span><span class="sxs-lookup"><span data-stu-id="a6651-112">Guid</span></span>|<span data-ttu-id="a6651-113">サービス プランの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a6651-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="a6651-114">Serviceplan の名前</span><span class="sxs-lookup"><span data-stu-id="a6651-114">servicePlanName</span></span>|<span data-ttu-id="a6651-115">String</span><span class="sxs-lookup"><span data-stu-id="a6651-115">String</span></span>|<span data-ttu-id="a6651-116">サービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="a6651-116">The name of the service plan.</span></span>|
|<span data-ttu-id="a6651-117">プロビジョニング状態</span><span class="sxs-lookup"><span data-stu-id="a6651-117">provisioningStatus</span></span>|<span data-ttu-id="a6651-118">String</span><span class="sxs-lookup"><span data-stu-id="a6651-118">String</span></span>|<span data-ttu-id="a6651-119">サービス プランのプロビジョニング状況。</span><span class="sxs-lookup"><span data-stu-id="a6651-119">The provisioning status of the service plan.</span></span> <span data-ttu-id="a6651-120">可能な値:</span><span class="sxs-lookup"><span data-stu-id="a6651-120">Possible values:</span></span><br/><span data-ttu-id="a6651-121">"Success"-サービスは完全にプロビジョニングされています。</span><span class="sxs-lookup"><span data-stu-id="a6651-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="a6651-122">[無効]-サービスが無効になっています。</span><span class="sxs-lookup"><span data-stu-id="a6651-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="a6651-123">"PendingInput"-サービスはまだ準備されていません。サービスの確認を待っている。</span><span class="sxs-lookup"><span data-stu-id="a6651-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="a6651-124">"PendingActivation"-サービスはプロビジョニングされていますが、管理者による明示的なライセンス認証が必要です (たとえば、Intune_O365 Service plan)。</span><span class="sxs-lookup"><span data-stu-id="a6651-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="a6651-125">"PendingProvisioning"-Microsoft では、製品 SKU に新しいサービスが追加されていますが、テナントではまだアクティブ化されていません。</span><span class="sxs-lookup"><span data-stu-id="a6651-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="a6651-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="a6651-126">appliesTo</span></span>|<span data-ttu-id="a6651-127">String</span><span class="sxs-lookup"><span data-stu-id="a6651-127">String</span></span>|<span data-ttu-id="a6651-128">サービスプランを割り当てることができるオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a6651-128">The object the service plan can be assigned to.</span></span> <span data-ttu-id="a6651-129">可能な値:</span><span class="sxs-lookup"><span data-stu-id="a6651-129">Possible values:</span></span><br/><span data-ttu-id="a6651-130">"User"-サービスプランを個々のユーザーに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a6651-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="a6651-131">"Company"-サービスプランは、テナント全体に割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a6651-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6651-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6651-132">JSON representation</span></span>

<span data-ttu-id="a6651-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a6651-133">Here is a JSON representation of the resource</span></span>

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
