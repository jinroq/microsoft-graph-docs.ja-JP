---
title: 'workbookRange: columnsAfter'
description: 指定した範囲の右にある特定の列数を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1b32235a01973ca0b357c0a4f31db310cc12073f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886898"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="79a3b-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="79a3b-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="79a3b-104">指定した範囲の右にある特定の列数を取得します。</span><span class="sxs-lookup"><span data-stu-id="79a3b-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="79a3b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79a3b-105">Permissions</span></span>
<span data-ttu-id="79a3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79a3b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79a3b-108">Permission type</span></span>      | <span data-ttu-id="79a3b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79a3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79a3b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79a3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79a3b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79a3b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79a3b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79a3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79a3b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79a3b-113">Not supported.</span></span>    |
|<span data-ttu-id="79a3b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79a3b-114">Application</span></span> | <span data-ttu-id="79a3b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79a3b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79a3b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79a3b-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79a3b-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="79a3b-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="79a3b-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="79a3b-118">Function parameters</span></span>

| <span data-ttu-id="79a3b-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="79a3b-119">Parameter</span></span>    | <span data-ttu-id="79a3b-120">型</span><span class="sxs-lookup"><span data-stu-id="79a3b-120">Type</span></span>   |<span data-ttu-id="79a3b-121">説明</span><span class="sxs-lookup"><span data-stu-id="79a3b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79a3b-122">count</span><span class="sxs-lookup"><span data-stu-id="79a3b-122">count</span></span>|<span data-ttu-id="79a3b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="79a3b-123">Int32</span></span>|<span data-ttu-id="79a3b-124">省略可能。</span><span class="sxs-lookup"><span data-stu-id="79a3b-124">Optional.</span></span> <span data-ttu-id="79a3b-125">結果の範囲に含める列の数です。</span><span class="sxs-lookup"><span data-stu-id="79a3b-125">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="79a3b-126">通常、正の数値を使用して現在の範囲外に範囲を作成します。</span><span class="sxs-lookup"><span data-stu-id="79a3b-126">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="79a3b-127">負の数値を使用して、現在の範囲内に範囲を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="79a3b-127">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="79a3b-128">既定値は 1 です</span><span class="sxs-lookup"><span data-stu-id="79a3b-128">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="79a3b-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79a3b-129">Request headers</span></span>
| <span data-ttu-id="79a3b-130">名前</span><span class="sxs-lookup"><span data-stu-id="79a3b-130">Name</span></span>       | <span data-ttu-id="79a3b-131">説明</span><span class="sxs-lookup"><span data-stu-id="79a3b-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79a3b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="79a3b-132">Authorization</span></span>  | <span data-ttu-id="79a3b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79a3b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79a3b-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="79a3b-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="79a3b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="79a3b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79a3b-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="79a3b-138">Request body</span></span>
<span data-ttu-id="79a3b-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79a3b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79a3b-140">応答</span><span class="sxs-lookup"><span data-stu-id="79a3b-140">Response</span></span>
<span data-ttu-id="79a3b-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79a3b-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79a3b-142">例</span><span class="sxs-lookup"><span data-stu-id="79a3b-142">Example</span></span>
<span data-ttu-id="79a3b-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="79a3b-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79a3b-144">要求</span><span class="sxs-lookup"><span data-stu-id="79a3b-144">Request</span></span>
<span data-ttu-id="79a3b-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79a3b-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79a3b-146">C#</span><span class="sxs-lookup"><span data-stu-id="79a3b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79a3b-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="79a3b-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79a3b-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="79a3b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79a3b-149">Java</span><span class="sxs-lookup"><span data-stu-id="79a3b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79a3b-150">応答</span><span class="sxs-lookup"><span data-stu-id="79a3b-150">Response</span></span>
<span data-ttu-id="79a3b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79a3b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
