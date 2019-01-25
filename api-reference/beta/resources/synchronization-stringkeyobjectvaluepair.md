---
title: stringKeyObjectValuePair リソースの種類
description: キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516967"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="ebb4f-104">stringKeyObjectValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebb4f-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebb4f-105">キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。</span><span class="sxs-lookup"><span data-stu-id="ebb4f-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="ebb4f-106">これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="ebb4f-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="ebb4f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb4f-107">Properties</span></span>
| <span data-ttu-id="ebb4f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb4f-108">Property</span></span>     | <span data-ttu-id="ebb4f-109">型</span><span class="sxs-lookup"><span data-stu-id="ebb4f-109">Type</span></span>   |<span data-ttu-id="ebb4f-110">説明</span><span class="sxs-lookup"><span data-stu-id="ebb4f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebb4f-111">Key</span><span class="sxs-lookup"><span data-stu-id="ebb4f-111">key</span></span>|<span data-ttu-id="ebb4f-112">String</span><span class="sxs-lookup"><span data-stu-id="ebb4f-112">String</span></span>|<span data-ttu-id="ebb4f-113">キー。</span><span class="sxs-lookup"><span data-stu-id="ebb4f-113">Key.</span></span>|
|<span data-ttu-id="ebb4f-114">value</span><span class="sxs-lookup"><span data-stu-id="ebb4f-114">value</span></span>|<span data-ttu-id="ebb4f-115">Any</span><span class="sxs-lookup"><span data-stu-id="ebb4f-115">Any</span></span>|<span data-ttu-id="ebb4f-116">任意の JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="ebb4f-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebb4f-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebb4f-117">JSON representation</span></span>

<span data-ttu-id="ebb4f-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ebb4f-118">The following is a JSON representation of the resource.</span></span>

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
