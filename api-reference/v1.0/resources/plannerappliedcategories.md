# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="76611-101">plannerAppliedCategories リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76611-101">plannerAppliedCategories resource type</span></span>


<span data-ttu-id="76611-p101">**AppliedCategoriesCollection** リソースは、タスクに適用されているカテゴリ (またはラベル) のコレクションを表します。これは [plannerTask](plannertask.md) オブジェクトの一部です。最大 6 つのカテゴリをタスクに適用できます。カテゴリの説明 (`category1`、`category2` など) は、[計画の詳細](plannerplandetails.md)オブジェクトの一部です。これはオープン型です。</span><span class="sxs-lookup"><span data-stu-id="76611-p101">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="76611-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76611-107">Properties</span></span>
<span data-ttu-id="76611-p102">クライアントは、オープン型のプロパティを定義できます。ただし、この場合クライアントは、対応するカテゴリがタスクに適用される際に、`category1`、`category2`、`category3`、`category4`、`category5` および/または `category6` を、`true` ブール値が設定されたプロパティとして指定する必要があります。以下に例を示します。これらが適用されなくなると、プロパティはその値が `false` ブール値に設定され、自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="76611-p102">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="76611-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76611-112">JSON representation</span></span>

<span data-ttu-id="76611-113">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="76611-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="76611-114">例:</span><span class="sxs-lookup"><span data-stu-id="76611-114">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->