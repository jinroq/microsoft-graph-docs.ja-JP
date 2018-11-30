---
title: parseExpressionResponse リソースの種類
description: '応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。'
ms.openlocfilehash: 625df0ca16135eaa35c5b679c79dea582c4012e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073524"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|エラー|odata.error|エラーの詳細、式の評価でエラーが発生する場合。|
|evaluationResult|String コレクション|式の評価によって生成された値のコレクションです。|
|evaluationSucceeded|ブール値|`true`場合は、評価が正常に完了しました。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。|
|parsingSucceeded|ブール値|`true`場合は、式が正しく解析されました。|

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->