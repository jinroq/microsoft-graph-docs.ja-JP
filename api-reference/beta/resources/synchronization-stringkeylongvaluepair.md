---
title: stringKeyLongValuePair リソースの種類
description: キーが文字列であり、値は、int64 型のキー/値ペアを表します。
localization_priority: Normal
ms.openlocfilehash: 97ca9f4f7b4079311a1ce6996fde0472c527e7f9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518304"
---
# <a name="stringkeylongvaluepair-resource-type"></a>stringKeyLongValuePair リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

キーが文字列であり、値は、int64 型のキー/値ペアを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Key|String|キー。|
|value|Int64|値|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeylongvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
