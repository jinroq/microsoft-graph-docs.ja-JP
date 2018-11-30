---
title: chatMessage リソースの種類
description: チャネルまたはチャットのエンティティ内で個別のチャット メッセージを表します。 メッセージは、ルートのメッセージまたはメッセージ内の**replyToId**プロパティで定義されているスレッドの一部にできます。
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066604"
---
# <a name="chatmessage-resource-type"></a>chatMessage リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[チャネル](channel.md)またはチャットのエンティティ内で個別のチャット メッセージを表します。 メッセージは、ルートのメッセージまたはメッセージ内の**replyToId**プロパティで定義されているスレッドの一部にできます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[リストのチャネルのメッセージ](../api/channel-list-messages.md) | [chatmessage](chatmessage.md)コレクション | チャネルでは、ルートのすべてのメッセージの一覧を取得します。|
|[チャネル取得メッセージ](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | チャンネルから 1 つのルートのメッセージを取得します。|
|[メッセージに対する返信の一覧](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md)コレクション| チャネルでのメッセージに対する返信をすべての一覧を取得します。|
|[メッセージへの応答を取得します。](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| チャネル内のメッセージに 1 つの返信を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用。 メッセージの一意の ID です。|
|replyToId| 文字列 | スレッドの親メッセージとルートのメッセージの id |
|from|[identitySet](identityset.md)| メッセージの送信者の詳細|
|etag| 文字列 | メッセージのバージョン番号 |
|messageType|String|サポートされているメッセージでは、現在の type の値: メッセージ、chatEvent を入力します。|
|createdDateTime|dateTimeOffset|読み取り専用です。 メッセージが作成された日時のタイムスタンプ|
|lastModifiedDateTime|dateTimeOffset|読み取り専用です。 メッセージが編集更新をされたときのタイムスタンプ|
|isDeleted|ブール|メッセージをソフト削除されている場合を表します。|
|deletedDateTime|dateTimeOffset|読み取り専用です。 タイムスタンプは、メッセージが削除されました |
|subject|文字列|メッセージの件名です。 省略可能|
|body|[itemBody](itembody.md)|メッセージのコンテンツのプレーン テキストと HTML 形式です。 プレーン テキストを返します既定では、アプリケーションは、クエリ パラメーターの一部として HTML を選択できます。|
|概要|文字列|プッシュ通知し、サマリー ・ ビューまたはフォール バック ・ ビューの使用できるメッセージの概要のテキスト|
|mentions|[chatMessageMention](chatmention.md)コレクション| メッセージに記載されているエンティティの一覧です。 チャネル、ユーザー、ボット、チームが現在サポートしています|
|importance| 文字列 | メッセージの重要度: 高、通常|
|反力| [chatMessageReaction](chatreaction.md)コレクション | このメッセージの反応 (たとえばなど)|
|locale|文字列|クライアントが設定するメッセージのロケール|
|attachments|[chatMessageAttachment](chatattachment.md)コレクション |添付ファイル|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
