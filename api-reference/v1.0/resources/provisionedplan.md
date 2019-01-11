---
title: provisionedPlan リソースの種類
description: ユーザー エンティティと組織エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: dd8d4f5b406a2291a829d7c11d4948bd9a08d453
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831487"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="b2f82-103">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2f82-103">provisionedPlan resource type</span></span>

<span data-ttu-id="b2f82-104">[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b2f82-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="b2f82-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f82-105">Properties</span></span>
| <span data-ttu-id="b2f82-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f82-106">Property</span></span>     | <span data-ttu-id="b2f82-107">種類</span><span class="sxs-lookup"><span data-stu-id="b2f82-107">Type</span></span>   |<span data-ttu-id="b2f82-108">説明</span><span class="sxs-lookup"><span data-stu-id="b2f82-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2f82-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b2f82-109">capabilityStatus</span></span>|<span data-ttu-id="b2f82-110">String</span><span class="sxs-lookup"><span data-stu-id="b2f82-110">String</span></span>|<span data-ttu-id="b2f82-111">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="b2f82-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="b2f82-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="b2f82-112">provisioningStatus</span></span>|<span data-ttu-id="b2f82-113">String</span><span class="sxs-lookup"><span data-stu-id="b2f82-113">String</span></span>|<span data-ttu-id="b2f82-114">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="b2f82-114">For example, “Success”.</span></span>|
|<span data-ttu-id="b2f82-115">service</span><span class="sxs-lookup"><span data-stu-id="b2f82-115">service</span></span>|<span data-ttu-id="b2f82-116">String</span><span class="sxs-lookup"><span data-stu-id="b2f82-116">String</span></span>|<span data-ttu-id="b2f82-117">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="b2f82-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2f82-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2f82-118">JSON representation</span></span>

<span data-ttu-id="b2f82-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b2f82-119">Here is a JSON representation of the resource</span></span>

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
