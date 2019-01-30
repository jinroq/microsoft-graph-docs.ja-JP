---
title: stringKeyObjectValuePair リソースの種類
description: キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642927"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="96492-104">stringKeyObjectValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96492-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96492-105">キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。</span><span class="sxs-lookup"><span data-stu-id="96492-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="96492-106">これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="96492-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="96492-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96492-107">Properties</span></span>
| <span data-ttu-id="96492-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96492-108">Property</span></span>     | <span data-ttu-id="96492-109">型</span><span class="sxs-lookup"><span data-stu-id="96492-109">Type</span></span>   |<span data-ttu-id="96492-110">説明</span><span class="sxs-lookup"><span data-stu-id="96492-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96492-111">Key</span><span class="sxs-lookup"><span data-stu-id="96492-111">key</span></span>|<span data-ttu-id="96492-112">String</span><span class="sxs-lookup"><span data-stu-id="96492-112">String</span></span>|<span data-ttu-id="96492-113">キー。</span><span class="sxs-lookup"><span data-stu-id="96492-113">Key.</span></span>|
|<span data-ttu-id="96492-114">value</span><span class="sxs-lookup"><span data-stu-id="96492-114">value</span></span>|<span data-ttu-id="96492-115">Any</span><span class="sxs-lookup"><span data-stu-id="96492-115">Any</span></span>|<span data-ttu-id="96492-116">任意の JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="96492-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96492-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96492-117">JSON representation</span></span>

<span data-ttu-id="96492-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96492-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
