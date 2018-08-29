# <a name="rangesort-resource-type"></a><span data-ttu-id="71249-101">RangeSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71249-101">RangeSort resource type</span></span>

<span data-ttu-id="71249-102">Range オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="71249-102">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="71249-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="71249-103">Methods</span></span>

| <span data-ttu-id="71249-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="71249-104">Method</span></span>           | <span data-ttu-id="71249-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="71249-105">Return Type</span></span>    |<span data-ttu-id="71249-106">説明</span><span class="sxs-lookup"><span data-stu-id="71249-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71249-107">適用する</span><span class="sxs-lookup"><span data-stu-id="71249-107">Apply</span></span>](../api/rangesort_apply.md)|<span data-ttu-id="71249-108">なし</span><span class="sxs-lookup"><span data-stu-id="71249-108">None</span></span>|<span data-ttu-id="71249-109">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="71249-109">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="71249-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71249-110">Properties</span></span>
<span data-ttu-id="71249-111">なし</span><span class="sxs-lookup"><span data-stu-id="71249-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="71249-112">関係</span><span class="sxs-lookup"><span data-stu-id="71249-112">Relationships</span></span>
<span data-ttu-id="71249-113">なし</span><span class="sxs-lookup"><span data-stu-id="71249-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71249-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71249-114">JSON representation</span></span>

<span data-ttu-id="71249-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71249-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="71249-116">要求</span><span class="sxs-lookup"><span data-stu-id="71249-116">Request</span></span>
<span data-ttu-id="71249-117">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71249-117">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="71249-118">応答</span><span class="sxs-lookup"><span data-stu-id="71249-118">Response</span></span>
<span data-ttu-id="71249-119">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="71249-119">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->