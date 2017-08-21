# <a name="worksheet-usedrange"></a><span data-ttu-id="36a7e-101">ワークシート:UsedRange</span><span class="sxs-lookup"><span data-stu-id="36a7e-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="36a7e-p101">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="36a7e-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36a7e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="36a7e-104">Prerequisites</span></span>
<span data-ttu-id="36a7e-105">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="36a7e-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="36a7e-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36a7e-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="36a7e-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36a7e-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="36a7e-108">オプションの要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="36a7e-108">Optional request parameter</span></span>
<span data-ttu-id="36a7e-109">要求の URL では、オプションのクエリ パラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="36a7e-109">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="36a7e-110">パラメーター</span><span class="sxs-lookup"><span data-stu-id="36a7e-110">Parameter</span></span>    | <span data-ttu-id="36a7e-111">型</span><span class="sxs-lookup"><span data-stu-id="36a7e-111">Type</span></span>   |<span data-ttu-id="36a7e-112">説明</span><span class="sxs-lookup"><span data-stu-id="36a7e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36a7e-113">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="36a7e-113">valuesOnly</span></span>|<span data-ttu-id="36a7e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="36a7e-114">Boolean</span></span>|<span data-ttu-id="36a7e-p102">省略可能。値の入っているセルのみを使用セルと見なします (書式設定は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="36a7e-p102">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|


## <a name="request-headers"></a><span data-ttu-id="36a7e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36a7e-117">Request headers</span></span>
| <span data-ttu-id="36a7e-118">名前</span><span class="sxs-lookup"><span data-stu-id="36a7e-118">Name</span></span>       | <span data-ttu-id="36a7e-119">説明</span><span class="sxs-lookup"><span data-stu-id="36a7e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36a7e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="36a7e-120">Authorization</span></span>  | <span data-ttu-id="36a7e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36a7e-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="36a7e-123">応答</span><span class="sxs-lookup"><span data-stu-id="36a7e-123">Response</span></span>

<span data-ttu-id="36a7e-124">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36a7e-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36a7e-125">例</span><span class="sxs-lookup"><span data-stu-id="36a7e-125">Example</span></span>
<span data-ttu-id="36a7e-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="36a7e-126">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36a7e-127">要求</span><span class="sxs-lookup"><span data-stu-id="36a7e-127">Request</span></span>
<span data-ttu-id="36a7e-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36a7e-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
Content-type: application/json

```

##### <a name="response"></a><span data-ttu-id="36a7e-129">応答</span><span class="sxs-lookup"><span data-stu-id="36a7e-129">Response</span></span>
<span data-ttu-id="36a7e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36a7e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
