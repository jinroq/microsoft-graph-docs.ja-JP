# <a name="chartfont-resource-type"></a><span data-ttu-id="6cbee-101">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6cbee-101">ChartFont resource type</span></span>

<span data-ttu-id="6cbee-102">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="6cbee-102">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="6cbee-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="6cbee-103">Methods</span></span>

| <span data-ttu-id="6cbee-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="6cbee-104">Method</span></span>           | <span data-ttu-id="6cbee-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6cbee-105">Return Type</span></span>    |<span data-ttu-id="6cbee-106">説明</span><span class="sxs-lookup"><span data-stu-id="6cbee-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cbee-107">ChartFont の取得</span><span class="sxs-lookup"><span data-stu-id="6cbee-107">Get ChartFont</span></span>](../api/chartfont_get.md) | [<span data-ttu-id="6cbee-108">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="6cbee-108">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="6cbee-109">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6cbee-109">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="6cbee-110">更新する</span><span class="sxs-lookup"><span data-stu-id="6cbee-110">Update</span></span>](../api/chartfont_update.md) | [<span data-ttu-id="6cbee-111">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="6cbee-111">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="6cbee-112">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="6cbee-112">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6cbee-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cbee-113">Properties</span></span>
| <span data-ttu-id="6cbee-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cbee-114">Property</span></span>     | <span data-ttu-id="6cbee-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="6cbee-115">Type</span></span>   |<span data-ttu-id="6cbee-116">説明</span><span class="sxs-lookup"><span data-stu-id="6cbee-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cbee-117">太字</span><span class="sxs-lookup"><span data-stu-id="6cbee-117">bold</span></span>|<span data-ttu-id="6cbee-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="6cbee-118">boolean</span></span>|<span data-ttu-id="6cbee-119">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="6cbee-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="6cbee-120">カラー</span><span class="sxs-lookup"><span data-stu-id="6cbee-120">color</span></span>|<span data-ttu-id="6cbee-121">文字列</span><span class="sxs-lookup"><span data-stu-id="6cbee-121">string</span></span>|<span data-ttu-id="6cbee-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="6cbee-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="6cbee-125">イタリック</span><span class="sxs-lookup"><span data-stu-id="6cbee-125">italic</span></span>|<span data-ttu-id="6cbee-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="6cbee-126">boolean</span></span>|<span data-ttu-id="6cbee-127">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="6cbee-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="6cbee-128">名前</span><span class="sxs-lookup"><span data-stu-id="6cbee-128">name</span></span>|<span data-ttu-id="6cbee-129">文字列</span><span class="sxs-lookup"><span data-stu-id="6cbee-129">string</span></span>|<span data-ttu-id="6cbee-130">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="6cbee-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="6cbee-131">サイズ</span><span class="sxs-lookup"><span data-stu-id="6cbee-131">size</span></span>|<span data-ttu-id="6cbee-132">二重線</span><span class="sxs-lookup"><span data-stu-id="6cbee-132">double</span></span>|<span data-ttu-id="6cbee-133">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="6cbee-133">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="6cbee-134">下線</span><span class="sxs-lookup"><span data-stu-id="6cbee-134">underline</span></span>|<span data-ttu-id="6cbee-135">文字列</span><span class="sxs-lookup"><span data-stu-id="6cbee-135">string</span></span>|<span data-ttu-id="6cbee-136">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="6cbee-136">Type of underline applied to the font.</span></span> <span data-ttu-id="6cbee-137">可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="6cbee-137">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cbee-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6cbee-138">Relationships</span></span>
<span data-ttu-id="6cbee-139">なし</span><span class="sxs-lookup"><span data-stu-id="6cbee-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6cbee-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cbee-140">JSON representation</span></span>

<span data-ttu-id="6cbee-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6cbee-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->