---
title: aadUserConversationMember リソース タイプ
description: 会話のユーザーを表します。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: fd326482869d9f72778edc9d4c55996f7aa59045
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236462"
---
# <a name="aaduserconversationmember-resource-type"></a>aadUserConversationMember リソース タイプ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[chat](chat.md) の Azure Active Directory ユーザーを表します。 このタイプは、[conversationMember](conversationmember.md) から継承されています。

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
|userId| string | ユーザーの GUID。 |
|メール| string  | ユーザーの電子メール アドレス。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
