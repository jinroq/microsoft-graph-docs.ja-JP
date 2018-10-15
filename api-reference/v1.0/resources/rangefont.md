# <a name="rangefont-resource-type"></a><span data-ttu-id="1eb3d-101">RangeFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1eb3d-101">RangeFont resource type</span></span>

<span data-ttu-id="1eb3d-102">このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-102">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="1eb3d-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="1eb3d-103">Methods</span></span>

| <span data-ttu-id="1eb3d-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="1eb3d-104">Method</span></span>           | <span data-ttu-id="1eb3d-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1eb3d-105">Return Type</span></span>    |<span data-ttu-id="1eb3d-106">説明</span><span class="sxs-lookup"><span data-stu-id="1eb3d-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1eb3d-107">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="1eb3d-107">Get RangeFont</span></span>](../api/rangefont_get.md) | [<span data-ttu-id="1eb3d-108">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="1eb3d-108">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="1eb3d-109">rangeFont オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-109">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="1eb3d-110">Update</span><span class="sxs-lookup"><span data-stu-id="1eb3d-110">Update</span></span>](../api/rangefont_update.md) | [<span data-ttu-id="1eb3d-111">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="1eb3d-111">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="1eb3d-112">RangeFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-112">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1eb3d-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1eb3d-113">Properties</span></span>
| <span data-ttu-id="1eb3d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1eb3d-114">Property</span></span>     | <span data-ttu-id="1eb3d-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="1eb3d-115">Type</span></span>   |<span data-ttu-id="1eb3d-116">説明</span><span class="sxs-lookup"><span data-stu-id="1eb3d-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eb3d-117">bold</span><span class="sxs-lookup"><span data-stu-id="1eb3d-117">bold</span></span>|<span data-ttu-id="1eb3d-118">boolean</span><span class="sxs-lookup"><span data-stu-id="1eb3d-118">boolean</span></span>|<span data-ttu-id="1eb3d-119">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="1eb3d-120">color</span><span class="sxs-lookup"><span data-stu-id="1eb3d-120">color</span></span>|<span data-ttu-id="1eb3d-121">string</span><span class="sxs-lookup"><span data-stu-id="1eb3d-121">string</span></span>|<span data-ttu-id="1eb3d-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="1eb3d-125">italic</span><span class="sxs-lookup"><span data-stu-id="1eb3d-125">italic</span></span>|<span data-ttu-id="1eb3d-126">boolean</span><span class="sxs-lookup"><span data-stu-id="1eb3d-126">boolean</span></span>|<span data-ttu-id="1eb3d-127">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="1eb3d-128">name</span><span class="sxs-lookup"><span data-stu-id="1eb3d-128">name</span></span>|<span data-ttu-id="1eb3d-129">string</span><span class="sxs-lookup"><span data-stu-id="1eb3d-129">string</span></span>|<span data-ttu-id="1eb3d-130">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="1eb3d-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="1eb3d-131">size</span><span class="sxs-lookup"><span data-stu-id="1eb3d-131">size</span></span>|<span data-ttu-id="1eb3d-132">double</span><span class="sxs-lookup"><span data-stu-id="1eb3d-132">double</span></span>|<span data-ttu-id="1eb3d-133">フォント サイズ</span><span class="sxs-lookup"><span data-stu-id="1eb3d-133">Font size.</span></span>|
|<span data-ttu-id="1eb3d-134">underline</span><span class="sxs-lookup"><span data-stu-id="1eb3d-134">underline</span></span>|<span data-ttu-id="1eb3d-135">string</span><span class="sxs-lookup"><span data-stu-id="1eb3d-135">string</span></span>|<span data-ttu-id="1eb3d-136">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-136">Type of underline applied to the font.</span></span> <span data-ttu-id="1eb3d-137">可能な値は、`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant` です。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-137">The possible values are `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`, , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eb3d-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1eb3d-138">Relationships</span></span>
<span data-ttu-id="1eb3d-139">なし</span><span class="sxs-lookup"><span data-stu-id="1eb3d-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1eb3d-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1eb3d-140">JSON representation</span></span>

<span data-ttu-id="1eb3d-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1eb3d-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->