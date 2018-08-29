# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="a50b7-101">ChartSeriesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a50b7-101">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="a50b7-102">グラフ系列の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="a50b7-102">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="a50b7-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="a50b7-103">Methods</span></span>
<span data-ttu-id="a50b7-104">なし</span><span class="sxs-lookup"><span data-stu-id="a50b7-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="a50b7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a50b7-105">Properties</span></span>
<span data-ttu-id="a50b7-106">なし</span><span class="sxs-lookup"><span data-stu-id="a50b7-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a50b7-107">関係</span><span class="sxs-lookup"><span data-stu-id="a50b7-107">Relationships</span></span>
| <span data-ttu-id="a50b7-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a50b7-108">Relationship</span></span> | <span data-ttu-id="a50b7-109">型</span><span class="sxs-lookup"><span data-stu-id="a50b7-109">Type</span></span>   |<span data-ttu-id="a50b7-110">説明</span><span class="sxs-lookup"><span data-stu-id="a50b7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a50b7-111">塗りつぶし</span><span class="sxs-lookup"><span data-stu-id="a50b7-111">fill</span></span>|[<span data-ttu-id="a50b7-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="a50b7-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a50b7-p101">グラフ系列の塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a50b7-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="a50b7-115">ライン</span><span class="sxs-lookup"><span data-stu-id="a50b7-115">line</span></span>|[<span data-ttu-id="a50b7-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a50b7-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="a50b7-p102">線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a50b7-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a50b7-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a50b7-119">JSON representation</span></span>

<span data-ttu-id="a50b7-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a50b7-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->