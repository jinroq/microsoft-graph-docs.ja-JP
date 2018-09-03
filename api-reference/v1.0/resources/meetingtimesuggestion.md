# <a name="meetingtimesuggestion-resource-type"></a>meetingTimeSuggestion リソースの種類

会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailability](attendeeavailability.md) コレクション|この提案された会議の各出席者の空き時間情報の状態を示す配列。|
|confidence|Double|すべての出席者が出席する見込みを表すパーセンテージ。|
|locations|[location](location.md) コレクション|この提案された会議の各会議場所の名前と地理的な場所を指定する配列。|
|meetingTimeSlot|[timeSlot](timeslot.md)|会議の提案されている期間。|
|organizerAvailability|FreeBusyStatus| この提案された会議の会議の開催者の可用性。 可能な値は、`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown` です。|
|suggestionReason|文字列|会議時間を提案する理由。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->