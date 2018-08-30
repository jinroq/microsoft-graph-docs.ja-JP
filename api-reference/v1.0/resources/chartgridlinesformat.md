# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="ad4cb-101">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad4cb-101">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="ad4cb-102">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="ad4cb-102">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="ad4cb-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad4cb-103">Methods</span></span>
<span data-ttu-id="ad4cb-104">なし</span><span class="sxs-lookup"><span data-stu-id="ad4cb-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="ad4cb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad4cb-105">Properties</span></span>
<span data-ttu-id="ad4cb-106">なし</span><span class="sxs-lookup"><span data-stu-id="ad4cb-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ad4cb-107">関係</span><span class="sxs-lookup"><span data-stu-id="ad4cb-107">Relationships</span></span>
| <span data-ttu-id="ad4cb-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad4cb-108">Relationship</span></span> | <span data-ttu-id="ad4cb-109">型</span><span class="sxs-lookup"><span data-stu-id="ad4cb-109">Type</span></span>   |<span data-ttu-id="ad4cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="ad4cb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad4cb-111">line</span><span class="sxs-lookup"><span data-stu-id="ad4cb-111">line</span></span>|[<span data-ttu-id="ad4cb-112">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ad4cb-112">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="ad4cb-p101">グラフの線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ad4cb-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ad4cb-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad4cb-115">JSON representation</span></span>

<span data-ttu-id="ad4cb-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad4cb-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->