---
title: eventMessage リソースの種類
description: 'メッセージは会議出席依頼、キャンセル、応答 (承諾、仮受諾、辞退のいずれか) を表します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11b38679916f85d9606989442ffb53e41c51c855
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342325"
---
# <a name="eventmessage-resource-type"></a>eventMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メッセージは会議出席依頼、キャンセル、応答 (承諾、仮受諾、辞退のいずれか) を表します。 

**eventmessage**エンティティは[message](message.md)から派生し、 [eventmessagの](eventmessagerequest.md)場合は**eventmessage**から派生し、会議出席依頼を表します。 **meetingMessageType** プロパティはイベント メッセージの種類を特定します。

開催者またはアプリが会議出席依頼を送信すると、その会議出席依頼が出席者の受信ボックスに **meetingMessageType** が **meetingRequest** の **eventMessage** インスタンスとして届きます。 また、Outlook では出席者の予定表に **event** インスタンスが自動的に作成され、**showAs** プロパティは **tentative** になります。 

出席者のメールボックスで関連付けられているイベントのプロパティを取得するために、[イベント メッセージ取得の例](../api/eventmessage-get.md#request-2)で示されているように、アプリで **eventMessage** の **event** ナビゲーション プロパティを使用できます。 また、アプリでは、イベントを承諾、[仮](../api/event-tentativelyaccept.md)承諾、または[拒否](../api/event-decline.md)することによって、プログラムによって、出席者の代わりにイベントに応答することもできます。 [](../api/event-accept.md)

会議出席依頼とは別に、イベント開催者が会議をキャンセルした結果として、または開催者の受信トレイで、会議出席依頼への返信が出席者によって行われたときに、出席者の受信トレイフォルダーに**eventmessage**インスタンスが見つかることがあります。 アプリはメッセージ上と同様にイベント メッセージ上でも動作しますが、わずかな違いがあります。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です  

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventMessage"
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
  "conversationIndex": "binary",
  "createdDateTime": "DateTimeOffset",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": "Boolean",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": {"@odata.type": "microsoft.graph.meetingMessageType"},
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "recurrence": {"@odata.type": "microsoft.graph.patternedrecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "UnsubscribeData": "string",
  "UnsubscribeEnabled": true,
  "webLink": "string"
}

```

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|メッセージの BCC 受信者。|
|body|[itemBody](itembody.md)|メッセージの本文。HTML 形式またはテキスト形式にできます。|
|bodyPreview|String|メッセージ本文の最初の 255 文字。テキスト形式です。 |
|categories|String コレクション|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) collection|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|conversationIndex|Binary|電子メールが属している会話のインデックス。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|要求された会議の終了時刻。|
|flag|[followUpFlag](followupflag.md)|メッセージのステータス、開始日、期限、または完了日を示すフラグ値。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。|
|hasAttachments|ブール型|メッセージに添付ファイルがあるかどうかを示します。|
|id|文字列型 (String)||
|importance|String| メッセージの重要度: `low`、`normal`、`high`。|
|inferenceClassification|String| 使用可能な値は、`focused`、`other` です。|
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) コレクション | [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) によって定義された、メッセージ ヘッダーのコレクション。メッセージが送信者から受信者に到達するまでに辿ったネットワーク パスの詳細を説明します。 読み取り専用。|
|internetMessageId |String |[RFC5322](https://www.ietf.org/rfc/rfc5322.txt) で指定されている形式のメッセージ ID。 |
|isAllDay |Boolean|イベントが 1 日中続くかどうかを示します。 このプロパティを調整するには、イベントの**startDateTime**および**enddatetime**プロパティの調整も必要です。|
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|Boolean|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isOutOfDate|Boolean|この会議出席要求がより新しい要求によって古くなっているかどうかを示します。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|location|[location](location.md)|要求された会議の場所。|
|meetingMessageType|String| イベント メッセージの種類: `none`、`meetingRequest`、`meetingCancelled``meetingAccepted``meetingTentativelyAccepted``meetingDeclined`。|
|parentFolderId|文字列|メッセージの親 mailFolder の一意識別子。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|要求された会議の定期的なパターン。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|要求された会議の開始時刻。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|type|String|要求された会議の`singleInstance`種類`occurence`: `exception`、 `seriesMaster`、、。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに特有のメッセージの本文の一部。|
|UnsubscribeData|String|List-Unsubscribe ヘッダーに基づいて解析された有効なエントリ。UnsubscribeEnabled プロパティが true の場合、これは List-Unsubscribe ヘッダー内の mail コマンドのデータです。|
|UnsubscribeEnabled|Boolean|メッセージが登録解除に対して有効になっているかどうかを示します。list-Unsubscribe ヘッダーが rfc-2369 に準拠している場合、その値は True です。|
|webLink|文字列|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|メッセージの[fileattachment](fileattachment.md)、 [itemattachment](itemattachment.md)、および[referenceattachment](referenceattachment.md)添付ファイルのコレクションです。 読み取り専用です。 Null 許容型。|
|event|[event](event.md)| イベント メッセージに関連付けられたイベント。参加者または部屋リソースの前提は、会議出席依頼イベント メッセージが届いたときにイベントを含む予定表を自動的に更新するようにカレンダー アテンダントが設定されていることです。ナビゲーション プロパティ。読み取り専用。|
|extensions|[extension](extension.md) コレクション| eventMessage に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| eventMessage に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| eventMessage に対して定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[eventMessage の取得](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |eventMessage オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |eventMessage オブジェクトを更新します。|
|[削除](../api/eventmessage-delete.md) | None |eventMessage オブジェクトを削除します。|
|[copy](../api/message-copy.md)|[message](message.md)|メッセージをフォルダーにコピーします。|
|[createForward](../api/message-createforward.md)|[message](message.md)|転送メッセージの下書きを作成します。その後、下書きを[更新](../api/message-update.md)または[送信](../api/message-send.md)できます。|
|[createReply](../api/message-createreply.md)|[message](message.md)|返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message-update.md)または[送信](../api/message-send.md)できます。|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|全員に返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message-update.md)または[送信](../api/message-send.md)できます。|
|[forward](../api/message-forward.md)|なし|メッセージを転送します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[move](../api/message-move.md)|[message](message.md)|メッセージをフォルダーに移動します。これにより、宛先フォルダーにメッセージの新しいコピーが作成されます。|
|[返信](../api/message-reply.md)|なし|メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[replyAll](../api/message-replyall.md)|なし|メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[送信](../api/message-send.md)|なし|以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[unsubscribe](../api/message-unsubscribe.md)|なし|List-Unsubscribe ヘッダー内の最初の mailto コマンドで指定されたデータとアドレスを使用して、メッセージを送信します。|
|**Attachments**| | |
|[添付ファイルを一覧表示する](../api/eventmessage-list-attachments.md) |[attachment](attachment.md) コレクション| eventMessage のすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| 添付ファイル コレクションへの投稿により、eventMessage に新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前で識別されるオープン拡張機能を取得します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |新規または既存の eventMessage に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ eventMessage の取得](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む eventMessage を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | 新規または既存の eventMessage に、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ eventMessage の取得](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | `$expand` を使用して、複数値の拡張プロパティを含む eventMessage を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/eventmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
