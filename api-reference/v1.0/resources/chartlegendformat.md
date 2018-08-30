# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="784d9-101">ChartLegendFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="784d9-101">ChartLegendFormat resource type</span></span>

<span data-ttu-id="784d9-102">グラフの凡例の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="784d9-102">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="784d9-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="784d9-103">Methods</span></span>
<span data-ttu-id="784d9-104">なし</span><span class="sxs-lookup"><span data-stu-id="784d9-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="784d9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="784d9-105">Properties</span></span>
<span data-ttu-id="784d9-106">なし</span><span class="sxs-lookup"><span data-stu-id="784d9-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="784d9-107">関係</span><span class="sxs-lookup"><span data-stu-id="784d9-107">Relationships</span></span>
| <span data-ttu-id="784d9-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="784d9-108">Relationship</span></span> | <span data-ttu-id="784d9-109">型</span><span class="sxs-lookup"><span data-stu-id="784d9-109">Type</span></span>   |<span data-ttu-id="784d9-110">説明</span><span class="sxs-lookup"><span data-stu-id="784d9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="784d9-111">塗りつぶし</span><span class="sxs-lookup"><span data-stu-id="784d9-111">fill</span></span>|[<span data-ttu-id="784d9-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="784d9-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="784d9-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="784d9-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="784d9-115">フォント</span><span class="sxs-lookup"><span data-stu-id="784d9-115">font</span></span>|[<span data-ttu-id="784d9-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="784d9-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="784d9-p102">グラフの凡例のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="784d9-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="784d9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="784d9-119">JSON representation</span></span>

<span data-ttu-id="784d9-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="784d9-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->