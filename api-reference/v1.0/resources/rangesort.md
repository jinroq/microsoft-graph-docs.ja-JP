---
title: RangeSort リソースの種類
description: Range オブジェクトの並べ替え操作を管理します。
author: lumine2008
ms.openlocfilehash: 44aa472b218fa2c5f4f0d0db1af6f9c919283197
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353509"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="263b5-103">RangeSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="263b5-103">RangeSort resource type</span></span>

<span data-ttu-id="263b5-104">Range オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="263b5-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="263b5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="263b5-105">Methods</span></span>

| <span data-ttu-id="263b5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="263b5-106">Method</span></span>           | <span data-ttu-id="263b5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="263b5-107">Return Type</span></span>    |<span data-ttu-id="263b5-108">説明</span><span class="sxs-lookup"><span data-stu-id="263b5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="263b5-109">Apply</span><span class="sxs-lookup"><span data-stu-id="263b5-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="263b5-110">なし</span><span class="sxs-lookup"><span data-stu-id="263b5-110">None</span></span>|<span data-ttu-id="263b5-111">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="263b5-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="263b5-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="263b5-112">Properties</span></span>
<span data-ttu-id="263b5-113">なし</span><span class="sxs-lookup"><span data-stu-id="263b5-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="263b5-114">関係</span><span class="sxs-lookup"><span data-stu-id="263b5-114">Relationships</span></span>
<span data-ttu-id="263b5-115">なし</span><span class="sxs-lookup"><span data-stu-id="263b5-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="263b5-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="263b5-116">JSON representation</span></span>

<span data-ttu-id="263b5-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="263b5-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="263b5-118">要求</span><span class="sxs-lookup"><span data-stu-id="263b5-118">Request</span></span>
<span data-ttu-id="263b5-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="263b5-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="263b5-120">応答</span><span class="sxs-lookup"><span data-stu-id="263b5-120">Response</span></span>
<span data-ttu-id="263b5-121">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="263b5-121">Here is an example of the response.</span></span> 
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