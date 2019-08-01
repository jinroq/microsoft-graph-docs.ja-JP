---
title: イベント リソースの種類
description: 予定表内のイベントです。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f9a77d6d386632df9f617f46af485220680ea1ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030423"
---
# <a name="event-resource-type"></a>event リソースの種類

[ユーザー](user.md)の予定表か、Office 365 [グループ](group.md)の既定の予定表のイベントです。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)を受信します。
- [デルタ](../api/event-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

> **注:** ユーザーの予定表とグループの予定表、およびそのイベントの操作方法には、わずかな相違点がいくつかあります。

- [calendarGroup](calendargroup.md) にはユーザーの予定表のみを整理できます。
- Outlook はグループの代わりにすべての会議出席依頼を自動的に受け入れます。 _ユーザー_の予定表の会議出席依頼のみを[承諾](../api/event-accept.md)、[仮承諾](../api/event-tentativelyaccept.md)、または[辞退](../api/event-decline.md)できます。
- Outlook はグループ イベントのアラームをサポートしていません。 _ユーザー_の予定表についてのみ、[リマインダー](reminder.md)を[再起動](../api/event-snoozereminder.md)または[無視](../api/event-dismissreminder.md)できます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[イベントを一覧表示する](../api/user-list-events.md)|[event](event.md) コレクション |ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/user-post-events.md) |[event](event.md)| インスタンス コレクションへの投稿により、新しいイベントを作成します。|
|[イベントの取得](../api/event-get.md) | [event](event.md) |event オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/event-update.md) | [event](event.md) |イベント オブジェクトを更新します。 |
|[削除](../api/event-delete.md) | なし |イベント オブジェクトを削除します。 |
|[承諾](../api/event-accept.md)|なし|ユーザーの予定表の指定のイベントを承諾します。|
|[仮承諾する](../api/event-tentativelyaccept.md)|なし|ユーザーの予定表の指定のイベントを仮承諾します。|
|[辞退する](../api/event-decline.md)|なし|ユーザーの予定表の指定のイベントに対する詳細を辞退します。|
|[delta](../api/event-delta.md)|[event](event.md) コレクション|ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。|
|[dismissReminder](../api/event-dismissreminder.md)|なし|ユーザーの予定表の指定したイベントのリマインダーを無視します。|
|[リマインダーを再起動する](../api/event-snoozereminder.md)|なし|ユーザーの予定表の指定したイベントのリマインダーを新しい時刻まで延期します。|
|[インスタンスを一覧表示する](../api/event-list-instances.md) |[event](event.md) コレクション| 指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/event-list-attachments.md) |[attachment](attachment.md) コレクション| イベントのすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/event-post-attachments.md) |[attachment](attachment.md)| 添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つイベントの取得](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | 新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つイベントの取得](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | `$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|attendees|[attendee](attendee.md) コレクション|イベントの出席者のコレクション。|
|body|[itemBody](itembody.md)|イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。|
|bodyPreview|String|イベントに関連付けられたメッセージのプレビュー。テキスト形式です。|
|categories|String collection|イベントに関連付けられたカテゴリ。|
|changeKey|String|イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|createdDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|end|[dateTimeTimeZone](datetimetimezone.md)|イベントが終了する日付、時刻、タイムゾーン 既定で、終了時刻は UTC 単位です。|
|hasAttachments|Boolean|イベントに添付ファイルが含まれている場合、true に設定します。|
|iCalUId|String|複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。 読み取り専用です。|
|id|String| 読み取り専用。|
|重要度|重要度|イベントの重要度。 使用可能な値: `low`、`normal`、`high`。|
|isAllDay|Boolean|イベントが一日中続く場合に、true に設定します。|
|isCancelled|Boolean|イベントがキャンセルされた場合に、true に設定します。|
|isOrganizer|Boolean|メッセージの送信者が開催者でもある場合に、true に設定します。|
|isReminderOn|Boolean|ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|location|[location](location.md)|イベントの場所。|
|locations|[location](location.md) コレクション|イベントを開催する場所、または参加者がいる場所。 **location** プロパティと **locations** プロパティは常に互いに一致します。 **location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。 |
|onlineMeetingUrl|String|オンライン会議の URL。 このプロパティは、開催者が Skype 会議などのオンライン会議としてイベントを指定する場合にのみ設定します。 読み取り専用です。|
|構成内容変更|[recipient](recipient.md)|イベントの開催者。|
|originalEndTimeZone|String|イベントの作成時に設定された終了タイム ゾーン。 値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。|
|originalStart|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。 |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|イベントの繰り返しパターン。|
|reminderMinutesBeforeStart|Int32|アラーム通知を行う、イベント開始時間前の分数。|
|responseRequested|Boolean|イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。|
|responseStatus|[responseStatus](responsestatus.md)|イベント メッセージへの応答で送信される応答のタイプを識別します。|
|sensitivity|sensitivity| 使用可能な値: `normal`、`personal`、`private`、`confidential`。|
|seriesMasterId|String|対象イベントが定期的なアイテムの一部である場合、定期的なアイテムのマスター アイテムの ID。|
|showAs|freeBusyStatus|表示するステータス。 使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|開始|[dateTimeTimeZone](datetimetimezone.md)|イベントが開始する日付、時刻、タイムゾーン。 既定で、開始時刻は UTC 単位です。|
|subject|String|イベントの件名行のテキスト。|
|type|eventType|イベントの種類。 使用可能な値: `singleInstance`、`occurrence`、`exception`、`seriesMaster`。 読み取り専用です。|
|webLink|String|Outlook Web App でイベントを開く URL。<br/><br/>Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br/><br/>この URL には、iFrame 内からアクセスできます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|イベントの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。|
|予定表|[calendar](calendar.md)|イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。|
|extensions|[Extension](extension.md) コレクション|イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|インスタンス|[event](event.md) コレクション|イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.event",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "instances",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "iCalUId": "string",
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
