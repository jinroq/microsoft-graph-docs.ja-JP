# <a name="pivottable-resource-type"></a>ピボットテーブル リソースの種類

Excel のピボットテーブルを表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookPivotTable を取得する](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/workbookpivottable_refresh.md)|なし|ピボットテーブルを更新します。 |
|[Refreshall](../api/workbookpivottable_refreshall.md)|なし|指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列| ピボットテーブルの ID。 読み取り専用です。|
|名前|文字列|ピボットテーブルの名前。    |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[WorkbookWorksheet](worksheet.md)| 現在の PivotTable を含んでいるワークシート。読み取り専用。   |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
