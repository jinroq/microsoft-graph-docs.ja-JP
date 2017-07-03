# <a name="event-resource-type"></a>イベント リソースの種類

予定表内のイベントです。

このリソースは以下をサポートしています。

- [拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。
- [デルタ](../api/event_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[イベントを一覧表示する](../api/user_list_events.md)|[event](event.md) コレクション |ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/user_post_events.md) |[event](event.md)| インスタンス コレクションへの投稿により、新しいイベントを作成します。|
|[イベントの取得](../api/event_get.md) | [event](event.md) |event オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/event_update.md) | [event](event.md) |イベント オブジェクトを更新します。 |
|[削除](../api/event_delete.md) | なし |イベント オブジェクトを削除します。 |
|[承諾](../api/event_accept.md)|なし|指定したイベントを承諾します。|
|[tentativelyAccept](../api/event_tentativelyaccept.md)|なし|指定したイベントを仮承諾します。|
|[辞退](../api/event_decline.md)|なし|指定したイベントへの招待を辞退します。|
|[delta](../api/event_delta.md)|[event](event.md) コレクション|ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。|
|[dismissReminder](../api/event_dismissreminder.md)|なし|指定したイベントのアラームを無視します。|
|[snoozeReminder](../api/event_snoozereminder.md)|なし|指定したイベントのアラームを再通知します。|
|[インスタンスの一覧表示](../api/event_list_instances.md) |[event](event.md) コレクション| 指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/event_list_attachments.md) |[attachment](attachment.md) コレクション| イベントのすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/event_post_attachments.md) |[attachment](attachment.md)| 添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[event](event.md)  |新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つイベントの取得](../api/singlevaluelegacyextendedproperty_get.md)  | [event](event.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [event](event.md) | 新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つイベントの取得](../api/multivaluelegacyextendedproperty_get.md)  | [event](event.md) | `$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。 |



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|attendees|[attendee](attendee.md) コレクション|イベントの出席者のコレクション。|
|body|[itemBody](itembody.md)|イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。|
|bodyPreview|String|イベントに関連付けられたメッセージのプレビュー。テキスト形式です。|
|categories|String collection|イベントに関連付けられたカテゴリ。|
|changeKey|String|イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|createdDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|end|[dateTimeTimeZone](datetimetimezone.md)|イベントが終了する日付、時刻、タイムゾーン|
|hasAttachments|Boolean|イベントに添付ファイルが含まれている場合、true に設定します。|
|iCalUId|String|複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。|
|id|String| 読み取り専用。|
|importance|String|イベントの重要度:低 = 0、標準 = 1、高 = 2。使用可能な値: `Low`、`Normal`、`High`。|
|isAllDay|Boolean|イベントが一日中続く場合に、true に設定します。|
|isCancelled|Boolean|イベントがキャンセルされた場合に、true に設定します。|
|isOrganizer|Boolean|メッセージの送信者が開催者でもある場合に、true に設定します。|
|isReminderOn|Boolean|ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|location|[location](location.md)|イベントの場所。|
|onlineMeetingUrl|String|オンライン会議の URL。|
|organizer|[recipient](recipient.md)|イベントの開催者。|
|originalEndTimeZone|String|イベントが作成されたときに設定された終了タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。|
|originalStart|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。 |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|イベントの繰り返しパターン。|
|reminderMinutesBeforeStart|Int32|アラーム通知を行う、イベント開始時間前の分数。|
|responseRequested|Boolean|イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。|
|responseStatus|[responseStatus](responsestatus.md)|イベント メッセージへの応答で送信される応答のタイプを識別します。|
|sensitivity|String| 使用可能な値: `Normal`、`Personal`、`Private`、`Confidential`。|
|seriesMasterId|String|アイテムに割り当てられたカテゴリ。|
|showAs|String|表示されるステータス:予定なし = 0、仮の予定 = 1、予定あり = 2、休暇 = 3、離席 = 4、不明 = -1。使用可能な値: `Free`、`Tentative`、`Busy`、`Oof`、`WorkingElsewhere`、`Unknown`。|
|start|[dateTimeTimeZone](datetimetimezone.md)|イベントが開始する日付、時刻、タイムゾーン。|
|subject|String|イベントの件名行のテキスト。|
|type|String|イベントの種類:SingleInstance = 0、発生 = 1、例外 = 2、SeriesMaster = 3。使用可能な値: `SingleInstance`、`Occurrence`、`Exception`、`SeriesMaster`。|
|webLink|String|Outlook Web App でイベントを開く URL。<br/><br/>Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br/><br/>この URL には、iFrame 内からアクセスできます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|イベントの [fileAttachment](fileAttachment.md) 添付ファイルと [itemAttachment](itemAttachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。|
|予定表|[calendar](calendar.md)|イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。|
|extensions|[Extension](extension.md) コレクション|イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|インスタンス|[event](event.md) コレクション|イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|


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
  "keyProperty": "id",
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
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
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

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](../../../concepts/delta_query_overview.md)
- [フォルダー内のイベントへの増分の変更を取得する](../../../concepts/delta_query_events.md)
- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
