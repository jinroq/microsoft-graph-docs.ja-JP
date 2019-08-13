---
title: RangeSort リソースの種類
description: Range オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 489ad01f0f94eda385f501a39f32cea6996d632b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364776"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="e8183-103">RangeSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8183-103">RangeSort resource type</span></span>

<span data-ttu-id="e8183-104">Range オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="e8183-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="e8183-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8183-105">Methods</span></span>

| <span data-ttu-id="e8183-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8183-106">Method</span></span>           | <span data-ttu-id="e8183-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e8183-107">Return Type</span></span>    |<span data-ttu-id="e8183-108">説明</span><span class="sxs-lookup"><span data-stu-id="e8183-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8183-109">Apply</span><span class="sxs-lookup"><span data-stu-id="e8183-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="e8183-110">None</span><span class="sxs-lookup"><span data-stu-id="e8183-110">None</span></span>|<span data-ttu-id="e8183-111">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="e8183-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8183-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8183-112">Properties</span></span>
<span data-ttu-id="e8183-113">なし</span><span class="sxs-lookup"><span data-stu-id="e8183-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e8183-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8183-114">Relationships</span></span>
<span data-ttu-id="e8183-115">なし</span><span class="sxs-lookup"><span data-stu-id="e8183-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8183-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8183-116">JSON representation</span></span>

<span data-ttu-id="e8183-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8183-117">Here is a JSON representation of the resource.</span></span>


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

##### <a name="request"></a><span data-ttu-id="e8183-118">要求</span><span class="sxs-lookup"><span data-stu-id="e8183-118">Request</span></span>
<span data-ttu-id="e8183-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e8183-119">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e8183-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e8183-120">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8183-121">C#</span><span class="sxs-lookup"><span data-stu-id="e8183-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8183-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8183-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8183-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="e8183-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8183-124">Java</span><span class="sxs-lookup"><span data-stu-id="e8183-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e8183-125">応答</span><span class="sxs-lookup"><span data-stu-id="e8183-125">Response</span></span>
<span data-ttu-id="e8183-126">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e8183-126">Here is an example of the response.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
