# <a name="attendee-resource-type"></a>参加者リソースの種類

イベントの参加者です。 これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。

[attendeeBase](attendeebase.md) から派生します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|status|[ResponseStatus](responsestatus.md)|イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。|
|type|String|参加者のタイプは、`required`、`optional`、`resource` です。|
|emailAddress|[emailAddress](emailaddress.md)|参加者の名前と SMTP アドレスが含まれます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->