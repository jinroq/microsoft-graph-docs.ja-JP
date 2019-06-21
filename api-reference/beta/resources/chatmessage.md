---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 269041dece2ab626c5f3d0ecccbf70d62c296ede
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084048"
---
# <a name="chatmessage-resource-type"></a>chatMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。
メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネル メッセージを一覧表示する](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) コレクション | チャネルのすべてのルート メッセージの一覧。|
|[チャネル メッセージを取得する](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | チャネルからのルート メッセージを 1 件取得します。|
|[メッセージへの返信を一覧表示する](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) コレクション| チャネル内のメッセージへの返信すべての一覧。|
|[メッセージへの返信を取得する](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| チャネル内のメッセージへの返信を 1 件取得します。|
|[チャネルでの chatMessage の作成](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| チャネル内で新しい最上位レベルのメッセージを作成します。|
|[チャネル内のメッセージに返信する](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| チャネル内の既存メッセージに返信します。|
|[チャット内のメッセージを一覧表示する](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 1 対 1 またはグループ チャットでのメッセージを一覧表示する。 |
|[チャット内のメッセージを取得する](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | チャット内の 1 つのメッセージを取得します。 |
|[ホストされているすべての画像を一覧表示する](../api/chatmessagehostedimage-list-hostedimages.md) | [hostedimage](../resources/chatmessagehostedimage.md)コレクション| メッセージ内のホストされているすべての画像を取得します。|
|[ホストされている画像を取得する](../api/chatmessagehostedimage-get.md) | [hostedImage](../resources/chatmessagehostedimage.md) | メッセージからホストされている画像を取得します。|
|[ホストされている画像バイトを取得する](../api/chatmessagehostedimage-getbytes.md) | バイナリ画像データ | メッセージからホストされている画像のバイナリ画像データを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 メッセージの一意の ID。|
|replyToId| string | 読み取り専用です。 スレッドの親メッセージ/ルート メッセージの ID。 (チャットではなく、チャネルのメッセージにのみ適用) |
|差出人|[identitySet](identityset.md)| 読み取り専用です。 メッセージの送信者の詳細。|
|etag| string | 読み取り専用です。 メッセージのバージョン番号。 |
|messageType|chatMessageType|メッセージの種類。 使用可能な値: `message`。|
|createdDateTime|dateTimeOffset|読み取り専用です。 メッセージ作成時のタイムスタンプ。|
|lastModifiedDateTime|dateTimeOffset|読み取り専用です。 メッセージ編集/更新時のタイムスタンプ。|
|deletedDateTime|dateTimeOffset|読み取り専用です。 メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。 |
|件名|string| プレーン テキストでの、メッセージの件名です。|
|本文|[itemBody](itembody.md)|メッセージのコンテンツのプレーンテキスト/HTML 表記。 表記は、本文内の contentType によって指定されます。 メッセージに [chatMessageMention ](chatmessagemention.md) が含まれている場合、コンテンツは常に HTML で表示されます。 |
|summary|string| プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト。 チャット メッセージではなく、チャネル メッセージにのみ適用されます。 |
|attachments|[chatMessageAttachment](chatmessageattachment.md) コレクション |添付ファイル。 添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。 |
|mentions|[chatMessageMention](chatmessagemention.md) コレクション| メッセージに記載されているエンティティの一覧。 現在、user、bot、team、channel がサポートされています。|
|importance| chatMessageImportance | メッセージの重要度です。 使用可能な値: `normal`、`high`、`urgent`。|
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
