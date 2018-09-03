# <a name="rangeformat-resource-type"></a>RangeFormat リソースの種類

範囲のフォント、塗りつぶし、境界線、配置などのプロパティをカプセル化する、書式設定オブジェクトです。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get RangeFormat](../api/rangeformat_get.md) | [WorkbookRangeFormat](rangeformat.md) |rangeFormat オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create RangeBorder](../api/rangeformat_post_borders.md) |[WorkbookRangeBorder](rangeborder.md)| 罫線コレクションに投稿して、新しい RangeBorder を作成します。|
|[List borders](../api/rangeformat_list_borders.md) |[WorkbookRangeBorder](rangeborder.md) コレクション| RangeBorder オブジェクトのコレクションを取得します。|
|[Update](../api/rangeformat_update.md) | [WorkbookRangeFormat](rangeformat.md) |RangeFormat オブジェクトを更新します。 |
|[Autofitcolumns](../api/rangeformat_autofitcolumns.md)|なし|列の現在のデータに基づいて、現在の範囲の列の幅が最適なものになるように変更します。|
|[Autofitrows](../api/rangeformat_autofitrows.md)|なし|現在の行のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|columnWidth|double|範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。|
|horizontalAlignment|string|指定したオブジェクトの水平方向の配置を表します。 指定できる値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。|
|rowHeight|double|範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。|
|verticalAlignment|string|指定したオブジェクトの垂直方向の配置を表します。 可能な値は、   `Top`、   `Center`、   `Bottom`、  `Justify`、   `Distributed` です。|
|wrapText|boolean|オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|borders|[WorkbookRangeBorder](rangeborder.md) コレクション|選択した範囲全体に適用する罫線オブジェクトのコレクションです。読み取り専用です。|
|fill|[WorkbookRangeFill](rangefill.md)|範囲全体に定義された塗りつぶしオブジェクトを返します。読み取り専用です。|
|font|[WorkbookRangeFont](rangefont.md)|選択した範囲全体に定義されているフォント オブジェクトを返します。読み取り専用です。|
|protection|[WorkbookFormatProtection](formatprotection.md)|範囲に対する書式保護オブジェクトを返します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->