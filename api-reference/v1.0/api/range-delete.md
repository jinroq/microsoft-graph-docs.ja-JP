---
title: '範囲: 削除'
description: 範囲に関連付けられているセルを削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1b2e7b338a653b8a3e542a29dd69c9c5673ea29a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607673"
---
# <a name="range-delete"></a><span data-ttu-id="fb1d7-103">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="fb1d7-103">Range: delete</span></span>

<span data-ttu-id="fb1d7-104">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb1d7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb1d7-105">Permissions</span></span>
<span data-ttu-id="fb1d7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb1d7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb1d7-108">Permission type</span></span>      | <span data-ttu-id="fb1d7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb1d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb1d7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb1d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb1d7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb1d7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb1d7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb1d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb1d7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-113">Not supported.</span></span>    |
|<span data-ttu-id="fb1d7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb1d7-114">Application</span></span> | <span data-ttu-id="fb1d7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb1d7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb1d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="fb1d7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb1d7-117">Request headers</span></span>
| <span data-ttu-id="fb1d7-118">名前</span><span class="sxs-lookup"><span data-stu-id="fb1d7-118">Name</span></span>       | <span data-ttu-id="fb1d7-119">説明</span><span class="sxs-lookup"><span data-stu-id="fb1d7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb1d7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb1d7-120">Authorization</span></span>  | <span data-ttu-id="fb1d7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb1d7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb1d7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb1d7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb1d7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb1d7-126">Request body</span></span>
<span data-ttu-id="fb1d7-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fb1d7-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb1d7-128">Parameter</span></span>    | <span data-ttu-id="fb1d7-129">型</span><span class="sxs-lookup"><span data-stu-id="fb1d7-129">Type</span></span>   |<span data-ttu-id="fb1d7-130">説明</span><span class="sxs-lookup"><span data-stu-id="fb1d7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb1d7-131">Shift</span><span class="sxs-lookup"><span data-stu-id="fb1d7-131">shift</span></span>|<span data-ttu-id="fb1d7-132">string</span><span class="sxs-lookup"><span data-stu-id="fb1d7-132">string</span></span>|<span data-ttu-id="fb1d7-133">セルをシフトする方向を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-133">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="fb1d7-134">使用可能な値は`Up`、 `Left`、です。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-134">The possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="fb1d7-135">応答</span><span class="sxs-lookup"><span data-stu-id="fb1d7-135">Response</span></span>

<span data-ttu-id="fb1d7-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb1d7-138">例</span><span class="sxs-lookup"><span data-stu-id="fb1d7-138">Example</span></span>
<span data-ttu-id="fb1d7-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fb1d7-140">要求</span><span class="sxs-lookup"><span data-stu-id="fb1d7-140">Request</span></span>
<span data-ttu-id="fb1d7-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="fb1d7-142">応答</span><span class="sxs-lookup"><span data-stu-id="fb1d7-142">Response</span></span>
<span data-ttu-id="fb1d7-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fb1d7-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fb1d7-144">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="fb1d7-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fb1d7-145">Visual</span><span class="sxs-lookup"><span data-stu-id="fb1d7-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb1d7-146">Java</span><span class="sxs-lookup"><span data-stu-id="fb1d7-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_delete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
