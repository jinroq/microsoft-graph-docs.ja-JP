# <a name="chartpointformat-resource-type"></a><span data-ttu-id="acb6c-101">ChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="acb6c-101">ChartPointFormat resource type</span></span>

<span data-ttu-id="acb6c-102">グラフのポイントの書式設定オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="acb6c-102">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="acb6c-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="acb6c-103">Methods</span></span>
<span data-ttu-id="acb6c-104">なし</span><span class="sxs-lookup"><span data-stu-id="acb6c-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="acb6c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acb6c-105">Properties</span></span>
<span data-ttu-id="acb6c-106">なし</span><span class="sxs-lookup"><span data-stu-id="acb6c-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="acb6c-107">関係</span><span class="sxs-lookup"><span data-stu-id="acb6c-107">Relationships</span></span>
| <span data-ttu-id="acb6c-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="acb6c-108">Relationship</span></span> | <span data-ttu-id="acb6c-109">型</span><span class="sxs-lookup"><span data-stu-id="acb6c-109">Type</span></span>   |<span data-ttu-id="acb6c-110">説明</span><span class="sxs-lookup"><span data-stu-id="acb6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb6c-111">塗りつぶし</span><span class="sxs-lookup"><span data-stu-id="acb6c-111">fill</span></span>|[<span data-ttu-id="acb6c-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="acb6c-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="acb6c-p101">グラフの塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="acb6c-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="acb6c-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="acb6c-115">JSON representation</span></span>

<span data-ttu-id="acb6c-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="acb6c-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->