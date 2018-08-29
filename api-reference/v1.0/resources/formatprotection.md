# <a name="formatprotection-resource-type"></a><span data-ttu-id="2eb2a-101">FormatProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2eb2a-101">FormatProtection resource type</span></span>

<span data-ttu-id="2eb2a-102">範囲オブジェクトの書式保護を表します。</span><span class="sxs-lookup"><span data-stu-id="2eb2a-102">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="2eb2a-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="2eb2a-103">Methods</span></span>

| <span data-ttu-id="2eb2a-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2eb2a-104">Method</span></span>           | <span data-ttu-id="2eb2a-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2eb2a-105">Return Type</span></span>    |<span data-ttu-id="2eb2a-106">説明</span><span class="sxs-lookup"><span data-stu-id="2eb2a-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2eb2a-107">FormatProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="2eb2a-107">Get FormatProtection</span></span>](../api/formatprotection_get.md) | [<span data-ttu-id="2eb2a-108">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="2eb2a-108">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="2eb2a-109">formatProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2eb2a-109">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="2eb2a-110">更新する</span><span class="sxs-lookup"><span data-stu-id="2eb2a-110">Update</span></span>](../api/formatprotection_update.md) | [<span data-ttu-id="2eb2a-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="2eb2a-111">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="2eb2a-112">FormatProtection オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2eb2a-112">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2eb2a-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2eb2a-113">Properties</span></span>
| <span data-ttu-id="2eb2a-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2eb2a-114">Property</span></span>     | <span data-ttu-id="2eb2a-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="2eb2a-115">Type</span></span>   |<span data-ttu-id="2eb2a-116">説明</span><span class="sxs-lookup"><span data-stu-id="2eb2a-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eb2a-117">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="2eb2a-117">formulaHidden</span></span>|<span data-ttu-id="2eb2a-118">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="2eb2a-118">boolean</span></span>|<span data-ttu-id="2eb2a-p101">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="2eb2a-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="2eb2a-121">locked</span><span class="sxs-lookup"><span data-stu-id="2eb2a-121">locked</span></span>|<span data-ttu-id="2eb2a-122">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="2eb2a-122">boolean</span></span>|<span data-ttu-id="2eb2a-p102">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="2eb2a-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2eb2a-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2eb2a-125">Relationships</span></span>
<span data-ttu-id="2eb2a-126">なし</span><span class="sxs-lookup"><span data-stu-id="2eb2a-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2eb2a-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2eb2a-127">JSON representation</span></span>

<span data-ttu-id="2eb2a-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2eb2a-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->