---
title: stringkeystringvaluepair リソースの種類
description: キーが文字列で、値が文字列であるキーと値のペアを表します。
localization_priority: Normal
ms.openlocfilehash: f91d63ee4b4d3b0328bbb6fbe58c74ec8f78c5b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526273"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="7bac9-103">stringkeystringvaluepair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7bac9-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bac9-104">キーが文字列で、値が文字列であるキーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="7bac9-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="7bac9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bac9-105">Properties</span></span>
| <span data-ttu-id="7bac9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bac9-106">Property</span></span>     | <span data-ttu-id="7bac9-107">型</span><span class="sxs-lookup"><span data-stu-id="7bac9-107">Type</span></span>   |<span data-ttu-id="7bac9-108">説明</span><span class="sxs-lookup"><span data-stu-id="7bac9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bac9-109">Key</span><span class="sxs-lookup"><span data-stu-id="7bac9-109">key</span></span>|<span data-ttu-id="7bac9-110">String</span><span class="sxs-lookup"><span data-stu-id="7bac9-110">String</span></span>|<span data-ttu-id="7bac9-111">キー。</span><span class="sxs-lookup"><span data-stu-id="7bac9-111">Key.</span></span>|
|<span data-ttu-id="7bac9-112">value</span><span class="sxs-lookup"><span data-stu-id="7bac9-112">value</span></span>|<span data-ttu-id="7bac9-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7bac9-113">String</span></span>|<span data-ttu-id="7bac9-114">値。</span><span class="sxs-lookup"><span data-stu-id="7bac9-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bac9-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7bac9-115">JSON representation</span></span>

<span data-ttu-id="7bac9-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7bac9-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
