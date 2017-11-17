# plannerChecklistItem リソースの種類
<a id="plannerchecklistitem-resource-type" class="xliff"></a>


**PlannerChecklistItem**リソースはタスクのチェックリスト内の項目を表します。タスクのチェックリストは、[checklistItems オブジェクト](plannerchecklistitems.md)で表されます。


## プロパティ
<a id="properties" class="xliff"></a>
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|isChecked|Boolean|項目がチェックされた場合は `true`、それ以外の場合は `false` です。|
|lastModifiedBy|[identitySet](identityset.md)| 読み取り専用です。これを最後に変更したユーザーの ID。|
|lastModifiedDateTime|DateTimeOffset|読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|orderHint|String|チェックリストでの項目の相対順序を設定するのに使用します。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|
|title|String|チェックリスト項目のタイトル|

## JSON 表記
<a id="json-representation" class="xliff"></a>
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->