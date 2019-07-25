---
title: 'workbookRange: rowsAbove'
description: 指定した範囲の上にある特定の行数を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c9a12f8054e71ad7fdf1c6d7392669f0a539bfca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884984"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="357b5-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="357b5-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="357b5-104">指定した範囲の上にある特定の行数を取得します。</span><span class="sxs-lookup"><span data-stu-id="357b5-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="357b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="357b5-105">Permissions</span></span>
<span data-ttu-id="357b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="357b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="357b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="357b5-108">Permission type</span></span>      | <span data-ttu-id="357b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="357b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="357b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="357b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="357b5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="357b5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="357b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="357b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="357b5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="357b5-113">Not supported.</span></span>    |
|<span data-ttu-id="357b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="357b5-114">Application</span></span> | <span data-ttu-id="357b5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="357b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="357b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="357b5-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="357b5-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="357b5-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="357b5-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="357b5-118">Function parameters</span></span>

| <span data-ttu-id="357b5-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="357b5-119">Parameter</span></span>    | <span data-ttu-id="357b5-120">型</span><span class="sxs-lookup"><span data-stu-id="357b5-120">Type</span></span>   |<span data-ttu-id="357b5-121">説明</span><span class="sxs-lookup"><span data-stu-id="357b5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="357b5-122">count</span><span class="sxs-lookup"><span data-stu-id="357b5-122">count</span></span>|<span data-ttu-id="357b5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="357b5-123">Int32</span></span>|<span data-ttu-id="357b5-p102">省略可能。結果の範囲に含める行の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="357b5-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="357b5-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="357b5-129">Request headers</span></span>
| <span data-ttu-id="357b5-130">名前</span><span class="sxs-lookup"><span data-stu-id="357b5-130">Name</span></span>       | <span data-ttu-id="357b5-131">説明</span><span class="sxs-lookup"><span data-stu-id="357b5-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="357b5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="357b5-132">Authorization</span></span>  | <span data-ttu-id="357b5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="357b5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="357b5-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="357b5-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="357b5-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="357b5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="357b5-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="357b5-138">Request body</span></span>
<span data-ttu-id="357b5-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="357b5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="357b5-140">応答</span><span class="sxs-lookup"><span data-stu-id="357b5-140">Response</span></span>
<span data-ttu-id="357b5-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="357b5-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="357b5-142">例</span><span class="sxs-lookup"><span data-stu-id="357b5-142">Example</span></span>
<span data-ttu-id="357b5-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="357b5-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="357b5-144">要求</span><span class="sxs-lookup"><span data-stu-id="357b5-144">Request</span></span>
<span data-ttu-id="357b5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="357b5-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="357b5-146">C#</span><span class="sxs-lookup"><span data-stu-id="357b5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="357b5-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="357b5-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="357b5-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="357b5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="357b5-149">Java</span><span class="sxs-lookup"><span data-stu-id="357b5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="357b5-150">応答</span><span class="sxs-lookup"><span data-stu-id="357b5-150">Response</span></span>
<span data-ttu-id="357b5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="357b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="357b5-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="357b5-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<span data-ttu-id="357b5-155">省略可能`count`なパラメーターを指定せずに呼び出された場合、この関数は範囲の上の単一行を返します。</span><span class="sxs-lookup"><span data-stu-id="357b5-155">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="357b5-156">要求</span><span class="sxs-lookup"><span data-stu-id="357b5-156">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="357b5-157">C#</span><span class="sxs-lookup"><span data-stu-id="357b5-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="357b5-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="357b5-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="357b5-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="357b5-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="357b5-160">Java</span><span class="sxs-lookup"><span data-stu-id="357b5-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="357b5-161">応答</span><span class="sxs-lookup"><span data-stu-id="357b5-161">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
