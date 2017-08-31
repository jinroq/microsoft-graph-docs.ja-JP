# <a name="worksheet-cell"></a><span data-ttu-id="59545-101">ワークシート:セル</span><span class="sxs-lookup"><span data-stu-id="59545-101">Worksheet: Cell</span></span>

<span data-ttu-id="59545-p101">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="59545-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="59545-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59545-104">Permissions</span></span>
<span data-ttu-id="59545-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59545-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59545-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59545-107">Permission type</span></span>      | <span data-ttu-id="59545-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59545-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59545-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59545-109">Delegated (work or school account)</span></span> | <span data-ttu-id="59545-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59545-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59545-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59545-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59545-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59545-112">Not supported.</span></span>    |
|<span data-ttu-id="59545-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59545-113">Application</span></span> | <span data-ttu-id="59545-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59545-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59545-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59545-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="59545-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59545-116">Request headers</span></span>
| <span data-ttu-id="59545-117">名前</span><span class="sxs-lookup"><span data-stu-id="59545-117">Name</span></span>       | <span data-ttu-id="59545-118">説明</span><span class="sxs-lookup"><span data-stu-id="59545-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59545-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="59545-119">Authorization</span></span>  | <span data-ttu-id="59545-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59545-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="59545-122">応答</span><span class="sxs-lookup"><span data-stu-id="59545-122">Response</span></span>

<span data-ttu-id="59545-123">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="59545-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59545-124">例</span><span class="sxs-lookup"><span data-stu-id="59545-124">Example</span></span>
<span data-ttu-id="59545-125">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="59545-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59545-126">要求</span><span class="sxs-lookup"><span data-stu-id="59545-126">Request</span></span>
<span data-ttu-id="59545-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59545-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="59545-128">応答</span><span class="sxs-lookup"><span data-stu-id="59545-128">Response</span></span>
<span data-ttu-id="59545-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="59545-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
