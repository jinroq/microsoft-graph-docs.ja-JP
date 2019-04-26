---
title: inferenceClassificationOverride リソースの種類
description: 特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。
localization_priority: Normal
ms.openlocfilehash: 8df0f1e5fa34c630c51de7c73234e6092448f867
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567537"
---
# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride リソースの種類

特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Update](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。 |
|[削除](../api/inferenceclassificationoverride-delete.md) | なし |その ID で指定されたオーバーライドを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| 特定の差出人からの着信メッセージを常時分類する方法を指定します。 使用可能な値は`focused`、 `other`、です。|
|id|string| オーバーライドの一意識別子。読み取り専用です。|
|senderEmailAddress|[emailAddress](emailaddress.md)|オーバーライドを作成する対象の差出人のメール アドレス情報。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
