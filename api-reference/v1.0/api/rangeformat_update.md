# <a name="update-rangeformat"></a><span data-ttu-id="48b26-101">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="48b26-101">Update rangeformat</span></span>

<span data-ttu-id="48b26-102">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="48b26-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48b26-103">Permissions</span></span>
<span data-ttu-id="48b26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48b26-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48b26-106">Permission type</span></span>      | <span data-ttu-id="48b26-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48b26-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48b26-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48b26-108">Delegated (work or school account)</span></span> | <span data-ttu-id="48b26-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48b26-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="48b26-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48b26-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48b26-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48b26-111">Not supported.</span></span>    |
|<span data-ttu-id="48b26-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48b26-112">Application</span></span> | <span data-ttu-id="48b26-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48b26-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48b26-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48b26-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="48b26-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48b26-115">Request headers</span></span>
| <span data-ttu-id="48b26-116">名前</span><span class="sxs-lookup"><span data-stu-id="48b26-116">Name</span></span>       | <span data-ttu-id="48b26-117">説明</span><span class="sxs-lookup"><span data-stu-id="48b26-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="48b26-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="48b26-118">Authorization</span></span>  | <span data-ttu-id="48b26-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48b26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48b26-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="48b26-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="48b26-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="48b26-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48b26-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="48b26-124">Request body</span></span>
<span data-ttu-id="48b26-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="48b26-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="48b26-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48b26-128">Property</span></span>     | <span data-ttu-id="48b26-129">型</span><span class="sxs-lookup"><span data-stu-id="48b26-129">Type</span></span>   |<span data-ttu-id="48b26-130">説明</span><span class="sxs-lookup"><span data-stu-id="48b26-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48b26-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="48b26-131">columnWidth</span></span>|<span data-ttu-id="48b26-132">double</span><span class="sxs-lookup"><span data-stu-id="48b26-132">double</span></span>|<span data-ttu-id="48b26-p105">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="48b26-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="48b26-135">horizontalAlignment</span></span>|<span data-ttu-id="48b26-136">string</span><span class="sxs-lookup"><span data-stu-id="48b26-136">string</span></span>|<span data-ttu-id="48b26-p106">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="48b26-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="48b26-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="48b26-139">rowHeight</span></span>|<span data-ttu-id="48b26-140">double</span><span class="sxs-lookup"><span data-stu-id="48b26-140">double</span></span>|<span data-ttu-id="48b26-p107">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="48b26-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="48b26-143">verticalAlignment</span></span>|<span data-ttu-id="48b26-144">string</span><span class="sxs-lookup"><span data-stu-id="48b26-144">string</span></span>|<span data-ttu-id="48b26-p108">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="48b26-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="48b26-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="48b26-147">wrapText</span></span>|<span data-ttu-id="48b26-148">boolean</span><span class="sxs-lookup"><span data-stu-id="48b26-148">boolean</span></span>|<span data-ttu-id="48b26-p109">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="48b26-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="48b26-151">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-151">Response</span></span>

<span data-ttu-id="48b26-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [RangeFormat](../resources/rangeformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="48b26-152">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48b26-153">例</span><span class="sxs-lookup"><span data-stu-id="48b26-153">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="48b26-154">表の 3 つのセルで書式設定、塗りつぶし、フォントのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="48b26-154">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="48b26-155">次の例は、指定された範囲の[RangeFormat](../resources/rangeformat.md)、[RangeFill](../resources/rangefill.md)、[RangeFont](../resources/rangefont.md) の各プロパティを更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="48b26-155">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="48b26-156">この一連の要求の結果は、以下の画像の一番上にある 3 つのセルのように書式設定された 3 つのセルを含む表です。</span><span class="sxs-lookup"><span data-stu-id="48b26-156">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![3 つのセルの書式設定、塗りつぶし、フォントのプロパティが更新された Excel のグラフ テーブル。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="48b26-158">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-158">Request</span></span>
<span data-ttu-id="48b26-159">この要求は、最初のセルの垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-159">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-160">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-160">Response</span></span>
<span data-ttu-id="48b26-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-164">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-164">Request</span></span>
<span data-ttu-id="48b26-165">この要求は、最初のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-165">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-166">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-166">Response</span></span>
<span data-ttu-id="48b26-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-170">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-170">Request</span></span>
<span data-ttu-id="48b26-171">この要求は、最初のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-171">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-172">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-172">Response</span></span>
<span data-ttu-id="48b26-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="48b26-176">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-176">Request</span></span>
<span data-ttu-id="48b26-177">この要求は、2 番目のセルの垂直方向の配置、水平方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-177">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-178">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-178">Response</span></span>
<span data-ttu-id="48b26-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-182">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-182">Request</span></span>
<span data-ttu-id="48b26-183">この要求は、2 番目のセルのフォント スタイルとサイズを更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-183">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-184">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-184">Response</span></span>
<span data-ttu-id="48b26-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-188">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-188">Request</span></span>
<span data-ttu-id="48b26-189">この要求は、2 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-189">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-190">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-190">Response</span></span>
<span data-ttu-id="48b26-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-194">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-194">Request</span></span>
<span data-ttu-id="48b26-195">この要求は、3 番目のセルの水平方向の配置、垂直方向の配置、行の高さ、列の高さを更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-195">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-196">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-196">Response</span></span>
<span data-ttu-id="48b26-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-200">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-200">Request</span></span>
<span data-ttu-id="48b26-201">この要求は、3 番目のセルのフォント スタイル、サイズ、色を更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-201">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="48b26-202">underline プロパティは値として **Single** または **Double** を取ることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="48b26-202">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="48b26-203">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-203">Response</span></span>
<span data-ttu-id="48b26-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="48b26-207">要求</span><span class="sxs-lookup"><span data-stu-id="48b26-207">Request</span></span>
<span data-ttu-id="48b26-208">この要求は、3 番目のセルの背景色を更新します。</span><span class="sxs-lookup"><span data-stu-id="48b26-208">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="48b26-209">応答</span><span class="sxs-lookup"><span data-stu-id="48b26-209">Response</span></span>
<span data-ttu-id="48b26-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48b26-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->