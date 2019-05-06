---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4c2631d0ba4883160c443000fa2ecb0e1853523d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339848"
---
# <a name="chatmessage-resource-type"></a>chatMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネル メッセージを一覧表示する](../api/channel-list-messages.md) | [chatmessage](chatmessage.md) コレクション | チャネルのすべてのルート メッセージの一覧を取得します。|
|[チャネル メッセージを取得する](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | チャネルからのルート メッセージを 1 件取得します。|
|[メッセージへの返信を一覧表示する](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md) コレクション| チャネル内のメッセージへの返信すべての一覧を取得します。|
|[メッセージへの返信を取得する](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| チャネル内のメッセージへの返信を 1 件取得します。|
|[チャネル内でメッセージを送信する](../api/channel-post-chatmessage.md) | [chatmessage](chatmessage.md)| チャネル内で新しい最上位レベルのメッセージを作成します。|
|[チャネル内のメッセージに返信する](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| チャネル内の既存メッセージに返信します。|
|[チャット内のメッセージを一覧表示する](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 1 対 1 またはグループ チャットでのメッセージを取得します。 |
|[チャット内のメッセージを取得する](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | チャット内の 1 つのメッセージを取得します。 |


## <a name="properties"></a>Properties
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 メッセージの一意の ID。|
|replyToId| string | スレッドの親メッセージ/ルート メッセージの ID。 (チャットではなく、チャネルのメッセージにのみ適用) |
|差出人|[identitySet](identityset.md)| 読み取り専用です。 メッセージの送信者の詳細。|
|etag| string | メッセージのバージョン番号。 |
|messageType|String|メッセージの種類。現在サポートされている値は message、chatEvent、Typing。|
|createdDateTime|dateTimeOffset|読み取り専用です。 メッセージ作成時のタイムスタンプ。|
|lastModifiedDateTime|dateTimeOffset|読み取り専用です。 メッセージ編集/更新時のタイムスタンプ。|
|deletedDateTime|dateTimeOffset|読み取り専用です。 メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。 |
|件名|string| プレーン テキストでの、メッセージの件名です。|
|本文|[itemBody](itembody.md)|メッセージのコンテンツのプレーンテキスト/HTML 表記。 表記は、本文内の contentType によって指定されます。 メッセージに [chatMessageMention ](chatmessagemention.md) が含まれている場合、コンテンツは常に HTML で表示されます。 |
|summary|string| プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト。 チャット メッセージではなく、チャネル メッセージにのみ適用されます。 |
|attachments|[chatMessageAttachment](chatmessageattachment.md) コレクション |添付ファイル。 添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。 |
|mentions|[chatMessageMention](chatmessagemention.md) コレクション| メッセージに記載されているエンティティの一覧。 現在、user、bot、team、channel がサポートされています。|
|importance| string | メッセージの重要度: 通常、高。|
|reactions| [chatMessageReaction](chatmessagereaction.md) コレクション | このメッセージに対する反応 (例: いいね!)。|
|locale|string|クライアントに設定されたメッセージのロケール。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "deleted": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
