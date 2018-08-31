# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails リソースの種類

**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plannerTaskDetails を取得](../api/plannertaskdetails_get.md) | [plannerTaskDetails](plannertaskdetails.md) |**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/plannertaskdetails_update.md) | [plannerTaskDetails](plannertaskdetails.md)    |**plannerTaskDetails** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|タスク上のチェックリスト項目のコレクション。|
|説明|文字列|タスクの説明|
|id|文字列| 読み取り専用。 タスクの詳細の ID です。 28 文字で大文字小文字を区別します。 サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。|
|previewType|文字列|タスクに表示されるプレビューの種類を設定します。 可能な値は、`automatic`、`noPreview`、`checklist`、`description`、`reference` です。 `automatic` に設定されている場合、表示されるプレビューは、タスクを表示するアプリによって選択されます。|
|references|[plannerExternalReferences](plannerexternalreferences.md)|タスク上の参照のコレクションです。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
