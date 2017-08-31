# <a name="range-cell"></a><span data-ttu-id="2731b-101">範囲:セル</span><span class="sxs-lookup"><span data-stu-id="2731b-101">Range: Cell</span></span>

<span data-ttu-id="2731b-p101">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。</span><span class="sxs-lookup"><span data-stu-id="2731b-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="2731b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2731b-105">Permissions</span></span>
<span data-ttu-id="2731b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2731b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2731b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2731b-108">Permission type</span></span>      | <span data-ttu-id="2731b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2731b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2731b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2731b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2731b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2731b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2731b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2731b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2731b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2731b-113">Not supported.</span></span>    |
|<span data-ttu-id="2731b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2731b-114">Application</span></span> | <span data-ttu-id="2731b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2731b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2731b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2731b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(<address>)/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="2731b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2731b-117">Request headers</span></span>
| <span data-ttu-id="2731b-118">名前</span><span class="sxs-lookup"><span data-stu-id="2731b-118">Name</span></span>       | <span data-ttu-id="2731b-119">説明</span><span class="sxs-lookup"><span data-stu-id="2731b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2731b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2731b-120">Authorization</span></span>  | <span data-ttu-id="2731b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2731b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2731b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2731b-123">Request body</span></span>
<span data-ttu-id="2731b-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2731b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2731b-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2731b-125">Parameter</span></span>    | <span data-ttu-id="2731b-126">型</span><span class="sxs-lookup"><span data-stu-id="2731b-126">Type</span></span>   |<span data-ttu-id="2731b-127">説明</span><span class="sxs-lookup"><span data-stu-id="2731b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2731b-128">row</span><span class="sxs-lookup"><span data-stu-id="2731b-128">row</span></span>|<span data-ttu-id="2731b-129">number</span><span class="sxs-lookup"><span data-stu-id="2731b-129">number</span></span>|<span data-ttu-id="2731b-p104">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="2731b-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="2731b-132">column</span><span class="sxs-lookup"><span data-stu-id="2731b-132">column</span></span>|<span data-ttu-id="2731b-133">number</span><span class="sxs-lookup"><span data-stu-id="2731b-133">number</span></span>|<span data-ttu-id="2731b-p105">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="2731b-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="2731b-136">応答</span><span class="sxs-lookup"><span data-stu-id="2731b-136">Response</span></span>

<span data-ttu-id="2731b-137">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2731b-137">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2731b-138">例</span><span class="sxs-lookup"><span data-stu-id="2731b-138">Example</span></span>
<span data-ttu-id="2731b-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2731b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2731b-140">要求</span><span class="sxs-lookup"><span data-stu-id="2731b-140">Request</span></span>
<span data-ttu-id="2731b-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2731b-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="2731b-142">応答</span><span class="sxs-lookup"><span data-stu-id="2731b-142">Response</span></span>
<span data-ttu-id="2731b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2731b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->