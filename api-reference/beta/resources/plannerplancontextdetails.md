---
title: プラン、contextdetails リソースの種類
description: 「 **plan the contextdetails** resource」には、プランのコンテキストに関する追加情報が含まれています。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 025e5b1623333d0235ae83e061e30247a3d130f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505950"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="95184-103">プラン、contextdetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95184-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95184-104">「 **plan the contextdetails** resource」には、プランの[コンテキスト](plannerplancontext.md)に関する追加情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="95184-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="95184-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95184-105">Properties</span></span>
| <span data-ttu-id="95184-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95184-106">Property</span></span>     | <span data-ttu-id="95184-107">型</span><span class="sxs-lookup"><span data-stu-id="95184-107">Type</span></span>   |<span data-ttu-id="95184-108">説明</span><span class="sxs-lookup"><span data-stu-id="95184-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95184-109">url</span><span class="sxs-lookup"><span data-stu-id="95184-109">url</span></span>|<span data-ttu-id="95184-110">String</span><span class="sxs-lookup"><span data-stu-id="95184-110">String</span></span>|<span data-ttu-id="95184-111">関連する[プランのコンテキスト](plannerplancontext.md)によって表されるユーザーの作業の URL。</span><span class="sxs-lookup"><span data-stu-id="95184-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="95184-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95184-112">JSON representation</span></span>

<span data-ttu-id="95184-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95184-113">The following is a JSON representation of the resource.</span></span>

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
