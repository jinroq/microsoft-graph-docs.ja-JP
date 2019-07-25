---
title: 'RangeFormat: autofitColumns'
description: 現在の列のデータに基づいて、現在の範囲の列の幅を最適な幅に変更します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ad6ae979aba1c1ccf1f147175192f3a82a8b1a44
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883115"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="4bc2f-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="4bc2f-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="4bc2f-104">現在の列のデータに基づいて、現在の範囲の列の幅を最適な幅に変更します。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bc2f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4bc2f-105">Permissions</span></span>
<span data-ttu-id="4bc2f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc2f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bc2f-108">Permission type</span></span>      | <span data-ttu-id="4bc2f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bc2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bc2f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bc2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bc2f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bc2f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4bc2f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bc2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bc2f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-113">Not supported.</span></span>    |
|<span data-ttu-id="4bc2f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bc2f-114">Application</span></span> | <span data-ttu-id="4bc2f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bc2f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bc2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="4bc2f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bc2f-117">Request headers</span></span>
| <span data-ttu-id="4bc2f-118">名前</span><span class="sxs-lookup"><span data-stu-id="4bc2f-118">Name</span></span>       | <span data-ttu-id="4bc2f-119">説明</span><span class="sxs-lookup"><span data-stu-id="4bc2f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4bc2f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bc2f-120">Authorization</span></span>  | <span data-ttu-id="4bc2f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bc2f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4bc2f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4bc2f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc2f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4bc2f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4bc2f-127">応答</span><span class="sxs-lookup"><span data-stu-id="4bc2f-127">Response</span></span>

<span data-ttu-id="4bc2f-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc2f-130">例</span><span class="sxs-lookup"><span data-stu-id="4bc2f-130">Example</span></span>
<span data-ttu-id="4bc2f-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4bc2f-132">要求</span><span class="sxs-lookup"><span data-stu-id="4bc2f-132">Request</span></span>
<span data-ttu-id="4bc2f-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4bc2f-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4bc2f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4bc2f-135">C#</span><span class="sxs-lookup"><span data-stu-id="4bc2f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4bc2f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="4bc2f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4bc2f-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="4bc2f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4bc2f-138">Java</span><span class="sxs-lookup"><span data-stu-id="4bc2f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangeformat-autofitcolumns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4bc2f-139">応答</span><span class="sxs-lookup"><span data-stu-id="4bc2f-139">Response</span></span>
<span data-ttu-id="4bc2f-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4bc2f-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
