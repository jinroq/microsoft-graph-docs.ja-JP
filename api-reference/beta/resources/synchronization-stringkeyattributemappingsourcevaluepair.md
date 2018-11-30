---
title: stringKeyAttributeMappingSourceValuePair リソースの種類
description: キーが文字列であり、値は、attributeMappingSource は、キー/値ペアを表します。
ms.openlocfilehash: 875c593ae652ce763f420d29e5dd4e5e2601bc88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073529"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>stringKeyAttributeMappingSourceValuePair リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

キーが文字列であり、値は、 [attributeMappingSource](synchronization-attributemappingsource.md)は、キー/値ペアを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Key|String|パラメーターの名前です。|
|value|[attributeMappingSource](synchronization-attributemappingsource.md)|パラメーターの値です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

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
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
