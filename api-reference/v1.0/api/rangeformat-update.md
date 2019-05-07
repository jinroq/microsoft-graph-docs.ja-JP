---
title: rangeformat オブジェクトを更新する
description: rangeformat オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 130acb8b4a3e086867a675e5792ab3ae5a451e85
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608262"
---
# <a name="update-rangeformat"></a><span data-ttu-id="8e24d-103">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="8e24d-103">Update rangeformat</span></span>

<span data-ttu-id="8e24d-104">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e24d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e24d-105">Permissions</span></span>
<span data-ttu-id="8e24d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e24d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e24d-108">Permission type</span></span>      | <span data-ttu-id="8e24d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e24d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e24d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e24d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e24d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e24d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e24d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e24d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e24d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e24d-113">Not supported.</span></span>    |
|<span data-ttu-id="8e24d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e24d-114">Application</span></span> | <span data-ttu-id="8e24d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e24d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e24d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="8e24d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e24d-117">Request headers</span></span>
| <span data-ttu-id="8e24d-118">名前</span><span class="sxs-lookup"><span data-stu-id="8e24d-118">Name</span></span>       | <span data-ttu-id="8e24d-119">説明</span><span class="sxs-lookup"><span data-stu-id="8e24d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8e24d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e24d-120">Authorization</span></span>  | <span data-ttu-id="8e24d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e24d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8e24d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8e24d-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e24d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e24d-126">Request body</span></span>
<span data-ttu-id="8e24d-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e24d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e24d-130">Property</span></span>     | <span data-ttu-id="8e24d-131">型</span><span class="sxs-lookup"><span data-stu-id="8e24d-131">Type</span></span>   |<span data-ttu-id="8e24d-132">説明</span><span class="sxs-lookup"><span data-stu-id="8e24d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e24d-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="8e24d-133">columnWidth</span></span>|<span data-ttu-id="8e24d-134">double</span><span class="sxs-lookup"><span data-stu-id="8e24d-134">double</span></span>|<span data-ttu-id="8e24d-p105">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="8e24d-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="8e24d-137">horizontalAlignment</span></span>|<span data-ttu-id="8e24d-138">string</span><span class="sxs-lookup"><span data-stu-id="8e24d-138">string</span></span>|<span data-ttu-id="8e24d-139">指定したオブジェクトの水平方向の配置を表します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="8e24d-140">使用可能な値は`General`、 `Left`、 `Center` `Right` `Fill` `Justify` `CenterAcrossSelection`、、、、、 `Distributed`、です。</span><span class="sxs-lookup"><span data-stu-id="8e24d-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="8e24d-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="8e24d-141">rowHeight</span></span>|<span data-ttu-id="8e24d-142">double</span><span class="sxs-lookup"><span data-stu-id="8e24d-142">double</span></span>|<span data-ttu-id="8e24d-p107">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="8e24d-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="8e24d-145">verticalAlignment</span></span>|<span data-ttu-id="8e24d-146">string</span><span class="sxs-lookup"><span data-stu-id="8e24d-146">string</span></span>|<span data-ttu-id="8e24d-147">指定したオブジェクトの垂直方向の配置を表します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="8e24d-148">使用可能な値: `Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="8e24d-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="8e24d-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="8e24d-149">wrapText</span></span>|<span data-ttu-id="8e24d-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="8e24d-150">boolean</span></span>|<span data-ttu-id="8e24d-p109">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="8e24d-153">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-153">Response</span></span>

<span data-ttu-id="8e24d-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookRangeFormat](../resources/rangeformat.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e24d-155">例</span><span class="sxs-lookup"><span data-stu-id="8e24d-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="8e24d-156">表の 3 つのセルで書式設定、塗りつぶし、フォントのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="8e24d-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="8e24d-157">次の例は、指定した範囲の[WorkbookRangeFormat](../resources/rangeformat.md)、 [WorkbookRangeFill](../resources/rangefill.md)、および[WorkbookRangeFont](../resources/rangefont.md)プロパティのプロパティを更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8e24d-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="8e24d-158">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="8e24d-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="8e24d-160">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-160">Request</span></span>
<span data-ttu-id="8e24d-161">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-162">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-162">Response</span></span>
<span data-ttu-id="8e24d-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-166">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-167">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-168">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-169">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-169">Request</span></span>
<span data-ttu-id="8e24d-170">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-170">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-171">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-171">Response</span></span>
<span data-ttu-id="8e24d-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-175">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-176">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-177">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-178">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-178">Request</span></span>
<span data-ttu-id="8e24d-179">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-179">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-180">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-180">Response</span></span>
<span data-ttu-id="8e24d-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-184">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-185">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-186">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="8e24d-187">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-187">Request</span></span>
<span data-ttu-id="8e24d-188">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-188">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-189">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-189">Response</span></span>
<span data-ttu-id="8e24d-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-193">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-193">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-194">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-194">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-195">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-195">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-196">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-196">Request</span></span>
<span data-ttu-id="8e24d-197">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-197">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-198">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-198">Response</span></span>
<span data-ttu-id="8e24d-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-202">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-202">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-203">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-203">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-204">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-204">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-205">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-205">Request</span></span>
<span data-ttu-id="8e24d-206">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-206">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-207">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-207">Response</span></span>
<span data-ttu-id="8e24d-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-211">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-211">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-212">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-212">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-213">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-213">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-214">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-214">Request</span></span>
<span data-ttu-id="8e24d-215">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-215">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-216">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-216">Response</span></span>
<span data-ttu-id="8e24d-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-220">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-220">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-221">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-221">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-222">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-222">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-223">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-223">Request</span></span>
<span data-ttu-id="8e24d-224">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-224">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="8e24d-225">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="8e24d-225">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-226">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-226">Response</span></span>
<span data-ttu-id="8e24d-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-230">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-230">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-231">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-231">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-232">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-232">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="8e24d-233">要求</span><span class="sxs-lookup"><span data-stu-id="8e24d-233">Request</span></span>
<span data-ttu-id="8e24d-234">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="8e24d-234">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="8e24d-235">応答</span><span class="sxs-lookup"><span data-stu-id="8e24d-235">Response</span></span>
<span data-ttu-id="8e24d-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e24d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8e24d-239">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8e24d-239">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8e24d-240">Visual</span><span class="sxs-lookup"><span data-stu-id="8e24d-240">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e24d-241">Java</span><span class="sxs-lookup"><span data-stu-id="8e24d-241">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->
