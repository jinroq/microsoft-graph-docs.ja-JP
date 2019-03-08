---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458660"
---
# <a name="chatmessage-resource-type"></a>chatMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チャネル](channel.md)またはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[チャネル メッセージを一覧表示する](../api/channel-list-messages.md) | [chatmessage](chatmessage.md) コレクション | チャネルのすべてのルート メッセージの一覧を取得します。|
|[チャネル メッセージを取得する](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | チャネルからのルート メッセージを 1 件取得します。|
|[メッセージへの返信を一覧表示する](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md) コレクション| チャネル内のメッセージへの返信すべての一覧を取得します。|
|[メッセージへの返信を取得する](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| チャネル内のメッセージへの返信を 1 件取得します。|
|[チャネル内でメッセージを送信する](../api/channel-post-chatmessage.md) | [chatmessage](chatmessage.md)| チャネル内で新しい最上位レベルのメッセージを作成します。|
|[チャネル内のメッセージに返信する](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| チャネル内の既存メッセージに返信します。|


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 メッセージの一意の ID。|
|replyToId| string | スレッドの親メッセージ/ルート メッセージの ID |
|from|[identitySet](identityset.md)| メッセージの送信者の詳細|
|etag| string | メッセージのバージョン番号 |
|messageType|String|メッセージの種類。現在サポートされている値: message、chatEvent、Typing|
|createdDateTime|dateTimeOffset|読み取り専用です。 メッセージ作成時のタイムスタンプ|
|lastModifiedDateTime|dateTimeOffset|読み取り専用です。 メッセージ編集/更新時のタイムスタンプ|
|deleted|Boolean|メッセージが削除済み (回復可能) かどうかを示します。|
|deletedDateTime|dateTimeOffset|読み取り専用です。 メッセージ削除時のタイムスタンプ |
|subject|string|メッセージの件名。 省略可能|
|body|[itemBody](itembody.md)|メッセージのコンテンツのプレーンテキスト/HTML 表記。 既定ではプレーンテキストを返しますが、クエリ パラメーターの一部としてアプリケーションで HTML を選択できます|
|summary|string|プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト|
|mentions|[chatMessageMention](chatmention.md) コレクション| メッセージに記載されているエンティティの一覧。 現在、user、bot、team、channel がサポートされています|
|importance| string | メッセージの重要度: 通常、高|
|reactions| [chatMessageReaction](chatreaction.md) コレクション | このメッセージに対する反応 (例: いいね!)|
|locale|string|クライアントに設定されたメッセージのロケール|
|attachments|[chatMessageAttachment](chatattachment.md) コレクション |添付ファイル|


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
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
