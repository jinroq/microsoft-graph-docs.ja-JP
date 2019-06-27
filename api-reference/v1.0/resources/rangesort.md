---
title: RangeSort リソースの種類
description: Range オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f917cb2fa7c8ade81fef2d713e368cc43ab40b3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275146"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="181ce-103">RangeSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="181ce-103">RangeSort resource type</span></span>

<span data-ttu-id="181ce-104">Range オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="181ce-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="181ce-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="181ce-105">Methods</span></span>

| <span data-ttu-id="181ce-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="181ce-106">Method</span></span>           | <span data-ttu-id="181ce-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="181ce-107">Return Type</span></span>    |<span data-ttu-id="181ce-108">説明</span><span class="sxs-lookup"><span data-stu-id="181ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="181ce-109">Apply</span><span class="sxs-lookup"><span data-stu-id="181ce-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="181ce-110">None</span><span class="sxs-lookup"><span data-stu-id="181ce-110">None</span></span>|<span data-ttu-id="181ce-111">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="181ce-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="181ce-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="181ce-112">Properties</span></span>
<span data-ttu-id="181ce-113">なし</span><span class="sxs-lookup"><span data-stu-id="181ce-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="181ce-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="181ce-114">Relationships</span></span>
<span data-ttu-id="181ce-115">なし</span><span class="sxs-lookup"><span data-stu-id="181ce-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="181ce-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="181ce-116">JSON representation</span></span>

<span data-ttu-id="181ce-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="181ce-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="181ce-118">要求</span><span class="sxs-lookup"><span data-stu-id="181ce-118">Request</span></span>
<span data-ttu-id="181ce-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="181ce-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="181ce-120">応答</span><span class="sxs-lookup"><span data-stu-id="181ce-120">Response</span></span>
<span data-ttu-id="181ce-121">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="181ce-121">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="181ce-122">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="181ce-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="181ce-123">C#</span><span class="sxs-lookup"><span data-stu-id="181ce-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_sort-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="181ce-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="181ce-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_sort-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="181ce-125">目的-C</span><span class="sxs-lookup"><span data-stu-id="181ce-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_sort-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
