---
title: イベント リソースの種類
description: 予定表内のイベントです。
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: b1986a6d463e1750fea05144e5a8520c62e5a94a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826762"
---
# <a name="event-resource-type"></a>イベント リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ユーザー](user.md)の予定表、または Office 365 の[グループ](group.md)の既定の予定表のイベントです。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)にサブスクライブします。
- [デルタ](../api/event-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

> **注:** ユーザーの予定表、グループ予定表、およびそのイベントと対話できるように、いくつかの小さな違いがあります。

 - の[calendarGroup](calendargroup.md)のユーザーの予定表のみを整理することができます。
 - Outlook は、グループのためのすべての会議出席依頼を自動的に受け入れます。 _ユーザー_の予定表のみの[承諾](../api/event-accept.md)、[仮承諾](../api/event-tentativelyaccept.md)、または会議出席依頼を[辞退する](../api/event-decline.md)ことをがします。
  - Outlook は、グループのイベントのアラームをサポートしていません。 [再通知](../api/event-snoozereminder.md)や[アラーム](reminder.md)を[消す](../api/event-dismissreminder.md)を_ユーザー_の予定表のみにできます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iud": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",
  
  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|attendees|[出席者](attendee.md)コレクション|イベントの参加者のコレクションです。|
|body|[ItemBody](itembody.md)|イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。|
|bodyPreview|String|イベントに関連付けられたメッセージのプレビュー。テキスト形式です。|
|categories|String コレクション|イベントに関連付けられたカテゴリ。 各カテゴリは、ユーザーに対して定義されている[outlookCategory](outlookcategory.md)の**表示名**のプロパティに対応します。|
|changeKey|String|イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|createdDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|end|[DateTimeTimeZone](datetimetimezone.md)|イベントが終了する日時。|
|hasAttachments|ブール値|イベントに添付ファイルが含まれている場合、true に設定します。|
|id|String| 読み取り専用。|
|importance|String|イベントの重要度。 可能な値は `low`、`normal`、`high` です。|
|isAllDay|ブール値|イベントが一日中続く場合に、true に設定します。|
|isCancelled|ブール値|イベントがキャンセルされた場合に、true に設定します。|
|isOrganizer|ブール値|メッセージの送信者が開催者でもある場合に、true に設定します。|
|isReminderOn|ブール値|ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|location|[Location](location.md)|イベントの場所。|
|locations|[場所](location.md)のコレクション|イベントを開催する場所、または参加者がいる場所。 **location** プロパティと **locations** プロパティは常に互いに一致します。 **location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。 |
|onlineMeetingUrl|String|オンライン会議の URL。 会議の開催者として、Skype などのオンライン会議イベントを指定する場合にのみ、プロパティが設定されています。 読み取り専用です。|
|organizer|[Recipient](recipient.md)|イベントの開催者。|
|originalEndTimeZone|String|イベントの作成時に設定された終了タイム ゾーン。 値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。|
|originalStart|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|イベントの繰り返しパターン。|
|reminderMinutesBeforeStart|Int32|アラーム通知を行う、イベント開始時間前の分数。|
|responseRequested|ブール値|イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。|
|responseStatus|[ResponseStatus](responsestatus.md)|イベント メッセージへの応答で送信される応答のタイプを識別します。|
|sensitivity|String| 使用可能な値: `normal`、`personal`、`private`、`confidential`。|
|seriesMasterId|String|項目の ID、定期的な系列マスター、このイベントが定期的な一連の一部である場合。|
|showAs|String|表示するステータス。 使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|開始|[DateTimeTimeZone](datetimetimezone.md)|イベントの開始時刻です。|
|subject|String|イベントの件名行のテキスト。|
|type|String|イベントの種類。 使用可能な値: `singleInstance`、`occurrence`、`exception`、`seriesMaster`。 読み取り専用です。|
|uid|String|複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。 **注:** このプロパティと同じ目的を機能する、 `iCalUid` v1.0 のエンドポイント上の[イベントのリソース](/graph/api/resources/event?view=graph-rest-1.0)のプロパティが同じ値を持つことは保証されませんが、します。|
|webLink|String|Outlook Web App でイベントを開く URL。<br/><br/>Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br/><br/>この URL には、iFrame 内からアクセスできます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) コレクション|イベントの[FileAttachment](fileattachment.md)、 [ItemAttachment](itemattachment.md)、および[referenceAttachment](referenceattachment.md)の添付ファイルのコレクションです。 ナビゲーション プロパティ。 読み取り専用です。 Null 許容型。|
|calendar|[Calendar](calendar.md)|イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。|
|extensions|[Extension](extension.md) コレクション|イベントに対して定義されている、開いている拡張機能のコレクションです。 Null 許容型。|
|インスタンス|[Event](event.md) collection|イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[イベントを一覧表示する](../api/user-list-events.md)|[Event](event.md) collection |ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/user-post-events.md) |[event](event.md)| インスタンス コレクションへの投稿により、新しいイベントを作成します。|
|[イベントの取得](../api/event-get.md) | [event](event.md) |event オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/event-update.md) | [event](event.md)   |イベント オブジェクトを更新します。 |
|[削除](../api/event-delete.md) | なし |イベント オブジェクトを削除します。 |
|[cancel](../api/event-cancel.md) | なし | 開催者から出席者全員にキャンセルについてのメッセージを送信し、指定された会議をキャンセルします。 |
|[承諾](../api/event-accept.md)|なし|ユーザーの予定表で指定したイベントをそのまま使用します。|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|なし|ユーザーの予定表で指定したイベントを仮承諾します。|
|[辞退](../api/event-decline.md)|なし|ユーザーの予定表で指定したイベントへの招待を辞退します。|
|[forward](../api/event-forward.md)|なし|新しい受信者に会議出席依頼を転送の開催者または出席者が会議のイベントのことができます。|
|[delta](../api/event-delta.md)|[event](event.md) コレクション|ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。|
|[dismissReminder](../api/event-dismissreminder.md)|なし|ユーザーの予定表で指定したイベントの事前通知を無視します。|
|[snoozeReminder](../api/event-snoozereminder.md)|なし|までは新しいユーザーの予定表で指定したイベントのアラームを延期します。|
|[インスタンスの一覧表示](../api/event-list-instances.md) |[Event](event.md) collection| Event オブジェクトのコレクションを取得します。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/event-list-attachments.md) |[Attachment](attachment.md) コレクション| イベントのすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/event-post-attachments.md) |[Attachment](attachment.md)| 添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つイベントの取得](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | 新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つイベントの取得](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | `$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。 |

## <a name="see-also"></a>関連項目

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](/graph/delta-query-overview)
- [フォルダー内のイベントへの増分の変更を取得する](/graph/delta-query-events)
- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
