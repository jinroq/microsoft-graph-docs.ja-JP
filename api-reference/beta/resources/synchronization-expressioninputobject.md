---
title: 式 Inputobject リソースの種類
description: '[同期スキーマ: parseexpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションが式評価を実行するときに入力テストデータとして使用するオブジェクトを表します。'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 113c38e540b8c41fb3d3156b27f6f5e1f1df42f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007950"
---
# <a name="expressioninputobject-resource-type"></a>式 Inputobject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Parseexpression](../api/synchronization-synchronizationschema-parseexpression.md)アクションが式の評価を実行するときに入力テストデータとして使用するオブジェクトを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|definition|[objectDefinition](synchronization-objectdefinition.md)|Test オブジェクトの定義。|
|properties|[Stringkeyobjectvaluepair](synchronization-stringkeyobjectvaluepair.md)コレクション|Test オブジェクトのプロパティ値を指定します。|

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
