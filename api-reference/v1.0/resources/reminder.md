# <a name="reminder-resource-type"></a>アラーム リソースの種類



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|changeKey|String|アラームのバージョンを識別します。アラームを変更するたびに **changeKey** も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|eventEndTime|[DateTimeTimeZone](datetimetimezone.md)|イベントが終了する日付、時刻、タイムゾーン。|
|eventId|String|イベントの一意の ID。読み取り専用です。|
|eventLocation|[Location](location.md)|イベントの場所。|
|eventStartTime|[DateTimeTimeZone](datetimetimezone.md)|イベントが開始する日付、時刻、タイムゾーン。|
|eventSubject|String|イベントの件名行のテキスト。|
|eventWebLink|String|Web 上の Outlook でイベントを開く URL。<br/><br/>Web 上の Outlook のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br/><br/>この URL には、iFrame 内からアクセスできます。|
|reminderFireTime|[DateTimeTimeZone](datetimetimezone.md)|アラームの発生を設定する日付、時刻、タイムゾーン。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->