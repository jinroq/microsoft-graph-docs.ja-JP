---
title: plannerPlanContextDetails リソースの種類
description: '**PlannerPlanContextDetails**リソースには、plannerPlanContext に関する追加情報が含まれています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 025e5b1623333d0235ae83e061e30247a3d130f6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520250"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="570fb-103">plannerPlanContextDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="570fb-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="570fb-104">**PlannerPlanContextDetails**リソースには、 [plannerPlanContext](plannerplancontext.md)に関する追加情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="570fb-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="570fb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="570fb-105">Properties</span></span>
| <span data-ttu-id="570fb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="570fb-106">Property</span></span>     | <span data-ttu-id="570fb-107">型</span><span class="sxs-lookup"><span data-stu-id="570fb-107">Type</span></span>   |<span data-ttu-id="570fb-108">説明</span><span class="sxs-lookup"><span data-stu-id="570fb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="570fb-109">url</span><span class="sxs-lookup"><span data-stu-id="570fb-109">url</span></span>|<span data-ttu-id="570fb-110">String</span><span class="sxs-lookup"><span data-stu-id="570fb-110">String</span></span>|<span data-ttu-id="570fb-111">関連付けられた[plannerPlanContext](plannerplancontext.md)によって表されるユーザー エクスペリエンスの URL です。</span><span class="sxs-lookup"><span data-stu-id="570fb-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="570fb-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="570fb-112">JSON representation</span></span>

<span data-ttu-id="570fb-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="570fb-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
