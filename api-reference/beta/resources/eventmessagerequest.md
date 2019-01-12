---
title: eventMessageRequest リソースの種類
description: 会議出席依頼を表すメッセージ。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5350b864ee38774f5b329110de6caf41f23dfe37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981099"
---
# <a name="eventmessagerequest-resource-type"></a>eventMessageRequest リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

会議出席依頼を表すメッセージ。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
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
|categories|String コレクション|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) collection|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|要求された会議の終了時間です。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。|
|hasAttachments|Boolean|メッセージに添付ファイルがあるかどうかを示します。|
|id|String|読み取り専用。|
|importance|String| メッセージの重要度: `Low`、`Normal`、`High`。|
|inferenceClassification|String| 使用可能な値は、`Focused`、`Other` です。|
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|Boolean|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isOutOfDate|Boolean|この会議出席要求がより新しい要求によって古くなっているかどうかを示します。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|location|[Location](location.md)|要求された会議の場所です。|
|meetingMessageType|String| イベント メッセージの種類: `None`、`MeetingRequest`、`MeetingCancelled``MeetingAccepted``MeetingTenativelyAccepted``MeetingDeclined`。|
|parentFolderId|String|メッセージの親 mailFolder の一意識別子。|
|previousEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|要求された会議の前の終了時間です。|
|previousLocation|[Location](location.md)|会議出席依頼の以前の場所。|
|previousStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|要求された会議の前の開始時刻。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|要求された会議の定期的なパターンです。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|要求された会議の開始時刻。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|type|String|要求された会議の種類: `singleInstance`、 `occurence`、 `exception`、 `seriesMaster`。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに特有のメッセージの本文の一部。|
|webLink|String|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) コレクション| 読み取り専用。Null 許容型。|
|イベント|[Event](event.md)| イベント メッセージに関連付けられたイベント。参加者または部屋リソースの前提は、会議出席依頼イベント メッセージが届いたときにイベントを含む予定表を自動的に更新するようにカレンダー アテンダントが設定されていることです。ナビゲーション プロパティ。読み取り専用。|
|extensions|[Extension](extension.md) コレクション| 読み取り専用。Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[eventMessage の取得](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |eventMessage オブジェクトのプロパティとリレーションシップを読み取ります。|
|[添付ファイルを作成します。](../api/eventmessage-post-attachments.md) |[添付ファイル](attachment.md)| 添付ファイル コレクションへの投稿により、新しい添付ファイルを作成します。|
|[添付ファイルを一覧表示する](../api/eventmessage-list-attachments.md) |[Attachment](attachment.md) コレクション| 添付ファイルのオブジェクト コレクションを取得します。|
|[更新する](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |eventMessage オブジェクトを更新します。 |
|[削除](../api/eventmessage-delete.md) | なし |eventMessage オブジェクトを削除します。 |
|[コピー](../api/message-copy.md)|[Message](message.md)||
|[createForward](../api/message-createforward.md)|[Message](message.md)||
|[createReply](../api/message-createreply.md)|[Message](message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)||
|[forward](../api/message-forward.md)|なし|メッセージを転送します。 その後、メッセージは [送信済みアイテム] フォルダーに保存されます。|
|[移動](../api/message-move.md)|[Message](message.md)|メッセージを mailFolder に移動します。|
|[返信](../api/message-reply.md)|なし|メッセージの送信者に返信します。 その後、メッセージは [送信済みアイテム] フォルダーに保存されます。|
|[replyAll](../api/message-replyall.md)|なし|メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[送信](../api/message-send.md)|なし|以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
