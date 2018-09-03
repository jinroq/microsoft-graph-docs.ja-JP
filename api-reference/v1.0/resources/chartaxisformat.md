# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="353b1-101">ChartAxisFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="353b1-101">ChartAxisFormat resource type</span></span>

<span data-ttu-id="353b1-102">グラフ軸の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="353b1-102">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="353b1-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="353b1-103">Methods</span></span>
<span data-ttu-id="353b1-104">なし</span><span class="sxs-lookup"><span data-stu-id="353b1-104">None</span></span>
## <a name="properties"></a><span data-ttu-id="353b1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="353b1-105">Properties</span></span>
<span data-ttu-id="353b1-106">なし</span><span class="sxs-lookup"><span data-stu-id="353b1-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="353b1-107">関係</span><span class="sxs-lookup"><span data-stu-id="353b1-107">Relationships</span></span>
| <span data-ttu-id="353b1-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="353b1-108">Relationship</span></span> | <span data-ttu-id="353b1-109">型</span><span class="sxs-lookup"><span data-stu-id="353b1-109">Type</span></span>   |<span data-ttu-id="353b1-110">説明</span><span class="sxs-lookup"><span data-stu-id="353b1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="353b1-111">フォント</span><span class="sxs-lookup"><span data-stu-id="353b1-111">font</span></span>|[<span data-ttu-id="353b1-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="353b1-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="353b1-p101">グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="353b1-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="353b1-115">線</span><span class="sxs-lookup"><span data-stu-id="353b1-115">line</span></span>|[<span data-ttu-id="353b1-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="353b1-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="353b1-p102">グラフの線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="353b1-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="353b1-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="353b1-119">JSON representation</span></span>

<span data-ttu-id="353b1-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="353b1-120">Here is a JSON representation of the resource.</span></span>

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