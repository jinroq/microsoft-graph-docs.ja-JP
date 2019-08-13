---
title: '範囲: クリア'
description: 範囲の値、書式、塗りつぶし、罫線などをクリアします。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 17150c23ea73a83297ebb570b601a0434fb75a03
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309206"
---
# <a name="range-clear"></a><span data-ttu-id="a906e-103">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="a906e-103">Range: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a906e-104">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="a906e-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="a906e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a906e-105">Permissions</span></span>
<span data-ttu-id="a906e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a906e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a906e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a906e-108">Permission type</span></span>      | <span data-ttu-id="a906e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a906e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a906e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a906e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a906e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a906e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a906e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a906e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a906e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a906e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a906e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a906e-114">Application</span></span> | <span data-ttu-id="a906e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a906e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a906e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a906e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="a906e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a906e-117">Request headers</span></span>
| <span data-ttu-id="a906e-118">名前</span><span class="sxs-lookup"><span data-stu-id="a906e-118">Name</span></span>       | <span data-ttu-id="a906e-119">説明</span><span class="sxs-lookup"><span data-stu-id="a906e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a906e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a906e-120">Authorization</span></span>  | <span data-ttu-id="a906e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a906e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a906e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a906e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a906e-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a906e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a906e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a906e-126">Request body</span></span>
<span data-ttu-id="a906e-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a906e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a906e-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a906e-128">Parameter</span></span>    | <span data-ttu-id="a906e-129">型</span><span class="sxs-lookup"><span data-stu-id="a906e-129">Type</span></span>   |<span data-ttu-id="a906e-130">説明</span><span class="sxs-lookup"><span data-stu-id="a906e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a906e-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="a906e-131">applyTo</span></span>|<span data-ttu-id="a906e-132">string</span><span class="sxs-lookup"><span data-stu-id="a906e-132">string</span></span>|<span data-ttu-id="a906e-p104">省略可能。クリア操作の種類を決定します。可能な値は、`All`、`Formats`、`Contents` です。</span><span class="sxs-lookup"><span data-stu-id="a906e-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="a906e-136">応答</span><span class="sxs-lookup"><span data-stu-id="a906e-136">Response</span></span>

<span data-ttu-id="a906e-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a906e-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a906e-139">例</span><span class="sxs-lookup"><span data-stu-id="a906e-139">Example</span></span>
<span data-ttu-id="a906e-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a906e-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a906e-141">要求</span><span class="sxs-lookup"><span data-stu-id="a906e-141">Request</span></span>
<span data-ttu-id="a906e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a906e-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a906e-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a906e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a906e-144">C#</span><span class="sxs-lookup"><span data-stu-id="a906e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a906e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a906e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a906e-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="a906e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a906e-147">Java</span><span class="sxs-lookup"><span data-stu-id="a906e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a906e-148">応答</span><span class="sxs-lookup"><span data-stu-id="a906e-148">Response</span></span>
<span data-ttu-id="a906e-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a906e-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
