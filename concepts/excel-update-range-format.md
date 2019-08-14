---
title: Microsoft Graph により Excel のある範囲の書式を更新する
description: 次の例は、指定された範囲の RangeFormat、RangeFill、RangeFont の各プロパティを更新する方法を示します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6f124621de40c22fea8ef7b8c728fe0bd322ad70
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372744"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="190cc-103">Microsoft Graph で Excel のある範囲の書式を更新する</span><span class="sxs-lookup"><span data-stu-id="190cc-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="190cc-104">次の例は、指定された範囲の [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0)、[RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0)、[RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) の各プロパティを更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="190cc-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="190cc-105">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="190cc-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="190cc-107">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-107">Request</span></span>
<span data-ttu-id="190cc-108">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-109">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-109">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-110">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-110">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-111">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-111">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-112">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-112">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-113">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-113">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-114">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-114">Response</span></span>
<span data-ttu-id="190cc-p101">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "General",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="190cc-118">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-118">Request</span></span>
<span data-ttu-id="190cc-119">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-119">This request updates the font style, size, and color of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-120">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-121">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-124">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-125">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-125">Response</span></span>
<span data-ttu-id="190cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": true,
    "color": "#4B180E",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="190cc-129">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-129">Request</span></span>
<span data-ttu-id="190cc-130">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-130">This request updates the background color of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-132">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-135">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-136">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-136">Response</span></span>
<span data-ttu-id="190cc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="190cc-140">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-140">Request</span></span>
<span data-ttu-id="190cc-141">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-141">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-143">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-146">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-147">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-147">Response</span></span>
<span data-ttu-id="190cc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Center",
    "rowHeight": 49,
    "verticalAlignment": "Center",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="190cc-151">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-151">Request</span></span>
<span data-ttu-id="190cc-152">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-152">This request updates the font style and size of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-154">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-157">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-158">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-158">Response</span></span>
<span data-ttu-id="190cc-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#000000",
    "italic": true,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="190cc-162">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-162">Request</span></span>
<span data-ttu-id="190cc-163">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-163">This request updates the background color of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-164">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-165">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-168">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-169">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-169">Response</span></span>
<span data-ttu-id="190cc-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="190cc-173">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-173">Request</span></span>
<span data-ttu-id="190cc-174">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-174">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-175">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-176">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-178">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-179">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-180">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-180">Response</span></span>
<span data-ttu-id="190cc-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Right",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="190cc-184">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-184">Request</span></span>
<span data-ttu-id="190cc-185">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-185">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="190cc-186">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="190cc-186">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-187">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-188">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-190">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-191">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-192">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-192">Response</span></span>
<span data-ttu-id="190cc-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#FFFFFF",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "Single"
}
```

##### <a name="request"></a><span data-ttu-id="190cc-196">要求</span><span class="sxs-lookup"><span data-stu-id="190cc-196">Request</span></span>
<span data-ttu-id="190cc-197">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="190cc-197">This request updates the background color of the third cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="190cc-198">プロトコル</span><span class="sxs-lookup"><span data-stu-id="190cc-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190cc-199">C#</span><span class="sxs-lookup"><span data-stu-id="190cc-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190cc-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190cc-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190cc-201">目的-C</span><span class="sxs-lookup"><span data-stu-id="190cc-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="190cc-202">Java</span><span class="sxs-lookup"><span data-stu-id="190cc-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="190cc-203">応答</span><span class="sxs-lookup"><span data-stu-id="190cc-203">Response</span></span>
<span data-ttu-id="190cc-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="190cc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


## <a name="see-also"></a><span data-ttu-id="190cc-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="190cc-207">See also</span></span>
* [<span data-ttu-id="190cc-208">Microsoft Graph で Excel のセッションを管理する</span><span class="sxs-lookup"><span data-stu-id="190cc-208">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="190cc-209">Microsoft Graph を使用して Excel ブックに書き込む</span><span class="sxs-lookup"><span data-stu-id="190cc-209">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="190cc-210">Microsoft Graph で Excel のブック関数を使用する</span><span class="sxs-lookup"><span data-stu-id="190cc-210">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="190cc-211">Microsoft Graph により Excel のグラフ イメージを表示する</span><span class="sxs-lookup"><span data-stu-id="190cc-211">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="190cc-212">Excel REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="190cc-212">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update a range format in Excel with Microsoft Graph",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
