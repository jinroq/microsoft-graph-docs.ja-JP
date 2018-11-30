---
title: stringKeyObjectValuePair リソースの種類
description: キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。
ms.openlocfilehash: ae536b2aab87b9920c2afcbe324e30b5f5380dbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070018"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>stringKeyObjectValuePair リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Key|String|キー。|
|value|Any|任意の JSON オブジェクト。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

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
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->