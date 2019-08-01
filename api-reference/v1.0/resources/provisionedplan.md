---
title: provisionedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの provisionedPlans プロパティは、**provisionedPlan** のコレクションです。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3560aab132448a0d13c4b4abe2590d4802cdf9f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034994"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="67da2-103">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67da2-103">provisionedPlan resource type</span></span>

<span data-ttu-id="67da2-104">**ユーザー** エンティティと[組織](user.md)エンティティの [provisionedPlans](organization.md) プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="67da2-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="67da2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67da2-105">Properties</span></span>
| <span data-ttu-id="67da2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67da2-106">Property</span></span>     | <span data-ttu-id="67da2-107">型</span><span class="sxs-lookup"><span data-stu-id="67da2-107">Type</span></span>   |<span data-ttu-id="67da2-108">説明</span><span class="sxs-lookup"><span data-stu-id="67da2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67da2-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="67da2-109">capabilityStatus</span></span>|<span data-ttu-id="67da2-110">String</span><span class="sxs-lookup"><span data-stu-id="67da2-110">String</span></span>|<span data-ttu-id="67da2-111">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="67da2-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="67da2-112">プロビジョニング状態</span><span class="sxs-lookup"><span data-stu-id="67da2-112">provisioningStatus</span></span>|<span data-ttu-id="67da2-113">String</span><span class="sxs-lookup"><span data-stu-id="67da2-113">String</span></span>|<span data-ttu-id="67da2-114">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="67da2-114">For example, “Success”.</span></span>|
|<span data-ttu-id="67da2-115">service</span><span class="sxs-lookup"><span data-stu-id="67da2-115">service</span></span>|<span data-ttu-id="67da2-116">String</span><span class="sxs-lookup"><span data-stu-id="67da2-116">String</span></span>|<span data-ttu-id="67da2-117">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="67da2-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67da2-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67da2-118">JSON representation</span></span>

<span data-ttu-id="67da2-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="67da2-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
