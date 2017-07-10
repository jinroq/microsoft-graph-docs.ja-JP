<a id="pivottable-resource-type" class="xliff"></a>
# ピボットテーブル リソースの種類

Excel のピボットテーブルを表します。

<a id="methods" class="xliff"></a>
## メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookPivotTable を取得する](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/workbookpivottable_refresh.md)|なし|ピボットテーブルを更新します。 |
|[Refreshall](../api/workbookpivottable_refreshall.md)|なし|指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。|

<a id="properties" class="xliff"></a>
## プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| ピボットテーブルの ID。 読み取り専用です。|
|name|String|ピボットテーブルの名前。    |

<a id="relationships" class="xliff"></a>
## リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[worksheet](worksheet.md)| 現在のピボットテーブルを含んでいるワークシート。読み取り専用です。   |

<a id="json-representation" class="xliff"></a>
## JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
