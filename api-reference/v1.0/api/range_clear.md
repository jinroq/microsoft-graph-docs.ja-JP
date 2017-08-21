# <a name="range-clear"></a><span data-ttu-id="a6988-101">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="a6988-101">Range: clear</span></span>

<span data-ttu-id="a6988-102">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="a6988-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6988-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6988-103">Prerequisites</span></span>
<span data-ttu-id="a6988-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a6988-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="a6988-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6988-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="a6988-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6988-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="a6988-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6988-107">Request headers</span></span>
| <span data-ttu-id="a6988-108">名前</span><span class="sxs-lookup"><span data-stu-id="a6988-108">Name</span></span>       | <span data-ttu-id="a6988-109">説明</span><span class="sxs-lookup"><span data-stu-id="a6988-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a6988-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6988-110">Authorization</span></span>  | <span data-ttu-id="a6988-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6988-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a6988-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6988-113">Request body</span></span>
<span data-ttu-id="a6988-114">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6988-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6988-115">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6988-115">Parameter</span></span>    | <span data-ttu-id="a6988-116">型</span><span class="sxs-lookup"><span data-stu-id="a6988-116">Type</span></span>   |<span data-ttu-id="a6988-117">説明</span><span class="sxs-lookup"><span data-stu-id="a6988-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6988-118">applyTo</span><span class="sxs-lookup"><span data-stu-id="a6988-118">applyTo</span></span>|<span data-ttu-id="a6988-119">string</span><span class="sxs-lookup"><span data-stu-id="a6988-119">string</span></span>|<span data-ttu-id="a6988-p102">省略可能。クリア操作の種類を決定します。可能な値は、`All`、`Formats`、`Contents` です。</span><span class="sxs-lookup"><span data-stu-id="a6988-p102">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="a6988-123">応答</span><span class="sxs-lookup"><span data-stu-id="a6988-123">Response</span></span>

<span data-ttu-id="a6988-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a6988-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6988-126">例</span><span class="sxs-lookup"><span data-stu-id="a6988-126">Example</span></span>
<span data-ttu-id="a6988-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a6988-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a6988-128">要求</span><span class="sxs-lookup"><span data-stu-id="a6988-128">Request</span></span>
<span data-ttu-id="a6988-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6988-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="a6988-130">応答</span><span class="sxs-lookup"><span data-stu-id="a6988-130">Response</span></span>
<span data-ttu-id="a6988-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a6988-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->