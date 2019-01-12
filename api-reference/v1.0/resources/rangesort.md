---
title: RangeSort リソースの種類
description: Range オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d1fb0be3feae69ff2cae34f360a0f78d46a6172
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947576"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="8ea30-103">RangeSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ea30-103">RangeSort resource type</span></span>

<span data-ttu-id="8ea30-104">Range オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="8ea30-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="8ea30-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8ea30-105">Methods</span></span>

| <span data-ttu-id="8ea30-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8ea30-106">Method</span></span>           | <span data-ttu-id="8ea30-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8ea30-107">Return Type</span></span>    |<span data-ttu-id="8ea30-108">説明</span><span class="sxs-lookup"><span data-stu-id="8ea30-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ea30-109">Apply</span><span class="sxs-lookup"><span data-stu-id="8ea30-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="8ea30-110">なし</span><span class="sxs-lookup"><span data-stu-id="8ea30-110">None</span></span>|<span data-ttu-id="8ea30-111">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="8ea30-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ea30-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ea30-112">Properties</span></span>
<span data-ttu-id="8ea30-113">なし</span><span class="sxs-lookup"><span data-stu-id="8ea30-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8ea30-114">関係</span><span class="sxs-lookup"><span data-stu-id="8ea30-114">Relationships</span></span>
<span data-ttu-id="8ea30-115">なし</span><span class="sxs-lookup"><span data-stu-id="8ea30-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ea30-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ea30-116">JSON representation</span></span>

<span data-ttu-id="8ea30-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ea30-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="8ea30-118">要求</span><span class="sxs-lookup"><span data-stu-id="8ea30-118">Request</span></span>
<span data-ttu-id="8ea30-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ea30-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="8ea30-120">応答</span><span class="sxs-lookup"><span data-stu-id="8ea30-120">Response</span></span>
<span data-ttu-id="8ea30-121">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8ea30-121">Here is an example of the response.</span></span> 
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
