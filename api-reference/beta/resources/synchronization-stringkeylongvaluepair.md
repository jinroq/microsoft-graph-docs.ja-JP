---
title: stringkeylongvaluepair リソースの種類
description: キーが文字列で、値が Int64 であるキーと値のペアを表します。
localization_priority: Normal
ms.openlocfilehash: 48ca44c70e02be153aaeb5ee1171cd8c60e0fa2d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342761"
---
# <a name="stringkeylongvaluepair-resource-type"></a>stringkeylongvaluepair リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

キーが文字列で、値が Int64 であるキーと値のペアを表します。

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
  "suppressions": []
}
-->
