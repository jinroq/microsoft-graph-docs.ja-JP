---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 チャットメッセージは、ルートチャットメッセージ、またはチャットメッセージの**replyToId**プロパティによって定義されたスレッドの一部にすることができます。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: a29afea30f0ea1d75f5c7ce1a0713976f10cc298
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677121"
---
# <a name="chatmessage-resource-type"></a>chatMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。 チャットメッセージは、ルートチャットメッセージ、またはチャットメッセージの**replyToId**プロパティで定義されている応答スレッドの一部にすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネルチャットメッセージの一覧表示](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) コレクション | チャネル内のすべてのルートチャットメッセージのリスト。|
|[チャネルデルタで chatMessages を取得する](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | チャネル内の増分チャットメッセージを取得します。 |
|[チャネルのチャットメッセージを取得する](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | チャネルから1つのルートチャットメッセージを取得します。|
|[ChatMessage への返信を一覧表示する](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) コレクション| チャネル内のチャットメッセージへのすべての返信の一覧。|
|[ChatMessage への返信を取得する](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| チャネル内のチャットメッセージに対して1回の返信を取得します。|
|[チャネルでの chatMessage の作成](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| チャネルに新しいトップレベルチャットメッセージを作成します。|
|[チャネル内の chatMessage に返信する](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| チャネル内の既存のチャットメッセージに返信します。|
|[チャットでの chatMessage の作成](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| 既存の1:1 またはグループチャットの会話でチャットメッセージを送信します。|
|[チャットのチャットメッセージを一覧表示する](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | チャットメッセージを1:1 またはグループチャットで一覧表示します。 |
|[チャットでの chatMessage の取得](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | チャットで1つのチャットメッセージを取得します。 |
|[ホストされているすべての画像を一覧表示する](../api/chatmessagehostedimage-list-hostedimages.md) | [Hostedimage](../resources/chatmessagehostedimage.md)コレクション| チャットメッセージ内のすべてのホストされた画像を取得します。|
|[ホストされた画像を取得する](../api/chatmessagehostedimage-get.md) | [hostedImage](../resources/chatmessagehostedimage.md) | チャットメッセージからホストされているイメージを取得します。|
|[ホストされた画像バイトを取得する](../api/chatmessagehostedimage-getbytes.md) | バイナリイメージデータ | チャットメッセージからホストされているイメージのバイナリイメージデータを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用。 メッセージの一意の Id。|
|replyToId| string | 読み取り専用です。 スレッドの親チャットメッセージまたはルートチャットメッセージの Id。 (チャットではないチャネルのチャットメッセージにのみ適用されます) |
|from|[identitySet](identityset.md)| 読み取り専用です。 チャットメッセージの送信者の詳細。|
|etag| string | 読み取り専用です。 チャットメッセージのバージョン番号。 |
|messageType|chatMessageType|チャットメッセージの種類。 使用可能な値は`message`次のとおりです。|
|createdDateTime|dateTimeOffset|読み取り専用です。 チャットメッセージが作成された時点のタイムスタンプ。|
|lastModifiedDateTime|dateTimeOffset|読み取り専用です。 チャットメッセージが作成または編集されたときのタイムスタンプ (チャネルでのルートチャットメッセージの場合)、または反応が追加または削除されたとき。 |
|deletedDateTime|dateTimeOffset|読み取り専用です。 チャットメッセージが削除されたタイムスタンプ、または削除されていない場合は null。 |
|subject|string| テキスト形式のチャットメッセージの件名。|
|body|[itemBody](itembody.md)|チャットメッセージの内容をプレーンテキストまたは HTML で表したものです。 表記は、本文内の contentType によって指定されます。 チャットメッセージに[chatMessageMention](chatmessagemention.md)が含まれている場合、コンテンツは常に HTML 形式です。 |
|summary|string| プッシュ通知および要約ビューに使用したり、ビューに戻したりすることができるチャットメッセージの概要テキスト。 チャットのチャットメッセージではなく、チャネルチャットメッセージのみに適用されます。 |
|attachments|[chatMessageAttachment](chatmessageattachment.md) コレクション |添付ファイル。 添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。 |
|mentions|[chatMessageMention](chatmessagemention.md) コレクション| チャットメッセージで言及されているエンティティのリスト。 現在、user、bot、team、channel がサポートされています。|
|importance| chatMessageImportance 度 | チャットメッセージの重要度。 使用可能な値: `normal`、`high`、`urgent`。|
|reactions| [chatMessageReaction](chatmessagereaction.md) コレクション | このチャットメッセージの反応 (たとえば、など)。|
|locale|string|クライアントによって設定されたチャットメッセージのロケール。|

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
