---
title: plannerPlanContextCollection リソースの種類
description: '**PlannerPlanContextCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。 このリソースは、オープン型であり、plannerPlan オブジェクトの一部であります。 プロパティと値のペアの値は、plannerPlanContext オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6ec515a164c5b0fca6334930b55a4b5d4e73b7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516498"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="9b4f9-105">plannerPlanContextCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b4f9-105">plannerPlanContextCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="9b4f9-106">**PlannerPlanContextCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-106">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="9b4f9-107">このリソースは、オープン型であり、 [plannerPlan](plannerplan.md)オブジェクトの一部であります。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-107">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="9b4f9-108">プロパティと値のペアの値は、 [plannerPlanContext](plannerplancontext.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-108">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="9b4f9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4f9-109">Properties</span></span>
<span data-ttu-id="9b4f9-110">このオープン型のプロパティを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-110">You can define the properties of this open type.</span></span> <span data-ttu-id="9b4f9-111">プロパティの値はプロパティ名と外部のコンテキストを表す特徴的な識別子である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-111">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="9b4f9-112">プロパティの値は、 [plannerPlanContext](plannerplancontext.md)オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-112">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="9b4f9-113">OData の要件に基づき、オープン型のプロパティ名は次の文字を含めることはできません: `.`、 `:`、 `%`、 `@`。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-113">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="9b4f9-114">これらの文字は、URL エンコーディングを使用してエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-114">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="9b4f9-115">お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b4f9-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b4f9-116">JSON representation</span></span>

<span data-ttu-id="9b4f9-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b4f9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextcollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
