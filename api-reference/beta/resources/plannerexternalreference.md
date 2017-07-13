# plannerExternalReference リソースの種類
<a id="plannerexternalreference-resource-type" class="xliff"></a>

**plannerExternalReference** リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。[externalReferences オブジェクト](plannerexternalreferences.md)のプロパティ/値の組の値です。



## プロパティ
<a id="properties" class="xliff"></a>
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|alias|String|参照を記述するエイリアス名。|
|lastModifiedBy|[identitySet](identityset.md)|読み取り専用です。これを最後に変更したユーザーの ID。|
|lastModifiedDateTime|DateTimeOffset|読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|previewPriority|String|タスクのプレビューとして参照が表示される、相対的な優先順位を設定するのに使用されます。|
|type|String|参照の種類を記述するのに使用されます。次の種類が含まれます: `PowerPoint`、`Word`、`Excel`、`Other`。|

## JSON 表記
<a id="json-representation" class="xliff"></a>
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->