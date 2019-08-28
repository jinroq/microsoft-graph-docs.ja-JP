---
title: conversationMember リソース タイプ
description: 会話のユーザーを表します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca5115922dfb40239b8ca290a39f3c5953d4e4ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973976"
---
# <a name="conversationmember-resource-type"></a>conversationMember リソース タイプ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[chat](chat.md) のユーザーを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャットのメンバーを一覧表示する](../api/conversationmember-list.md) | [conversationmember](conversationmember.md) コレクション | チャットのすべてのメンバーのリストを取得します。|
|[チャットのメンバーを取得する](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | チャットの 1 人のユーザーを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 ユーザーの一意の ID。|
|displayName| string | ユーザーの表示名。 |
|roles| string コレクション | そのユーザーのロール。 |

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->