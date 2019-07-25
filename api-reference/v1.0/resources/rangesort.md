---
title: RangeSort リソースの種類
description: Range オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1fa09d156210d7dbe31b5896be071663cc214c64
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891670"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="e3ddb-103">RangeSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3ddb-103">RangeSort resource type</span></span>

<span data-ttu-id="e3ddb-104">Range オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="e3ddb-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="e3ddb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3ddb-105">Methods</span></span>

| <span data-ttu-id="e3ddb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3ddb-106">Method</span></span>           | <span data-ttu-id="e3ddb-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e3ddb-107">Return Type</span></span>    |<span data-ttu-id="e3ddb-108">説明</span><span class="sxs-lookup"><span data-stu-id="e3ddb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3ddb-109">Apply</span><span class="sxs-lookup"><span data-stu-id="e3ddb-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="e3ddb-110">None</span><span class="sxs-lookup"><span data-stu-id="e3ddb-110">None</span></span>|<span data-ttu-id="e3ddb-111">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="e3ddb-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3ddb-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3ddb-112">Properties</span></span>
<span data-ttu-id="e3ddb-113">なし</span><span class="sxs-lookup"><span data-stu-id="e3ddb-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e3ddb-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3ddb-114">Relationships</span></span>
<span data-ttu-id="e3ddb-115">なし</span><span class="sxs-lookup"><span data-stu-id="e3ddb-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3ddb-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3ddb-116">JSON representation</span></span>

<span data-ttu-id="e3ddb-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3ddb-117">Here is a JSON representation of the resource.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e3ddb-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e3ddb-118">HTTP</span></span>](#tab/http)
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

##### <a name="request"></a><span data-ttu-id="e3ddb-119">要求</span><span class="sxs-lookup"><span data-stu-id="e3ddb-119">Request</span></span>
<span data-ttu-id="e3ddb-120">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3ddb-120">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3ddb-121">C#</span><span class="sxs-lookup"><span data-stu-id="e3ddb-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3ddb-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3ddb-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3ddb-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3ddb-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e3ddb-124">Java</span><span class="sxs-lookup"><span data-stu-id="e3ddb-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3ddb-125">応答</span><span class="sxs-lookup"><span data-stu-id="e3ddb-125">Response</span></span>
<span data-ttu-id="e3ddb-126">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e3ddb-126">Here is an example of the response.</span></span> 
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
