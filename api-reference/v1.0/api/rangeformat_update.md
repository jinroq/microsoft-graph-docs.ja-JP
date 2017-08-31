# <a name="update-rangeformat"></a><span data-ttu-id="58adf-101">rangeformat オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="58adf-101">Update rangeformat</span></span>

<span data-ttu-id="58adf-102">rangeformat オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58adf-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="58adf-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58adf-103">Permissions</span></span>
<span data-ttu-id="58adf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58adf-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58adf-106">Permission type</span></span>      | <span data-ttu-id="58adf-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58adf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58adf-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58adf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="58adf-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58adf-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58adf-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58adf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58adf-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58adf-111">Not supported.</span></span>    |
|<span data-ttu-id="58adf-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58adf-112">Application</span></span> | <span data-ttu-id="58adf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58adf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58adf-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58adf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(<address>)/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="58adf-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58adf-115">Optional request headers</span></span>
| <span data-ttu-id="58adf-116">名前</span><span class="sxs-lookup"><span data-stu-id="58adf-116">Name</span></span>       | <span data-ttu-id="58adf-117">説明</span><span class="sxs-lookup"><span data-stu-id="58adf-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="58adf-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="58adf-118">Authorization</span></span>  | <span data-ttu-id="58adf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58adf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58adf-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="58adf-121">Request body</span></span>
<span data-ttu-id="58adf-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="58adf-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="58adf-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58adf-125">Property</span></span>     | <span data-ttu-id="58adf-126">型</span><span class="sxs-lookup"><span data-stu-id="58adf-126">Type</span></span>   |<span data-ttu-id="58adf-127">説明</span><span class="sxs-lookup"><span data-stu-id="58adf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58adf-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="58adf-128">columnWidth</span></span>|<span data-ttu-id="58adf-129">double</span><span class="sxs-lookup"><span data-stu-id="58adf-129">double</span></span>|<span data-ttu-id="58adf-p104">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="58adf-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="58adf-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="58adf-132">horizontalAlignment</span></span>|<span data-ttu-id="58adf-133">string</span><span class="sxs-lookup"><span data-stu-id="58adf-133">string</span></span>|<span data-ttu-id="58adf-p105">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="58adf-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="58adf-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="58adf-136">rowHeight</span></span>|<span data-ttu-id="58adf-137">double</span><span class="sxs-lookup"><span data-stu-id="58adf-137">double</span></span>|<span data-ttu-id="58adf-p106">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="58adf-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="58adf-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="58adf-140">verticalAlignment</span></span>|<span data-ttu-id="58adf-141">string</span><span class="sxs-lookup"><span data-stu-id="58adf-141">string</span></span>|<span data-ttu-id="58adf-p107">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="58adf-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="58adf-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="58adf-144">wrapText</span></span>|<span data-ttu-id="58adf-145">boolean</span><span class="sxs-lookup"><span data-stu-id="58adf-145">boolean</span></span>|<span data-ttu-id="58adf-p108">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="58adf-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="58adf-148">応答</span><span class="sxs-lookup"><span data-stu-id="58adf-148">Response</span></span>

<span data-ttu-id="58adf-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [RangeFormat](../resources/rangeformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="58adf-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58adf-150">例</span><span class="sxs-lookup"><span data-stu-id="58adf-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58adf-151">要求</span><span class="sxs-lookup"><span data-stu-id="58adf-151">Request</span></span>
<span data-ttu-id="58adf-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58adf-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```
##### <a name="response"></a><span data-ttu-id="58adf-153">応答</span><span class="sxs-lookup"><span data-stu-id="58adf-153">Response</span></span>
<span data-ttu-id="58adf-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58adf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
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