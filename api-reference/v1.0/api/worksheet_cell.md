# <a name="worksheet-cell"></a><span data-ttu-id="18f39-101">ワークシート:セル</span><span class="sxs-lookup"><span data-stu-id="18f39-101">Worksheet: Cell</span></span>

<span data-ttu-id="18f39-p101">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="18f39-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18f39-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="18f39-104">Prerequisites</span></span>
<span data-ttu-id="18f39-105">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="18f39-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="18f39-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18f39-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="18f39-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18f39-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="18f39-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18f39-108">Request headers</span></span>
| <span data-ttu-id="18f39-109">名前</span><span class="sxs-lookup"><span data-stu-id="18f39-109">Name</span></span>       | <span data-ttu-id="18f39-110">説明</span><span class="sxs-lookup"><span data-stu-id="18f39-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18f39-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f39-111">Authorization</span></span>  | <span data-ttu-id="18f39-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18f39-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="18f39-114">応答</span><span class="sxs-lookup"><span data-stu-id="18f39-114">Response</span></span>

<span data-ttu-id="18f39-115">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18f39-115">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f39-116">例</span><span class="sxs-lookup"><span data-stu-id="18f39-116">Example</span></span>
<span data-ttu-id="18f39-117">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="18f39-117">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18f39-118">要求</span><span class="sxs-lookup"><span data-stu-id="18f39-118">Request</span></span>
<span data-ttu-id="18f39-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18f39-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="18f39-120">応答</span><span class="sxs-lookup"><span data-stu-id="18f39-120">Response</span></span>
<span data-ttu-id="18f39-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18f39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
