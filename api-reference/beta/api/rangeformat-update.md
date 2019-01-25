---
title: rangeformat オブジェクトを更新する
description: rangeformat オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2bd576fcb30facd220e9abf7a8a1fee8d22f80a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524493"
---
# <a name="update-rangeformat"></a><span data-ttu-id="3db20-103">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="3db20-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3db20-104">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3db20-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3db20-105">Permissions</span></span>
<span data-ttu-id="3db20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3db20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db20-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3db20-108">Permission type</span></span>      | <span data-ttu-id="3db20-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3db20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db20-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3db20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3db20-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db20-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3db20-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3db20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db20-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db20-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3db20-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3db20-114">Application</span></span> | <span data-ttu-id="3db20-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3db20-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3db20-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3db20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="3db20-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3db20-117">Optional request headers</span></span>
| <span data-ttu-id="3db20-118">名前</span><span class="sxs-lookup"><span data-stu-id="3db20-118">Name</span></span>       | <span data-ttu-id="3db20-119">説明</span><span class="sxs-lookup"><span data-stu-id="3db20-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3db20-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3db20-120">Authorization</span></span>  | <span data-ttu-id="3db20-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3db20-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3db20-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3db20-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3db20-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3db20-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3db20-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3db20-126">Request body</span></span>
<span data-ttu-id="3db20-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3db20-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3db20-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3db20-130">Property</span></span>     | <span data-ttu-id="3db20-131">型</span><span class="sxs-lookup"><span data-stu-id="3db20-131">Type</span></span>   |<span data-ttu-id="3db20-132">説明</span><span class="sxs-lookup"><span data-stu-id="3db20-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3db20-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="3db20-133">columnWidth</span></span>|<span data-ttu-id="3db20-134">double</span><span class="sxs-lookup"><span data-stu-id="3db20-134">double</span></span>|<span data-ttu-id="3db20-p105">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="3db20-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="3db20-137">horizontalAlignment</span></span>|<span data-ttu-id="3db20-138">string</span><span class="sxs-lookup"><span data-stu-id="3db20-138">string</span></span>|<span data-ttu-id="3db20-p106">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="3db20-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="3db20-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="3db20-141">rowHeight</span></span>|<span data-ttu-id="3db20-142">double</span><span class="sxs-lookup"><span data-stu-id="3db20-142">double</span></span>|<span data-ttu-id="3db20-p107">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="3db20-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="3db20-145">verticalAlignment</span></span>|<span data-ttu-id="3db20-146">文字列</span><span class="sxs-lookup"><span data-stu-id="3db20-146">string</span></span>|<span data-ttu-id="3db20-p108">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="3db20-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="3db20-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="3db20-149">wrapText</span></span>|<span data-ttu-id="3db20-150">boolean</span><span class="sxs-lookup"><span data-stu-id="3db20-150">boolean</span></span>|<span data-ttu-id="3db20-p109">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="3db20-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="3db20-153">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-153">Response</span></span>

<span data-ttu-id="3db20-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [RangeFormat](../resources/rangeformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3db20-154">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3db20-155">例</span><span class="sxs-lookup"><span data-stu-id="3db20-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="3db20-156">表の 3 つのセルで書式設定、塗りつぶし、フォントのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="3db20-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="3db20-157">次の例は、指定された範囲の[RangeFormat](../resources/rangeformat.md)、[RangeFill](../resources/rangefill.md)、[RangeFont](../resources/rangefont.md) の各プロパティを更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3db20-157">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="3db20-158">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="3db20-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="3db20-160">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-160">Request</span></span>
<span data-ttu-id="3db20-161">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="3db20-162">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-162">Response</span></span>
<span data-ttu-id="3db20-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="3db20-166">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-166">Request</span></span>
<span data-ttu-id="3db20-167">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-167">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="3db20-168">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-168">Response</span></span>
<span data-ttu-id="3db20-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="3db20-172">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-172">Request</span></span>
<span data-ttu-id="3db20-173">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-173">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="3db20-174">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-174">Response</span></span>
<span data-ttu-id="3db20-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="3db20-178">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-178">Request</span></span>
<span data-ttu-id="3db20-179">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="3db20-180">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-180">Response</span></span>
<span data-ttu-id="3db20-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="3db20-184">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-184">Request</span></span>
<span data-ttu-id="3db20-185">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-185">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="3db20-186">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-186">Response</span></span>
<span data-ttu-id="3db20-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="3db20-190">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-190">Request</span></span>
<span data-ttu-id="3db20-191">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-191">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="3db20-192">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-192">Response</span></span>
<span data-ttu-id="3db20-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="3db20-196">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-196">Request</span></span>
<span data-ttu-id="3db20-197">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="3db20-198">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-198">Response</span></span>
<span data-ttu-id="3db20-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="3db20-202">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-202">Request</span></span>
<span data-ttu-id="3db20-203">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="3db20-204">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3db20-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="3db20-205">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-205">Response</span></span>
<span data-ttu-id="3db20-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="3db20-209">要求</span><span class="sxs-lookup"><span data-stu-id="3db20-209">Request</span></span>
<span data-ttu-id="3db20-210">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="3db20-210">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="3db20-211">応答</span><span class="sxs-lookup"><span data-stu-id="3db20-211">Response</span></span>
<span data-ttu-id="3db20-p119">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3db20-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
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
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
