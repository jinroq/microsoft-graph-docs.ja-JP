---
title: 'workbookRange: rowsAbove'
description: 指定した範囲の上にある特定の行数を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 614fa4796761bb6a388fd44176bbc885251ad6a7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866339"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="80c82-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="80c82-103">workbookRange: rowsAbove</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80c82-104">指定した範囲の上にある特定の行数を取得します。</span><span class="sxs-lookup"><span data-stu-id="80c82-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="80c82-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80c82-105">Permissions</span></span>
<span data-ttu-id="80c82-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80c82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80c82-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80c82-108">Permission type</span></span>      | <span data-ttu-id="80c82-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80c82-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80c82-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80c82-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80c82-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80c82-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80c82-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80c82-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80c82-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80c82-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80c82-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80c82-114">Application</span></span> | <span data-ttu-id="80c82-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80c82-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80c82-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80c82-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="80c82-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="80c82-117">Function parameters</span></span>

| <span data-ttu-id="80c82-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="80c82-118">Parameter</span></span>    | <span data-ttu-id="80c82-119">型</span><span class="sxs-lookup"><span data-stu-id="80c82-119">Type</span></span>   |<span data-ttu-id="80c82-120">説明</span><span class="sxs-lookup"><span data-stu-id="80c82-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80c82-121">count</span><span class="sxs-lookup"><span data-stu-id="80c82-121">count</span></span>|<span data-ttu-id="80c82-122">Int32</span><span class="sxs-lookup"><span data-stu-id="80c82-122">Int32</span></span>|<span data-ttu-id="80c82-p102">省略可能。結果の範囲に含める行の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="80c82-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="80c82-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80c82-128">Request headers</span></span>
| <span data-ttu-id="80c82-129">名前</span><span class="sxs-lookup"><span data-stu-id="80c82-129">Name</span></span>       | <span data-ttu-id="80c82-130">説明</span><span class="sxs-lookup"><span data-stu-id="80c82-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80c82-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="80c82-131">Authorization</span></span>  | <span data-ttu-id="80c82-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80c82-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80c82-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="80c82-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="80c82-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="80c82-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80c82-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="80c82-137">Request body</span></span>
<span data-ttu-id="80c82-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="80c82-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80c82-139">応答</span><span class="sxs-lookup"><span data-stu-id="80c82-139">Response</span></span>

<span data-ttu-id="80c82-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80c82-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80c82-141">例</span><span class="sxs-lookup"><span data-stu-id="80c82-141">Example</span></span>
<span data-ttu-id="80c82-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="80c82-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80c82-143">要求</span><span class="sxs-lookup"><span data-stu-id="80c82-143">Request</span></span>
<span data-ttu-id="80c82-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80c82-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80c82-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="80c82-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsAbove"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80c82-146">C#</span><span class="sxs-lookup"><span data-stu-id="80c82-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80c82-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="80c82-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80c82-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="80c82-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="80c82-149">Java</span><span class="sxs-lookup"><span data-stu-id="80c82-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80c82-150">応答</span><span class="sxs-lookup"><span data-stu-id="80c82-150">Response</span></span>
<span data-ttu-id="80c82-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80c82-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
