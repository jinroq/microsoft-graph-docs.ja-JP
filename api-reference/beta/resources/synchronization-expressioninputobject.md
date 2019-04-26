---
title: 式 inputobject リソースの種類
description: '[同期スキーマ: parseexpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションが式評価を実行するときに入力テストデータとして使用するオブジェクトを表します。'
localization_priority: Normal
ms.openlocfilehash: 90d394639de7050eaed3b696dd8526e144cac03d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345602"
---
# <a name="expressioninputobject-resource-type"></a>式 inputobject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[parseexpression](../api/synchronization-synchronizationschema-parseexpression.md)アクションが式の評価を実行するときに入力テストデータとして使用するオブジェクトを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|definition|[objectdefinition](synchronization-objectdefinition.md)|test オブジェクトの定義。|
|properties|[stringkeyobjectvaluepair](synchronization-stringkeyobjectvaluepair.md)コレクション|test オブジェクトのプロパティ値を指定します。|

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
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
