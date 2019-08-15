---
title: rangeformat オブジェクトを更新する
description: rangeformat オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 44c14fb2a50cc936604fb59ecf8f0ef7b1eb5df4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411978"
---
# <a name="update-rangeformat"></a><span data-ttu-id="de6b5-103">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="de6b5-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6b5-104">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de6b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de6b5-105">Permissions</span></span>
<span data-ttu-id="de6b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de6b5-108">Permission type</span></span>      | <span data-ttu-id="de6b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de6b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de6b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de6b5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6b5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de6b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de6b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6b5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6b5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de6b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de6b5-114">Application</span></span> | <span data-ttu-id="de6b5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de6b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de6b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="de6b5-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de6b5-117">Optional request headers</span></span>
| <span data-ttu-id="de6b5-118">名前</span><span class="sxs-lookup"><span data-stu-id="de6b5-118">Name</span></span>       | <span data-ttu-id="de6b5-119">説明</span><span class="sxs-lookup"><span data-stu-id="de6b5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="de6b5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de6b5-120">Authorization</span></span>  | <span data-ttu-id="de6b5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de6b5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="de6b5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="de6b5-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de6b5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="de6b5-126">Request body</span></span>
<span data-ttu-id="de6b5-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de6b5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de6b5-130">Property</span></span>     | <span data-ttu-id="de6b5-131">型</span><span class="sxs-lookup"><span data-stu-id="de6b5-131">Type</span></span>   |<span data-ttu-id="de6b5-132">説明</span><span class="sxs-lookup"><span data-stu-id="de6b5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de6b5-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="de6b5-133">columnWidth</span></span>|<span data-ttu-id="de6b5-134">double</span><span class="sxs-lookup"><span data-stu-id="de6b5-134">double</span></span>|<span data-ttu-id="de6b5-p105">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="de6b5-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="de6b5-137">horizontalAlignment</span></span>|<span data-ttu-id="de6b5-138">string</span><span class="sxs-lookup"><span data-stu-id="de6b5-138">string</span></span>|<span data-ttu-id="de6b5-p106">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="de6b5-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="de6b5-141">rowHeight</span></span>|<span data-ttu-id="de6b5-142">double</span><span class="sxs-lookup"><span data-stu-id="de6b5-142">double</span></span>|<span data-ttu-id="de6b5-p107">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="de6b5-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="de6b5-145">verticalAlignment</span></span>|<span data-ttu-id="de6b5-146">string</span><span class="sxs-lookup"><span data-stu-id="de6b5-146">string</span></span>|<span data-ttu-id="de6b5-p108">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="de6b5-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="de6b5-149">wrapText</span></span>|<span data-ttu-id="de6b5-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="de6b5-150">boolean</span></span>|<span data-ttu-id="de6b5-p109">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="de6b5-153">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-153">Response</span></span>

<span data-ttu-id="de6b5-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookRangeFormat](../resources/workbookrangeformat.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-154">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de6b5-155">例</span><span class="sxs-lookup"><span data-stu-id="de6b5-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="de6b5-156">表の 3 つのセルで書式設定、塗りつぶし、フォントのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="de6b5-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="de6b5-157">次の例は、指定した範囲の[workbookRangeFormat](../resources/workbookrangeformat.md)、 [WorkbookRangeFill](../resources/workbookrangefill.md)、および[workbookRangeFont](../resources/workbookrangefont.md)プロパティのプロパティを更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="de6b5-157">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="de6b5-158">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="de6b5-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="de6b5-160">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-160">Request</span></span>
<span data-ttu-id="de6b5-161">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-163">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-166">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-166">Response</span></span>
<span data-ttu-id="de6b5-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-170">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-170">Request</span></span>
<span data-ttu-id="de6b5-171">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-171">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-172">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-173">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-176">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-176">Response</span></span>
<span data-ttu-id="de6b5-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-180">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-180">Request</span></span>
<span data-ttu-id="de6b5-181">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-181">This request updates the background color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-182">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-183">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-185">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-186">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-186">Response</span></span>
<span data-ttu-id="de6b5-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="de6b5-190">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-190">Request</span></span>
<span data-ttu-id="de6b5-191">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-191">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-192">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-193">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-195">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-196">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-196">Response</span></span>
<span data-ttu-id="de6b5-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-200">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-200">Request</span></span>
<span data-ttu-id="de6b5-201">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-201">This request updates the font style and size of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-202">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-203">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-205">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-206">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-206">Response</span></span>
<span data-ttu-id="de6b5-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-210">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-210">Request</span></span>
<span data-ttu-id="de6b5-211">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-211">This request updates the background color of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-212">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-212">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-213">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-215">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-216">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-216">Response</span></span>
<span data-ttu-id="de6b5-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-220">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-220">Request</span></span>
<span data-ttu-id="de6b5-221">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-221">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-222">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-222">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-223">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-225">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-226">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-226">Response</span></span>
<span data-ttu-id="de6b5-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-230">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-230">Request</span></span>
<span data-ttu-id="de6b5-231">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-231">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="de6b5-232">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="de6b5-232">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-233">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-234">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-236">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-237">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-237">Response</span></span>
<span data-ttu-id="de6b5-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="de6b5-241">要求</span><span class="sxs-lookup"><span data-stu-id="de6b5-241">Request</span></span>
<span data-ttu-id="de6b5-242">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="de6b5-242">This request updates the background color of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="de6b5-243">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de6b5-243">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de6b5-244">C#</span><span class="sxs-lookup"><span data-stu-id="de6b5-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6b5-245">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6b5-245">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de6b5-246">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6b5-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="de6b5-247">応答</span><span class="sxs-lookup"><span data-stu-id="de6b5-247">Response</span></span>
<span data-ttu-id="de6b5-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de6b5-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:\r\n       Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ]
}
-->
