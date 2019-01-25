---
title: filterOperand リソースの種類
description: オペランドの値のコレクションが含まれています。
localization_priority: Normal
ms.openlocfilehash: ab62477889cc92954ed308c508e18a638cd59375
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515378"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="edb20-103">filterOperand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="edb20-103">filterOperand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edb20-104">オペランドの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="edb20-104">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="edb20-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edb20-105">Properties</span></span>
| <span data-ttu-id="edb20-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edb20-106">Property</span></span>     | <span data-ttu-id="edb20-107">型</span><span class="sxs-lookup"><span data-stu-id="edb20-107">Type</span></span>   |<span data-ttu-id="edb20-108">説明</span><span class="sxs-lookup"><span data-stu-id="edb20-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edb20-109">values</span><span class="sxs-lookup"><span data-stu-id="edb20-109">values</span></span>|<span data-ttu-id="edb20-110">String コレクション</span><span class="sxs-lookup"><span data-stu-id="edb20-110">String collection</span></span>|<span data-ttu-id="edb20-111">値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="edb20-111">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edb20-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="edb20-112">JSON representation</span></span>

<span data-ttu-id="edb20-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="edb20-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperand"
}-->

```json
{
  "values": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
