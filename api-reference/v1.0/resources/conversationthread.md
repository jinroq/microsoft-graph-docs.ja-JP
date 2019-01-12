---
title: conversationThread リソースの種類
description: onversationThread は、投稿のコレクションです。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a1a45f5ac6d26b58f1179616d3a6b9b76c6c1618
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912317"
---
# <a name="conversationthread-resource-type"></a>conversationThread リソースの種類
onversationThread は、[投稿](post.md)のコレクションです。

最後の投稿の受信者コレクションはスレッド全体の集計された受信者です。スレッドの受信者コレクションは増大する可能性があります。スレッドから受信者が削除されると、新しいスレッドが作成されます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[スレッドを一覧表示する](../api/group-list-threads.md) | [conversationThread](conversationthread.md) コレクション |グループのすべてのスレッドを取得します。|
|[スレッドを作成する](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |最初にスレッドを作成して、新しい会話を開始します。グループには、新しい会話、会話スレッド、および投稿が作成されます。|
|[conversationThread を取得する](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |グループに属している特定のスレッドを取得します。 |
|[Update](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |conversationThread オブジェクトを更新します。 |
|[Delete](../api/conversationthread-delete.md) | なし |conversationThread オブジェクトを削除します。 |
|[Reply](../api/conversationthread-reply.md)|なし|新しい投稿のエンティティを作成して、このスレッドに返信します。|
|[投稿を一覧表示する](../api/conversationthread-list-posts.md) |[post](post.md) コレクション| 指定したスレッドの投稿を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。|
|toRecipients|[recipient](recipient.md) collection|スレッドの宛先の受信者。|
|ccRecipients|[recipient](recipient.md) collection|スレッドの CC の受信者。|
|topic|String|会話のトピックです。会話の作成時にこのプロパティを設定できますが、更新することはできません。||
|hasAttachments|Boolean|このスレッド内のいずれかの投稿に添付ファイルが 1 つ以上あるかどうかを示します。|
|lastDeliveredDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|uniqueSenders|String コレクション|このスレッドにメッセージを送信したすべてのユーザー。|
|preview|String|この会話における最新投稿の本文からの短い概要。|
|isLocked|Boolean|スレッドがロックされているかどうかを示します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|投稿|[post](post.md) コレクション| 読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
