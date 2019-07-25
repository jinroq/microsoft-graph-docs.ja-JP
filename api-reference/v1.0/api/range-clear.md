---
title: '範囲: クリア'
description: 範囲の値、書式、塗りつぶし、罫線などをクリアします。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 910eaedd10f155a9189295158d0f1f2f630af9cd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857238"
---
# <a name="range-clear"></a><span data-ttu-id="7471f-103">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="7471f-103">Range: clear</span></span>

<span data-ttu-id="7471f-104">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="7471f-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="7471f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7471f-105">Permissions</span></span>
<span data-ttu-id="7471f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7471f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7471f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7471f-108">Permission type</span></span>      | <span data-ttu-id="7471f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7471f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7471f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7471f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7471f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7471f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7471f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7471f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7471f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7471f-113">Not supported.</span></span>    |
|<span data-ttu-id="7471f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7471f-114">Application</span></span> | <span data-ttu-id="7471f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7471f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7471f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7471f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="7471f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7471f-117">Request headers</span></span>
| <span data-ttu-id="7471f-118">名前</span><span class="sxs-lookup"><span data-stu-id="7471f-118">Name</span></span>       | <span data-ttu-id="7471f-119">説明</span><span class="sxs-lookup"><span data-stu-id="7471f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7471f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7471f-120">Authorization</span></span>  | <span data-ttu-id="7471f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7471f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7471f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7471f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7471f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7471f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7471f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7471f-126">Request body</span></span>
<span data-ttu-id="7471f-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7471f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7471f-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7471f-128">Parameter</span></span>    | <span data-ttu-id="7471f-129">型</span><span class="sxs-lookup"><span data-stu-id="7471f-129">Type</span></span>   |<span data-ttu-id="7471f-130">説明</span><span class="sxs-lookup"><span data-stu-id="7471f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7471f-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="7471f-131">applyTo</span></span>|<span data-ttu-id="7471f-132">string</span><span class="sxs-lookup"><span data-stu-id="7471f-132">string</span></span>|<span data-ttu-id="7471f-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7471f-133">Optional.</span></span> <span data-ttu-id="7471f-134">クリア操作の種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="7471f-134">Determines the type of clear action.</span></span>  <span data-ttu-id="7471f-135">使用可能な値: `All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="7471f-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="7471f-136">応答</span><span class="sxs-lookup"><span data-stu-id="7471f-136">Response</span></span>

<span data-ttu-id="7471f-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7471f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7471f-139">例</span><span class="sxs-lookup"><span data-stu-id="7471f-139">Example</span></span>
<span data-ttu-id="7471f-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7471f-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7471f-141">要求</span><span class="sxs-lookup"><span data-stu-id="7471f-141">Request</span></span>
<span data-ttu-id="7471f-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7471f-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7471f-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7471f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7471f-144">C#</span><span class="sxs-lookup"><span data-stu-id="7471f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7471f-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="7471f-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7471f-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="7471f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7471f-147">Java</span><span class="sxs-lookup"><span data-stu-id="7471f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7471f-148">応答</span><span class="sxs-lookup"><span data-stu-id="7471f-148">Response</span></span>
<span data-ttu-id="7471f-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7471f-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
