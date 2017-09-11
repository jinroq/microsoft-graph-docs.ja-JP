# <a name="get-thumbnailset"></a><span data-ttu-id="5b0a4-101">thumbnailSet を取得する　</span><span class="sxs-lookup"><span data-stu-id="5b0a4-101">Get thumbnailSet</span></span>

<span data-ttu-id="5b0a4-102">[thumbnailSet](../resources/thumbnailset.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="5b0a4-103">詳細については、「[サムネイルを一覧表示する](item_list_thumbnails.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b0a4-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b0a4-104">Permissions</span></span>
<span data-ttu-id="5b0a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5b0a4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b0a4-107">Permission type</span></span>      | <span data-ttu-id="5b0a4-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b0a4-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="5b0a4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b0a4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5b0a4-110">Files.Read</span><span class="sxs-lookup"><span data-stu-id="5b0a4-110">Files.Read</span></span>    | 
|<span data-ttu-id="5b0a4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b0a4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b0a4-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="5b0a4-112">Files.Read</span></span>    | 
|<span data-ttu-id="5b0a4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b0a4-113">Application</span></span> | <span data-ttu-id="5b0a4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-114">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5b0a4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b0a4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b0a4-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b0a4-116">Optional query parameters</span></span>
<span data-ttu-id="5b0a4-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b0a4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b0a4-118">Request headers</span></span>
| <span data-ttu-id="5b0a4-119">名前</span><span class="sxs-lookup"><span data-stu-id="5b0a4-119">Name</span></span>       | <span data-ttu-id="5b0a4-120">型</span><span class="sxs-lookup"><span data-stu-id="5b0a4-120">Type</span></span> | <span data-ttu-id="5b0a4-121">説明</span><span class="sxs-lookup"><span data-stu-id="5b0a4-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b0a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b0a4-122">Authorization</span></span>  | <span data-ttu-id="5b0a4-123">string</span><span class="sxs-lookup"><span data-stu-id="5b0a4-123">string</span></span>  | <span data-ttu-id="5b0a4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5b0a4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b0a4-126">Request body</span></span>
<span data-ttu-id="5b0a4-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b0a4-128">応答</span><span class="sxs-lookup"><span data-stu-id="5b0a4-128">Response</span></span>

<span data-ttu-id="5b0a4-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thumbnailSet](../resources/thumbnailset.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-129">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b0a4-130">例</span><span class="sxs-lookup"><span data-stu-id="5b0a4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b0a4-131">要求</span><span class="sxs-lookup"><span data-stu-id="5b0a4-131">Request</span></span>
<span data-ttu-id="5b0a4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="5b0a4-133">応答</span><span class="sxs-lookup"><span data-stu-id="5b0a4-133">Response</span></span>
<span data-ttu-id="5b0a4-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5b0a4-134">Here is an example of the response.</span></span>
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
