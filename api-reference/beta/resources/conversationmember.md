---
title: conversationMember リソース タイプ
description: 会話のユーザーを表します。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379298"
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

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a>関連項目

[aadUserConversationMember](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
