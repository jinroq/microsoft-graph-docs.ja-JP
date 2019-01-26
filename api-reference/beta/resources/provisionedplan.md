---
title: provisionedPlan リソースの種類
description: ユーザー エンティティと組織エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: be19bb49409751ae5d7a0f11387e74770fde333b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572550"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="dc8a5-103">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc8a5-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc8a5-104">[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="dc8a5-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="dc8a5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc8a5-105">Properties</span></span>
| <span data-ttu-id="dc8a5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc8a5-106">Property</span></span>     | <span data-ttu-id="dc8a5-107">型</span><span class="sxs-lookup"><span data-stu-id="dc8a5-107">Type</span></span>   |<span data-ttu-id="dc8a5-108">説明</span><span class="sxs-lookup"><span data-stu-id="dc8a5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc8a5-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="dc8a5-109">capabilityStatus</span></span>|<span data-ttu-id="dc8a5-110">String</span><span class="sxs-lookup"><span data-stu-id="dc8a5-110">String</span></span>|<span data-ttu-id="dc8a5-111">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="dc8a5-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="dc8a5-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="dc8a5-112">provisioningStatus</span></span>|<span data-ttu-id="dc8a5-113">String</span><span class="sxs-lookup"><span data-stu-id="dc8a5-113">String</span></span>|<span data-ttu-id="dc8a5-114">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="dc8a5-114">For example, “Success”.</span></span>|
|<span data-ttu-id="dc8a5-115">service</span><span class="sxs-lookup"><span data-stu-id="dc8a5-115">service</span></span>|<span data-ttu-id="dc8a5-116">String</span><span class="sxs-lookup"><span data-stu-id="dc8a5-116">String</span></span>|<span data-ttu-id="dc8a5-117">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="dc8a5-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc8a5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc8a5-118">JSON representation</span></span>

<span data-ttu-id="dc8a5-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dc8a5-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/provisionedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
