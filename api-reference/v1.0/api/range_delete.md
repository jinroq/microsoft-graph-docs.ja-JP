# <a name="range-delete"></a><span data-ttu-id="8b11f-101">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="8b11f-101">Range: delete</span></span>

<span data-ttu-id="8b11f-102">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="8b11f-102">Deletes the cells associated with the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b11f-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="8b11f-103">Prerequisites</span></span>
<span data-ttu-id="8b11f-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8b11f-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="8b11f-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b11f-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="8b11f-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b11f-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="8b11f-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b11f-107">Request headers</span></span>
| <span data-ttu-id="8b11f-108">名前</span><span class="sxs-lookup"><span data-stu-id="8b11f-108">Name</span></span>       | <span data-ttu-id="8b11f-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b11f-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b11f-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b11f-110">Authorization</span></span>  | <span data-ttu-id="8b11f-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b11f-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8b11f-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b11f-113">Request body</span></span>
<span data-ttu-id="8b11f-114">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b11f-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b11f-115">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b11f-115">Parameter</span></span>    | <span data-ttu-id="8b11f-116">型</span><span class="sxs-lookup"><span data-stu-id="8b11f-116">Type</span></span>   |<span data-ttu-id="8b11f-117">説明</span><span class="sxs-lookup"><span data-stu-id="8b11f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b11f-118"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="8b11f-118">shift</span></span>|<span data-ttu-id="8b11f-119">string</span><span class="sxs-lookup"><span data-stu-id="8b11f-119">string</span></span>|<span data-ttu-id="8b11f-p102">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="8b11f-p102">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="8b11f-122">応答</span><span class="sxs-lookup"><span data-stu-id="8b11f-122">Response</span></span>

<span data-ttu-id="8b11f-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8b11f-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b11f-125">例</span><span class="sxs-lookup"><span data-stu-id="8b11f-125">Example</span></span>
<span data-ttu-id="8b11f-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8b11f-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b11f-127">要求</span><span class="sxs-lookup"><span data-stu-id="8b11f-127">Request</span></span>
<span data-ttu-id="8b11f-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b11f-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="8b11f-129">応答</span><span class="sxs-lookup"><span data-stu-id="8b11f-129">Response</span></span>
<span data-ttu-id="8b11f-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8b11f-130">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->