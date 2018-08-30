# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="d9f25-101">ChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9f25-101">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="d9f25-102">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="d9f25-102">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="d9f25-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9f25-103">Methods</span></span>
<span data-ttu-id="d9f25-104">なし</span><span class="sxs-lookup"><span data-stu-id="d9f25-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="d9f25-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9f25-105">Properties</span></span>
<span data-ttu-id="d9f25-106">なし</span><span class="sxs-lookup"><span data-stu-id="d9f25-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d9f25-107">関係</span><span class="sxs-lookup"><span data-stu-id="d9f25-107">Relationships</span></span>
| <span data-ttu-id="d9f25-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d9f25-108">Relationship</span></span> | <span data-ttu-id="d9f25-109">型</span><span class="sxs-lookup"><span data-stu-id="d9f25-109">Type</span></span>   |<span data-ttu-id="d9f25-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9f25-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9f25-111">font</span><span class="sxs-lookup"><span data-stu-id="d9f25-111">font</span></span>|[<span data-ttu-id="d9f25-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d9f25-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d9f25-p101">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d9f25-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9f25-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9f25-115">JSON representation</span></span>

<span data-ttu-id="d9f25-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9f25-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->