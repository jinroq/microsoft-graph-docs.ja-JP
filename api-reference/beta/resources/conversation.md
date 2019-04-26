---
title: 会話リソースの種類
description: 会話はスレッドのコレクションであり、スレッドにはそのスレッドへの投稿が含まれています。 会話内のすべてのスレッドと投稿は同じ件名を共有します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: db7c8822a3d91369554007656baed171ae81b1fd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341245"
---
# <a name="conversation-resource-type"></a>会話リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会話は[スレッド](conversationthread.md)のコレクションです。スレッドにはそのスレッドへの投稿が含まれています。会話のすべてのスレッドと投稿は同じ件名を共有します。

このリソースは、[変更通知](/graph/webhooks)のサブスクライブをサポートしています。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[会話を一覧表示する](../api/group-list-conversations.md) | [conversation](conversation.md) コレクション |このグループの会話の一覧を取得します。|
|[Create](../api/group-post-conversations.md) |[conversation](conversation.md)| スレッドと投稿を含めて、新しい会話を作成します。|
|[会話を取得する](../api/conversation-get.md) | [conversation](conversation.md) |会話オブジェクトのプロパティと関係を読み取ります。|
|[削除](../api/conversation-delete.md) | なし |conversation オブジェクトを削除します。 |
|[会話スレッドを一覧表示する](../api/conversation-list-threads.md) |[conversationThread](conversationthread.md) コレクション| グループの会話のすべてのスレッドを取得します。|
|[会話スレッドを作成する](../api/conversation-post-threads.md) |[conversationThread](conversationthread.md) コレクション| 指定した会話にスレッドを作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|hasAttachments|Boolean|この会話内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。|
|id|String|会話の一意識別子。読み取り専用です。|
|lastDeliveredDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|preview|String|この会話における最新投稿の本文からの短い概要。|
|topic|String|会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。|
|uniqueSenders|String collection|この会話にメッセージを送信したすべてのユーザーです。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|threads|[conversationThread](conversationthread.md) コレクション|会話内のすべての会話スレッドのコレクションです。ナビゲーションのプロパティです。読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
