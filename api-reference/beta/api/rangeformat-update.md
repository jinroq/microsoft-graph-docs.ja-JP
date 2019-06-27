---
title: rangeformat オブジェクトを更新する
description: rangeformat オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7be6aee49e177501554c124e3a3bd7c4618392c0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268012"
---
# <a name="update-rangeformat"></a><span data-ttu-id="def1f-103">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="def1f-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def1f-104">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="def1f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="def1f-105">Permissions</span></span>
<span data-ttu-id="def1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="def1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def1f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="def1f-108">Permission type</span></span>      | <span data-ttu-id="def1f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="def1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="def1f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="def1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="def1f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="def1f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="def1f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="def1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def1f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="def1f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="def1f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="def1f-114">Application</span></span> | <span data-ttu-id="def1f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="def1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="def1f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="def1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="def1f-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="def1f-117">Optional request headers</span></span>
| <span data-ttu-id="def1f-118">名前</span><span class="sxs-lookup"><span data-stu-id="def1f-118">Name</span></span>       | <span data-ttu-id="def1f-119">説明</span><span class="sxs-lookup"><span data-stu-id="def1f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="def1f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="def1f-120">Authorization</span></span>  | <span data-ttu-id="def1f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="def1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="def1f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="def1f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="def1f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="def1f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="def1f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="def1f-126">Request body</span></span>
<span data-ttu-id="def1f-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="def1f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="def1f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="def1f-130">Property</span></span>     | <span data-ttu-id="def1f-131">型</span><span class="sxs-lookup"><span data-stu-id="def1f-131">Type</span></span>   |<span data-ttu-id="def1f-132">説明</span><span class="sxs-lookup"><span data-stu-id="def1f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="def1f-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="def1f-133">columnWidth</span></span>|<span data-ttu-id="def1f-134">double</span><span class="sxs-lookup"><span data-stu-id="def1f-134">double</span></span>|<span data-ttu-id="def1f-p105">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="def1f-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="def1f-137">horizontalAlignment</span></span>|<span data-ttu-id="def1f-138">string</span><span class="sxs-lookup"><span data-stu-id="def1f-138">string</span></span>|<span data-ttu-id="def1f-p106">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="def1f-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="def1f-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="def1f-141">rowHeight</span></span>|<span data-ttu-id="def1f-142">double</span><span class="sxs-lookup"><span data-stu-id="def1f-142">double</span></span>|<span data-ttu-id="def1f-p107">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="def1f-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="def1f-145">verticalAlignment</span></span>|<span data-ttu-id="def1f-146">string</span><span class="sxs-lookup"><span data-stu-id="def1f-146">string</span></span>|<span data-ttu-id="def1f-p108">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="def1f-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="def1f-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="def1f-149">wrapText</span></span>|<span data-ttu-id="def1f-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="def1f-150">boolean</span></span>|<span data-ttu-id="def1f-p109">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="def1f-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="def1f-153">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-153">Response</span></span>

<span data-ttu-id="def1f-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookRangeFormat](../resources/workbookrangeformat.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="def1f-154">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="def1f-155">例</span><span class="sxs-lookup"><span data-stu-id="def1f-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="def1f-156">表の 3 つのセルで書式設定、塗りつぶし、フォントのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="def1f-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="def1f-157">次の例は、指定した範囲の[workbookRangeFormat](../resources/workbookrangeformat.md)、 [WorkbookRangeFill](../resources/workbookrangefill.md)、および[workbookRangeFont](../resources/workbookrangefont.md)プロパティのプロパティを更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="def1f-157">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="def1f-158">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="def1f-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="def1f-160">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-160">Request</span></span>
<span data-ttu-id="def1f-161">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-162">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-162">Response</span></span>
<span data-ttu-id="def1f-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-166">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-167">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-169">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-170">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-170">Request</span></span>
<span data-ttu-id="def1f-171">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-171">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-172">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-172">Response</span></span>
<span data-ttu-id="def1f-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-176">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-177">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-179">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-180">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-180">Request</span></span>
<span data-ttu-id="def1f-181">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-181">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-182">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-182">Response</span></span>
<span data-ttu-id="def1f-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-186">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-187">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-189">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="def1f-190">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-190">Request</span></span>
<span data-ttu-id="def1f-191">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-191">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-192">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-192">Response</span></span>
<span data-ttu-id="def1f-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-196">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-196">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-197">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-197">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-198">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-198">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-199">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-199">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-200">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-200">Request</span></span>
<span data-ttu-id="def1f-201">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-201">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-202">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-202">Response</span></span>
<span data-ttu-id="def1f-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-206">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-207">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-209">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-209">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-210">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-210">Request</span></span>
<span data-ttu-id="def1f-211">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-211">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-212">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-212">Response</span></span>
<span data-ttu-id="def1f-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-216">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-216">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-217">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-217">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-218">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-218">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-219">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-219">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-220">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-220">Request</span></span>
<span data-ttu-id="def1f-221">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-221">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-222">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-222">Response</span></span>
<span data-ttu-id="def1f-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-226">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-226">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-227">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-227">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-229">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-229">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-230">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-230">Request</span></span>
<span data-ttu-id="def1f-231">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-231">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="def1f-232">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="def1f-232">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="def1f-233">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-233">Response</span></span>
<span data-ttu-id="def1f-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-237">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-237">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-238">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-238">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-239">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-239">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-240">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-240">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="def1f-241">要求</span><span class="sxs-lookup"><span data-stu-id="def1f-241">Request</span></span>
<span data-ttu-id="def1f-242">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="def1f-242">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="def1f-243">応答</span><span class="sxs-lookup"><span data-stu-id="def1f-243">Response</span></span>
<span data-ttu-id="def1f-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="def1f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="def1f-247">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="def1f-247">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="def1f-248">C#</span><span class="sxs-lookup"><span data-stu-id="def1f-248">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def1f-249">Javascript</span><span class="sxs-lookup"><span data-stu-id="def1f-249">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="def1f-250">目的-C</span><span class="sxs-lookup"><span data-stu-id="def1f-250">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


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
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: update_rangeformat_font_three/underline:\r\n       Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ]
}
-->
