---
title: expressionInputObject リソースの種類
description: 'テストの入力データとして使用するオブジェクトを表すとき、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)式の評価を実行するアクションです。'
ms.openlocfilehash: 06b7344f7e6418db0557f2b12dfa7e964b9d5ab7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073332"
---
# <a name="expressioninputobject-resource-type"></a>expressionInputObject リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テストの入力データとして使用するオブジェクトを表すとき、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)式の評価を実行するアクションです。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|definition|[objectDefinition](synchronization-objectdefinition.md)|テスト オブジェクトの定義です。|
|プロパティ|[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)コレクション|テスト オブジェクトのプロパティの値です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->