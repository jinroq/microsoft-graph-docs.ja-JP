# <a name="chartaxisformat-resource-type"></a>ChartAxisFormat リソースの種類

グラフ軸の書式設定プロパティをカプセル化します。


## <a name="methods"></a>メソッド
なし
## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|フォント|[WorkbookChartFont](chartfont.md)|グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。|
|線|[WorkbookChartLineFormat](chartlineformat.md)|グラフの線の書式設定を表します。値の取得のみ可能です。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->