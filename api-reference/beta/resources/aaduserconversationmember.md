---
title: aadUserConversationMember リソース タイプ
description: チャットまたはチャネルの Azure Active Directory ユーザーを表します。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 058164d44ef6d9d6ba6667cf1cb7249bf57c2a83
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633511"
---
# <a name="aaduserconversationmember-resource-type"></a>aadUserConversationMember リソース タイプ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャット](chat.md)または[チャネル](channel.md)の Azure Active Directory ユーザーを表します。 このタイプは、[conversationMember](conversationmember.md) から継承されています。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[メンバーを一覧表示する](../api/conversationmember-list.md) | [conversationmember](conversationmember.md) コレクション | チャットまたはチャネルのすべてのメンバーのリストを取得します。|
|[メンバーを取得する](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | チャットまたはチャネルの 1 人のユーザーを取得します。|
|[メンバーを追加する](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| チャネルにメンバーを追加します。|
|[メンバーを更新する](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| チャネルのメンバーを更新します。|
|[メンバーを削除する](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| チャネルからメンバーを削除します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
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
