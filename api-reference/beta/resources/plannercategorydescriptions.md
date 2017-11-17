# plannerCategoryDescriptions リソースの種類
<a id="plannercategorydescriptions-resource-type" class="xliff"></a>

**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。 


## プロパティ
<a id="properties" class="xliff"></a>
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|category1|String|Category 1 に関連付けられているラベル|
|category2|String|Category 2 に関連付けられているラベル|
|category3|String|Category 3 に関連付けられているラベル|
|category4|String|Category 4 に関連付けられているラベル|
|category5|String|Category 5 に関連付けられているラベル|
|category6|String|Category 6 に関連付けられているラベル|

## JSON 表記
<a id="json-representation" class="xliff"></a>
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->