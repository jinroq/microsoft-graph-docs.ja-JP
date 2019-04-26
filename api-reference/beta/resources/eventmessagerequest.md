---
title: eventmessagerequest リソースの種類
description: 会議出席依頼を表すメッセージ。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ead65f036fe5537b7e349124b2771eff575be22f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333955"
---
# <a name="eventmessagerequest-resource-type"></a>eventmessagerequest リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議出席依頼を表すメッセージ。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|メッセージの BCC 受信者。|
|body|[itemBody](itembody.md)|メッセージの本文。|
|bodyPreview|String|メッセージ本文の最初の 255 文字。|
|categories|String collection|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) コレクション|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|要求された会議の終了時刻。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。|
|hasAttachments|Boolean|メッセージに添付ファイルがあるかどうかを示します。|
|id|String|読み取り専用です。|
|importance|String| メッセージの重要度: `Low`、`Normal`、`High`。|
|inferenceClassification|String| 可能な値は、`Focused`、`Other` です。|
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|Boolean|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isOutOfDate|Boolean|この会議出席要求がより新しい要求によって古くなっているかどうかを示します。|
|isRead|ブール値|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|ブール値|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|location|[Location](location.md)|要求された会議の場所。|
|meetingMessageType|String| イベント メッセージの種類: `none`、`meetingRequest`、`meetingCancelled``meetingAccepted``meetingTentativelyAccepted``meetingDeclined`。|
|parentFolderId|String|メッセージの親 mailFolder の一意識別子。|
|前の enddatetime|[DateTimeTimeZone](datetimetimezone.md)|要求された会議の前回の終了時刻。|
|previousLocation|[Location](location.md)|会議出席依頼の以前の場所。|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)|要求された会議の前回の開始時刻。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|要求された会議の定期的なパターン。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|要求された会議の開始時刻。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|type|String|要求された会議の`singleInstance`種類`occurence`: `exception`、 `seriesMaster`、、。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに特有のメッセージの本文の一部。|
|webLink|String|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) コレクション| 読み取り専用。Null 許容型。|
|イベント|[Event](event.md)| イベント メッセージに関連付けられたイベント。参加者または部屋リソースの前提は、会議出席依頼イベント メッセージが届いたときにイベントを含む予定表を自動的に更新するようにカレンダー アテンダントが設定されていることです。ナビゲーション プロパティ。読み取り専用。|
|extensions|[Extension](extension.md) コレクション| 読み取り専用です。 Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[eventMessage の取得](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |eventMessage オブジェクトのプロパティとリレーションシップを読み取ります。|
|[添付ファイルの作成](../api/eventmessage-post-attachments.md) |[Attachment](attachment.md)| 添付ファイル コレクションへの投稿により、新しい添付ファイルを作成します。|
|[添付ファイルを一覧表示する](../api/eventmessage-list-attachments.md) |[Attachment](attachment.md) コレクション| 添付ファイルのオブジェクト コレクションを取得します。|
|[更新する](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |eventMessage オブジェクトを更新します。 |
|[削除](../api/eventmessage-delete.md) | None |eventMessage オブジェクトを削除します。 |
|[コピー](../api/message-copy.md)|[Message](message.md)||
|[createForward](../api/message-createforward.md)|[Message](message.md)||
|[createReply](../api/message-createreply.md)|[Message](message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)||
|[forward](../api/message-forward.md)|なし|メッセージを転送します。 その後、メッセージは [送信済みアイテム] フォルダーに保存されます。|
|[move](../api/message-move.md)|[Message](message.md)|メッセージを mailfolder に移動します。|
|[返信](../api/message-reply.md)|なし|メッセージの送信者に replys を送信します。 その後、メッセージは [送信済みアイテム] フォルダーに保存されます。|
|[replyAll](../api/message-replyall.md)|なし|メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[送信](../api/message-send.md)|なし|以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
