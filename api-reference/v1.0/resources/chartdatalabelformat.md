# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="99986-101">ChartDataLabelFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99986-101">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="99986-102">グラフのデータ ラベルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="99986-102">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="99986-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="99986-103">Methods</span></span>
<span data-ttu-id="99986-104">なし</span><span class="sxs-lookup"><span data-stu-id="99986-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="99986-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99986-105">Properties</span></span>
<span data-ttu-id="99986-106">なし</span><span class="sxs-lookup"><span data-stu-id="99986-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="99986-107">関係</span><span class="sxs-lookup"><span data-stu-id="99986-107">Relationships</span></span>
| <span data-ttu-id="99986-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="99986-108">Relationship</span></span> | <span data-ttu-id="99986-109">型</span><span class="sxs-lookup"><span data-stu-id="99986-109">Type</span></span>   |<span data-ttu-id="99986-110">説明</span><span class="sxs-lookup"><span data-stu-id="99986-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99986-111">塗りつぶし</span><span class="sxs-lookup"><span data-stu-id="99986-111">fill</span></span>|[<span data-ttu-id="99986-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="99986-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="99986-p101">現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="99986-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="99986-115">フォント</span><span class="sxs-lookup"><span data-stu-id="99986-115">font</span></span>|[<span data-ttu-id="99986-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="99986-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="99986-p102">グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="99986-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="99986-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99986-119">JSON representation</span></span>

<span data-ttu-id="99986-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="99986-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->