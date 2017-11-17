# <a name="filter-resource-type"></a>フィルター リソースの種類

テーブルの列のフィルター処理を管理します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Apply](../api/filter_apply.md)|なし|指定した列に指定されたフィルター条件を適用します。|
|[Clear](../api/filter_clear.md)|なし|指定した列のフィルターをクリアします。|

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|criteria|[FilterCriteria](filtercriteria.md)|指定した列に現在適用されているフィルターです。読み取り専用です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->