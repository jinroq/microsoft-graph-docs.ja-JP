# plannerAssignment リソースの種類
<a id="plannerassignment-resource-type" class="xliff"></a>

**PlannerAssignment** リソースは、ユーザーに対するタスクの割り当てを表します。この種類は、オープン型の [plannerAssignments](plannerassignments.md) で使用されます。


## プロパティ
<a id="properties" class="xliff"></a>
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|assignor など、タスクの割り当てを実行したユーザーの ID。|
|assignedDateTime|DateTimeOffset|タスクが割り当てられた時間。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|orderHint|String|タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|

## JSON 表記
<a id="json-representation" class="xliff"></a>
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->