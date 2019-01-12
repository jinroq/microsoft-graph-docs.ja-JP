---
title: rangeformat オブジェクトを更新する
description: rangeformat オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 649a0c88779ab54c8e4cb8ab93238be3ee000a4d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952546"
---
# <a name="update-rangeformat"></a><span data-ttu-id="aa006-103">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="aa006-103">Update rangeformat</span></span>

<span data-ttu-id="aa006-104">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa006-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aa006-105">Permissions</span></span>
<span data-ttu-id="aa006-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa006-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa006-108">Permission type</span></span>      | <span data-ttu-id="aa006-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa006-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa006-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa006-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa006-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa006-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa006-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa006-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa006-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa006-113">Not supported.</span></span>    |
|<span data-ttu-id="aa006-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa006-114">Application</span></span> | <span data-ttu-id="aa006-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa006-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa006-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa006-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="aa006-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa006-117">Request headers</span></span>
| <span data-ttu-id="aa006-118">名前</span><span class="sxs-lookup"><span data-stu-id="aa006-118">Name</span></span>       | <span data-ttu-id="aa006-119">説明</span><span class="sxs-lookup"><span data-stu-id="aa006-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aa006-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa006-120">Authorization</span></span>  | <span data-ttu-id="aa006-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aa006-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa006-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aa006-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa006-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="aa006-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa006-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa006-126">Request body</span></span>
<span data-ttu-id="aa006-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="aa006-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aa006-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa006-130">Property</span></span>     | <span data-ttu-id="aa006-131">種類</span><span class="sxs-lookup"><span data-stu-id="aa006-131">Type</span></span>   |<span data-ttu-id="aa006-132">説明</span><span class="sxs-lookup"><span data-stu-id="aa006-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa006-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="aa006-133">columnWidth</span></span>|<span data-ttu-id="aa006-134">double</span><span class="sxs-lookup"><span data-stu-id="aa006-134">double</span></span>|<span data-ttu-id="aa006-p105">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="aa006-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="aa006-137">horizontalAlignment</span></span>|<span data-ttu-id="aa006-138">文字列</span><span class="sxs-lookup"><span data-stu-id="aa006-138">string</span></span>|<span data-ttu-id="aa006-139">指定したオブジェクトの水平方向の配置を表します。</span><span class="sxs-lookup"><span data-stu-id="aa006-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="aa006-140">可能な値: `General`、 `Left`、 `Center`、 `Right`、 `Fill`、 `Justify`、 `CenterAcrossSelection`、 `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="aa006-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="aa006-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="aa006-141">rowHeight</span></span>|<span data-ttu-id="aa006-142">double</span><span class="sxs-lookup"><span data-stu-id="aa006-142">double</span></span>|<span data-ttu-id="aa006-p107">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="aa006-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="aa006-145">verticalAlignment</span></span>|<span data-ttu-id="aa006-146">文字列</span><span class="sxs-lookup"><span data-stu-id="aa006-146">string</span></span>|<span data-ttu-id="aa006-147">指定したオブジェクトの垂直方向の配置を表します。</span><span class="sxs-lookup"><span data-stu-id="aa006-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="aa006-148">可能な値: `Top`、 `Center`、 `Bottom`、 `Justify`、 `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="aa006-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="aa006-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="aa006-149">wrapText</span></span>|<span data-ttu-id="aa006-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="aa006-150">boolean</span></span>|<span data-ttu-id="aa006-p109">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="aa006-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="aa006-153">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-153">Response</span></span>

<span data-ttu-id="aa006-154">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookRangeFormat](../resources/rangeformat.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa006-155">例</span><span class="sxs-lookup"><span data-stu-id="aa006-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="aa006-156">表の 3 つのセルで書式設定、塗りつぶし、フォントのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="aa006-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="aa006-157">次の例では、指定した範囲の[WorkbookRangeFormat](../resources/rangeformat.md)、 [WorkbookRangeFill](../resources/rangefill.md)、および[WorkbookRangeFont](../resources/rangefont.md)プロパティのプロパティを更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="aa006-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="aa006-158">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="aa006-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="aa006-160">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-160">Request</span></span>
<span data-ttu-id="aa006-161">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-162">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-162">Response</span></span>
<span data-ttu-id="aa006-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-166">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-166">Request</span></span>
<span data-ttu-id="aa006-167">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-167">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-168">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-168">Response</span></span>
<span data-ttu-id="aa006-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-172">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-172">Request</span></span>
<span data-ttu-id="aa006-173">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-173">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-174">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-174">Response</span></span>
<span data-ttu-id="aa006-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="aa006-178">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-178">Request</span></span>
<span data-ttu-id="aa006-179">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-180">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-180">Response</span></span>
<span data-ttu-id="aa006-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-184">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-184">Request</span></span>
<span data-ttu-id="aa006-185">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-185">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-186">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-186">Response</span></span>
<span data-ttu-id="aa006-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-190">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-190">Request</span></span>
<span data-ttu-id="aa006-191">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-191">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-192">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-192">Response</span></span>
<span data-ttu-id="aa006-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-196">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-196">Request</span></span>
<span data-ttu-id="aa006-197">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-198">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-198">Response</span></span>
<span data-ttu-id="aa006-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-202">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-202">Request</span></span>
<span data-ttu-id="aa006-203">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="aa006-204">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="aa006-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="aa006-205">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-205">Response</span></span>
<span data-ttu-id="aa006-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="aa006-209">要求</span><span class="sxs-lookup"><span data-stu-id="aa006-209">Request</span></span>
<span data-ttu-id="aa006-210">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa006-210">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="aa006-211">応答</span><span class="sxs-lookup"><span data-stu-id="aa006-211">Response</span></span>
<span data-ttu-id="aa006-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa006-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->
