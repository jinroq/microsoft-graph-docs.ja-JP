---
title: 範囲:UsedRange
description: 指定した範囲オブジェクトのうち使用されている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ab53ea29a0437b5258a3be9aa3f92a1833f8f0e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888598"
---
# <a name="range-usedrange"></a><span data-ttu-id="49dcd-103">範囲:UsedRange</span><span class="sxs-lookup"><span data-stu-id="49dcd-103">Range: UsedRange</span></span>

<span data-ttu-id="49dcd-104">指定した範囲オブジェクトのうち使用されている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="49dcd-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49dcd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49dcd-105">Permissions</span></span>
<span data-ttu-id="49dcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49dcd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49dcd-108">Permission type</span></span>      | <span data-ttu-id="49dcd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49dcd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49dcd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49dcd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49dcd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49dcd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49dcd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49dcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49dcd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49dcd-113">Not supported.</span></span>    |
|<span data-ttu-id="49dcd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49dcd-114">Application</span></span> | <span data-ttu-id="49dcd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49dcd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49dcd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49dcd-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49dcd-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="49dcd-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="49dcd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49dcd-118">Request headers</span></span>
| <span data-ttu-id="49dcd-119">名前</span><span class="sxs-lookup"><span data-stu-id="49dcd-119">Name</span></span>       | <span data-ttu-id="49dcd-120">説明</span><span class="sxs-lookup"><span data-stu-id="49dcd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49dcd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49dcd-121">Authorization</span></span>  | <span data-ttu-id="49dcd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="49dcd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49dcd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49dcd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="49dcd-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="49dcd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="49dcd-127">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="49dcd-127">Path parameters</span></span>
| <span data-ttu-id="49dcd-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="49dcd-128">Parameter</span></span>    | <span data-ttu-id="49dcd-129">型</span><span class="sxs-lookup"><span data-stu-id="49dcd-129">Type</span></span>   |<span data-ttu-id="49dcd-130">説明</span><span class="sxs-lookup"><span data-stu-id="49dcd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49dcd-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="49dcd-131">valuesOnly</span></span>|<span data-ttu-id="49dcd-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="49dcd-132">boolean</span></span>|<span data-ttu-id="49dcd-p104">省略可能。値の入っているセルのみを使用セルと見なします。</span><span class="sxs-lookup"><span data-stu-id="49dcd-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="49dcd-135">応答</span><span class="sxs-lookup"><span data-stu-id="49dcd-135">Response</span></span>

<span data-ttu-id="49dcd-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="49dcd-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49dcd-137">例</span><span class="sxs-lookup"><span data-stu-id="49dcd-137">Example</span></span>
<span data-ttu-id="49dcd-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="49dcd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49dcd-139">要求</span><span class="sxs-lookup"><span data-stu-id="49dcd-139">Request</span></span>
<span data-ttu-id="49dcd-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49dcd-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49dcd-141">C#</span><span class="sxs-lookup"><span data-stu-id="49dcd-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49dcd-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="49dcd-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49dcd-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="49dcd-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49dcd-144">Java</span><span class="sxs-lookup"><span data-stu-id="49dcd-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49dcd-145">応答</span><span class="sxs-lookup"><span data-stu-id="49dcd-145">Response</span></span>
<span data-ttu-id="49dcd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49dcd-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="49dcd-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<span data-ttu-id="49dcd-150">省略可能`valuesOnly`なパラメーターを指定する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49dcd-150">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="49dcd-151">要求</span><span class="sxs-lookup"><span data-stu-id="49dcd-151">Request</span></span>
<span data-ttu-id="49dcd-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49dcd-152">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49dcd-153">C#</span><span class="sxs-lookup"><span data-stu-id="49dcd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49dcd-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="49dcd-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49dcd-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="49dcd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49dcd-156">Java</span><span class="sxs-lookup"><span data-stu-id="49dcd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49dcd-157">応答</span><span class="sxs-lookup"><span data-stu-id="49dcd-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
