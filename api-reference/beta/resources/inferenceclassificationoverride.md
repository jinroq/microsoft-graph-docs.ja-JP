---
title: inferenceClassificationOverride リソースの種類
description: 特定の送信者からの受信メッセージを常に分類する方法についてのユーザーのオーバーライドを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d01cbeb7b031c3e3b9ed66757a155eca6e33e479
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005766"
---
# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の送信者からの受信メッセージを常に[優先受信トレイ](manage-focused-inbox.md)として分類する方法に対するユーザーのオーバーライドを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Update](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。 |
|[Delete](../api/inferenceclassificationoverride-delete.md) | None |その ID で指定されたオーバーライドを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|classifyAs|string| 特定の差出人からの着信メッセージを常時分類する方法を指定します。可能な値は、`focused`、`other` です。|
|id|string| オーバーライドの一意識別子。読み取り専用です。|
|senderEmailAddress|[emailAddress](emailaddress.md)|オーバーライドを作成する対象の差出人のメール アドレス情報。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
