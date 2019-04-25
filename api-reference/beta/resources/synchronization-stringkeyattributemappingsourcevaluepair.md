---
title: stringKeyAttributeMappingSourceValuePair リソースの種類
description: キーが文字列で、値が attributeMappingSource であるキーと値のペアを表します。
localization_priority: Normal
ms.openlocfilehash: ff914c23a238356a821d2902bf18900cf9957548
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523225"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="8baf6-103">stringKeyAttributeMappingSourceValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8baf6-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8baf6-104">キーが文字列で、値が[attributeMappingSource](synchronization-attributemappingsource.md)であるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="8baf6-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8baf6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8baf6-105">Properties</span></span>
| <span data-ttu-id="8baf6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8baf6-106">Property</span></span>     | <span data-ttu-id="8baf6-107">型</span><span class="sxs-lookup"><span data-stu-id="8baf6-107">Type</span></span>   |<span data-ttu-id="8baf6-108">説明</span><span class="sxs-lookup"><span data-stu-id="8baf6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8baf6-109">Key</span><span class="sxs-lookup"><span data-stu-id="8baf6-109">key</span></span>|<span data-ttu-id="8baf6-110">String
</span><span class="sxs-lookup"><span data-stu-id="8baf6-110">String</span></span>|<span data-ttu-id="8baf6-111">The name of the parameter.</span><span class="sxs-lookup"><span data-stu-id="8baf6-111">The name of the parameter.</span></span>|
|<span data-ttu-id="8baf6-112">value</span><span class="sxs-lookup"><span data-stu-id="8baf6-112">value</span></span>|[<span data-ttu-id="8baf6-113">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="8baf6-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="8baf6-114">パラメーターの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8baf6-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8baf6-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8baf6-115">JSON representation</span></span>

<span data-ttu-id="8baf6-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8baf6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyattributemappingsourcevaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
