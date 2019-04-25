---
title: stringkeyobjectvaluepair リソースの種類
description: キーが文字列で、値が任意の JSON オブジェクトであるキーと値のペアを表します。 これは、有効な JSON オブジェクトであるという名前の`value`プロパティがあると想定される OData オープン型です。
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523211"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="5cfba-104">stringkeyobjectvaluepair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5cfba-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cfba-105">キーが文字列で、値が任意の JSON オブジェクトであるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="5cfba-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="5cfba-106">これは、有効な JSON オブジェクトであるという名前の`value`プロパティがあると想定される OData オープン型です。</span><span class="sxs-lookup"><span data-stu-id="5cfba-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="5cfba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cfba-107">Properties</span></span>
| <span data-ttu-id="5cfba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cfba-108">Property</span></span>     | <span data-ttu-id="5cfba-109">型</span><span class="sxs-lookup"><span data-stu-id="5cfba-109">Type</span></span>   |<span data-ttu-id="5cfba-110">説明</span><span class="sxs-lookup"><span data-stu-id="5cfba-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cfba-111">Key</span><span class="sxs-lookup"><span data-stu-id="5cfba-111">key</span></span>|<span data-ttu-id="5cfba-112">String</span><span class="sxs-lookup"><span data-stu-id="5cfba-112">String</span></span>|<span data-ttu-id="5cfba-113">キー。</span><span class="sxs-lookup"><span data-stu-id="5cfba-113">Key.</span></span>|
|<span data-ttu-id="5cfba-114">value</span><span class="sxs-lookup"><span data-stu-id="5cfba-114">value</span></span>|<span data-ttu-id="5cfba-115">任意</span><span class="sxs-lookup"><span data-stu-id="5cfba-115">Any</span></span>|<span data-ttu-id="5cfba-116">任意の JSON オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="5cfba-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cfba-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5cfba-117">JSON representation</span></span>

<span data-ttu-id="5cfba-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5cfba-118">The following is a JSON representation of the resource.</span></span>

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
