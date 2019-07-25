---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c2e80c70a2e152c9f1f853139ffa4cfd0a1a7a1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884349"
---
# <a name="worksheet-range"></a><span data-ttu-id="ed9cb-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="ed9cb-103">Worksheet: Range</span></span>

<span data-ttu-id="ed9cb-104">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed9cb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed9cb-105">Permissions</span></span>
<span data-ttu-id="ed9cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed9cb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed9cb-108">Permission type</span></span>      | <span data-ttu-id="ed9cb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed9cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed9cb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed9cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed9cb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed9cb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ed9cb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed9cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed9cb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-113">Not supported.</span></span>    |
|<span data-ttu-id="ed9cb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed9cb-114">Application</span></span> | <span data-ttu-id="ed9cb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed9cb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed9cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="ed9cb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed9cb-117">Request headers</span></span>
| <span data-ttu-id="ed9cb-118">名前</span><span class="sxs-lookup"><span data-stu-id="ed9cb-118">Name</span></span>       | <span data-ttu-id="ed9cb-119">説明</span><span class="sxs-lookup"><span data-stu-id="ed9cb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed9cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed9cb-120">Authorization</span></span>  | <span data-ttu-id="ed9cb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed9cb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ed9cb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ed9cb-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="ed9cb-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed9cb-126">Function parameters</span></span>

| <span data-ttu-id="ed9cb-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed9cb-127">Parameter</span></span>    | <span data-ttu-id="ed9cb-128">型</span><span class="sxs-lookup"><span data-stu-id="ed9cb-128">Type</span></span>   |<span data-ttu-id="ed9cb-129">説明</span><span class="sxs-lookup"><span data-stu-id="ed9cb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed9cb-130">address</span><span class="sxs-lookup"><span data-stu-id="ed9cb-130">address</span></span>|<span data-ttu-id="ed9cb-131">string</span><span class="sxs-lookup"><span data-stu-id="ed9cb-131">string</span></span>|<span data-ttu-id="ed9cb-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="ed9cb-135">応答</span><span class="sxs-lookup"><span data-stu-id="ed9cb-135">Response</span></span>

<span data-ttu-id="ed9cb-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed9cb-137">例</span><span class="sxs-lookup"><span data-stu-id="ed9cb-137">Example</span></span>
<span data-ttu-id="ed9cb-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed9cb-139">要求</span><span class="sxs-lookup"><span data-stu-id="ed9cb-139">Request</span></span>
<span data-ttu-id="ed9cb-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed9cb-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ed9cb-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed9cb-142">C#</span><span class="sxs-lookup"><span data-stu-id="ed9cb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed9cb-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed9cb-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed9cb-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="ed9cb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ed9cb-145">Java</span><span class="sxs-lookup"><span data-stu-id="ed9cb-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed9cb-146">応答</span><span class="sxs-lookup"><span data-stu-id="ed9cb-146">Response</span></span>
<span data-ttu-id="ed9cb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="ed9cb-150">オプション`address`のパラメーターが指定されていない場合、この関数はワークシートの範囲全体を返します。</span><span class="sxs-lookup"><span data-stu-id="ed9cb-150">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="ed9cb-151">要求</span><span class="sxs-lookup"><span data-stu-id="ed9cb-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ed9cb-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ed9cb-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed9cb-153">C#</span><span class="sxs-lookup"><span data-stu-id="ed9cb-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed9cb-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed9cb-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed9cb-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="ed9cb-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ed9cb-156">Java</span><span class="sxs-lookup"><span data-stu-id="ed9cb-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed9cb-157">応答</span><span class="sxs-lookup"><span data-stu-id="ed9cb-157">Response</span></span>

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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
