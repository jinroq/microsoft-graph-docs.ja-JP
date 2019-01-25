---
title: エンティティ リソースの種類
description: なし
localization_priority: Normal
ms.openlocfilehash: e1dd9a8d66dd326076c8a7dd534c2210f53d06e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509120"
---
# <a name="entity-resource-type"></a><span data-ttu-id="07d3f-103">エンティティ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07d3f-103">entity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="07d3f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07d3f-104">Properties</span></span>
| <span data-ttu-id="07d3f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07d3f-105">Property</span></span> | <span data-ttu-id="07d3f-106">型</span><span class="sxs-lookup"><span data-stu-id="07d3f-106">Type</span></span>  | <span data-ttu-id="07d3f-107">説明</span><span class="sxs-lookup"><span data-stu-id="07d3f-107">Description</span></span> |
|:---------|:------|:------------|
|<span data-ttu-id="07d3f-108">id</span><span class="sxs-lookup"><span data-stu-id="07d3f-108">id</span></span>        |<span data-ttu-id="07d3f-109">String</span><span class="sxs-lookup"><span data-stu-id="07d3f-109">String</span></span> | <span data-ttu-id="07d3f-110">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="07d3f-110">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="07d3f-111">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07d3f-111">Relationships</span></span>
<span data-ttu-id="07d3f-112">なし</span><span class="sxs-lookup"><span data-stu-id="07d3f-112">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07d3f-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07d3f-113">JSON representation</span></span>

<span data-ttu-id="07d3f-114">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="07d3f-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "abstract": "true",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entity"
}-->
```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "entity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/entity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
