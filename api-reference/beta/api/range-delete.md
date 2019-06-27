---
title: '範囲: 削除'
description: 範囲に関連付けられているセルを削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc9404bd6560973dc3fb256d40320a1df77e801b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267642"
---
# <a name="range-delete"></a><span data-ttu-id="1f055-103">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="1f055-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f055-104">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="1f055-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f055-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f055-105">Permissions</span></span>
<span data-ttu-id="1f055-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f055-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f055-108">Permission type</span></span>      | <span data-ttu-id="1f055-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f055-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f055-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f055-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f055-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f055-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f055-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f055-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f055-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f055-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f055-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f055-114">Application</span></span> | <span data-ttu-id="1f055-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f055-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f055-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f055-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="1f055-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f055-117">Request headers</span></span>
| <span data-ttu-id="1f055-118">名前</span><span class="sxs-lookup"><span data-stu-id="1f055-118">Name</span></span>       | <span data-ttu-id="1f055-119">説明</span><span class="sxs-lookup"><span data-stu-id="1f055-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1f055-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f055-120">Authorization</span></span>  | <span data-ttu-id="1f055-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1f055-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f055-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f055-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f055-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1f055-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f055-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f055-126">Request body</span></span>
<span data-ttu-id="1f055-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1f055-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1f055-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1f055-128">Parameter</span></span>    | <span data-ttu-id="1f055-129">型</span><span class="sxs-lookup"><span data-stu-id="1f055-129">Type</span></span>   |<span data-ttu-id="1f055-130">説明</span><span class="sxs-lookup"><span data-stu-id="1f055-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f055-131">Shift</span><span class="sxs-lookup"><span data-stu-id="1f055-131">shift</span></span>|<span data-ttu-id="1f055-132">string</span><span class="sxs-lookup"><span data-stu-id="1f055-132">string</span></span>|<span data-ttu-id="1f055-p104">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="1f055-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="1f055-135">応答</span><span class="sxs-lookup"><span data-stu-id="1f055-135">Response</span></span>

<span data-ttu-id="1f055-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1f055-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f055-138">例</span><span class="sxs-lookup"><span data-stu-id="1f055-138">Example</span></span>
<span data-ttu-id="1f055-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1f055-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1f055-140">要求</span><span class="sxs-lookup"><span data-stu-id="1f055-140">Request</span></span>
<span data-ttu-id="1f055-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f055-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="1f055-142">応答</span><span class="sxs-lookup"><span data-stu-id="1f055-142">Response</span></span>
<span data-ttu-id="1f055-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1f055-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1f055-144">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1f055-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1f055-145">C#</span><span class="sxs-lookup"><span data-stu-id="1f055-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f055-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f055-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1f055-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="1f055-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
