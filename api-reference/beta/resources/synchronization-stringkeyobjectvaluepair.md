---
title: stringKeyObjectValuePair リソースの種類
description: キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。
localization_priority: Normal
ms.openlocfilehash: 8545a4ef5a4931d3b886c95b4f39218bc418f53d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831452"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>stringKeyObjectValuePair リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

キーが文字列であり、値は、任意の JSON オブジェクトのキー/値ペアを表します。 これは、OData オープン型という名前のプロパティを要求する`value`は有効な JSON オブジェクト。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
