---
title: Parseexpression Response リソースの種類
description: '[同期スキーマ: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションからの応答を表します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d63a8834640d357e41051750f7f2cd50b8724fee
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620487"
---
# <a name="parseexpressionresponse-resource-type"></a>Parseexpression Response リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Parseexpression](../api/synchronization-synchronizationschema-parseexpression.md)アクションからの応答を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|エラー|publicError|エラーの詳細。式の評価結果でエラーが発生した場合。|
|evaluationResult|文字列コレクション|式の評価によって生成された値のコレクション。|
|evaluationSucceeded|Boolean|`true`評価が成功した場合。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。|
|parsingSucceeded|Boolean|`true`式が正常に解析された場合。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
