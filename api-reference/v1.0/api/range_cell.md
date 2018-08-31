# <a name="range-cell"></a><span data-ttu-id="ff089-101">範囲:セル</span><span class="sxs-lookup"><span data-stu-id="ff089-101">Range: Cell</span></span>

<span data-ttu-id="ff089-p101">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。</span><span class="sxs-lookup"><span data-stu-id="ff089-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff089-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff089-105">Permissions</span></span>
<span data-ttu-id="ff089-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff089-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff089-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff089-108">Permission type</span></span>      | <span data-ttu-id="ff089-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff089-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff089-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff089-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff089-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff089-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff089-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff089-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff089-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff089-113">Not supported.</span></span>    |
|<span data-ttu-id="ff089-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff089-114">Application</span></span> | <span data-ttu-id="ff089-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff089-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff089-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff089-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="ff089-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff089-117">Request headers</span></span>
| <span data-ttu-id="ff089-118">名前</span><span class="sxs-lookup"><span data-stu-id="ff089-118">Name</span></span>       | <span data-ttu-id="ff089-119">説明</span><span class="sxs-lookup"><span data-stu-id="ff089-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff089-120">承認</span><span class="sxs-lookup"><span data-stu-id="ff089-120">Authorization</span></span>  | <span data-ttu-id="ff089-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff089-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff089-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ff089-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ff089-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ff089-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="ff089-126">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff089-126">Path parameters</span></span>
<span data-ttu-id="ff089-127">パスには、次のパラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="ff089-127">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="ff089-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff089-128">Parameter</span></span>    | <span data-ttu-id="ff089-129">型</span><span class="sxs-lookup"><span data-stu-id="ff089-129">Type</span></span>   |<span data-ttu-id="ff089-130">説明</span><span class="sxs-lookup"><span data-stu-id="ff089-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff089-131">行</span><span class="sxs-lookup"><span data-stu-id="ff089-131">row</span></span>|<span data-ttu-id="ff089-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ff089-132">Int32</span></span>|<span data-ttu-id="ff089-p105">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="ff089-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="ff089-135">列</span><span class="sxs-lookup"><span data-stu-id="ff089-135">column</span></span>|<span data-ttu-id="ff089-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ff089-136">Int32</span></span>|<span data-ttu-id="ff089-p106">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="ff089-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="ff089-139">応答</span><span class="sxs-lookup"><span data-stu-id="ff089-139">Response</span></span>

<span data-ttu-id="ff089-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff089-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff089-141">例</span><span class="sxs-lookup"><span data-stu-id="ff089-141">Example</span></span>
<span data-ttu-id="ff089-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ff089-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff089-143">要求</span><span class="sxs-lookup"><span data-stu-id="ff089-143">Request</span></span>
<span data-ttu-id="ff089-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff089-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```

##### <a name="response"></a><span data-ttu-id="ff089-145">応答</span><span class="sxs-lookup"><span data-stu-id="ff089-145">Response</span></span>
<span data-ttu-id="ff089-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff089-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->