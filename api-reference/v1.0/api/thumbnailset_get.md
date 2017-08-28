# <a name="get-thumbnailset"></a><span data-ttu-id="b1d95-101">thumbnailSet を取得する　</span><span class="sxs-lookup"><span data-stu-id="b1d95-101">Get thumbnailSet</span></span>

<span data-ttu-id="b1d95-102">[thumbnailSet](../resources/thumbnailset.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b1d95-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="b1d95-103">詳細については、「[サムネイルを一覧表示する](item_list_thumbnails.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1d95-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1d95-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1d95-104">Prerequisites</span></span>
<span data-ttu-id="b1d95-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1d95-105">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="b1d95-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="b1d95-106">Files.Read</span></span>

## <a name="http-request"></a><span data-ttu-id="b1d95-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1d95-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1d95-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b1d95-108">Optional query parameters</span></span>
<span data-ttu-id="b1d95-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b1d95-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1d95-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1d95-110">Request headers</span></span>
| <span data-ttu-id="b1d95-111">名前</span><span class="sxs-lookup"><span data-stu-id="b1d95-111">Name</span></span>       | <span data-ttu-id="b1d95-112">型</span><span class="sxs-lookup"><span data-stu-id="b1d95-112">Type</span></span> | <span data-ttu-id="b1d95-113">説明</span><span class="sxs-lookup"><span data-stu-id="b1d95-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1d95-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1d95-114">Authorization</span></span>  | <span data-ttu-id="b1d95-115">string</span><span class="sxs-lookup"><span data-stu-id="b1d95-115">string</span></span>  | <span data-ttu-id="b1d95-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1d95-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1d95-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1d95-118">Request body</span></span>
<span data-ttu-id="b1d95-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1d95-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1d95-120">応答</span><span class="sxs-lookup"><span data-stu-id="b1d95-120">Response</span></span>

<span data-ttu-id="b1d95-121">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thumbnailSet](../resources/thumbnailset.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b1d95-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1d95-122">例</span><span class="sxs-lookup"><span data-stu-id="b1d95-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1d95-123">要求</span><span class="sxs-lookup"><span data-stu-id="b1d95-123">Request</span></span>
<span data-ttu-id="b1d95-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1d95-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="b1d95-125">応答</span><span class="sxs-lookup"><span data-stu-id="b1d95-125">Response</span></span>
<span data-ttu-id="b1d95-126">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b1d95-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
