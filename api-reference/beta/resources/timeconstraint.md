# <a name="timeconstraint-resource-type"></a>timeConstraint リソースの種類

指定した性質の活動の期間です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|activityDomain|String|活動の性質です (省略可能)。使用可能な値: `unknown`、`work`、`personal`。現在、[findMeetingTimes](../api/user_findmeetingtimes.md) では、この値は常に `work` であると想定し、開催者または出席者の勤務時間中の会議提案のみを返します。|
|timeslots|[timeSlot](timeslot.md) コレクション|期間の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->