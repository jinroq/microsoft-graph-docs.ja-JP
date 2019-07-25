---
title: '範囲: 削除'
description: 範囲に関連付けられているセルを削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2c9288e882aa1b2e329a05599356088152722dcd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874962"
---
# <a name="range-delete"></a><span data-ttu-id="2ebb8-103">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="2ebb8-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ebb8-104">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ebb8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2ebb8-105">Permissions</span></span>
<span data-ttu-id="2ebb8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ebb8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ebb8-108">Permission type</span></span>      | <span data-ttu-id="2ebb8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ebb8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ebb8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ebb8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ebb8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ebb8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ebb8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ebb8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ebb8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ebb8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ebb8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ebb8-114">Application</span></span> | <span data-ttu-id="2ebb8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ebb8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ebb8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="2ebb8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ebb8-117">Request headers</span></span>
| <span data-ttu-id="2ebb8-118">名前</span><span class="sxs-lookup"><span data-stu-id="2ebb8-118">Name</span></span>       | <span data-ttu-id="2ebb8-119">説明</span><span class="sxs-lookup"><span data-stu-id="2ebb8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ebb8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ebb8-120">Authorization</span></span>  | <span data-ttu-id="2ebb8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ebb8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ebb8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ebb8-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ebb8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ebb8-126">Request body</span></span>
<span data-ttu-id="2ebb8-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ebb8-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2ebb8-128">Parameter</span></span>    | <span data-ttu-id="2ebb8-129">型</span><span class="sxs-lookup"><span data-stu-id="2ebb8-129">Type</span></span>   |<span data-ttu-id="2ebb8-130">説明</span><span class="sxs-lookup"><span data-stu-id="2ebb8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ebb8-131">Shift</span><span class="sxs-lookup"><span data-stu-id="2ebb8-131">shift</span></span>|<span data-ttu-id="2ebb8-132">string</span><span class="sxs-lookup"><span data-stu-id="2ebb8-132">string</span></span>|<span data-ttu-id="2ebb8-p104">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="2ebb8-135">応答</span><span class="sxs-lookup"><span data-stu-id="2ebb8-135">Response</span></span>

<span data-ttu-id="2ebb8-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ebb8-138">例</span><span class="sxs-lookup"><span data-stu-id="2ebb8-138">Example</span></span>
<span data-ttu-id="2ebb8-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ebb8-140">要求</span><span class="sxs-lookup"><span data-stu-id="2ebb8-140">Request</span></span>
<span data-ttu-id="2ebb8-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ebb8-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2ebb8-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ebb8-143">C#</span><span class="sxs-lookup"><span data-stu-id="2ebb8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ebb8-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ebb8-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ebb8-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="2ebb8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ebb8-146">Java</span><span class="sxs-lookup"><span data-stu-id="2ebb8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ebb8-147">応答</span><span class="sxs-lookup"><span data-stu-id="2ebb8-147">Response</span></span>
<span data-ttu-id="2ebb8-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2ebb8-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

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
  ]
}
-->
