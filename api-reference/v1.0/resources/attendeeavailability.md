# <a name="attendeeavailability-resource-type"></a>attendeeAvailability リソースの種類

出席者の種類と空き時間情報。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|出席者|[AttendeeBase](attendeebase.md)|出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。|
|状態|FreeBusyStatus| 出席者の空き時間の状態。 指定できる値は、  `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown` です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
