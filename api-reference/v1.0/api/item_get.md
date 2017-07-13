# <span data-ttu-id="cd791-101">DriveItem リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="cd791-101">Get a DriveItem resource</span></span>
<a id="get-a-driveitem-resource" class="xliff"></a>

<span data-ttu-id="cd791-102">[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="cd791-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <span data-ttu-id="cd791-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd791-103">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="cd791-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd791-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="cd791-105">Files.Read</span><span class="sxs-lookup"><span data-stu-id="cd791-105">Files.Read</span></span>
* <span data-ttu-id="cd791-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd791-106">Files.ReadWrite</span></span>
* <span data-ttu-id="cd791-107">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd791-107">Files.Read.All</span></span>
* <span data-ttu-id="cd791-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd791-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="cd791-109">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd791-109">Sites.Read.All</span></span>
* <span data-ttu-id="cd791-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd791-110">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="cd791-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd791-111">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="cd791-112">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cd791-112">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="cd791-113">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cd791-113">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="cd791-114">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd791-114">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="cd791-115">名前</span><span class="sxs-lookup"><span data-stu-id="cd791-115">Name</span></span>          | <span data-ttu-id="cd791-116">値</span><span class="sxs-lookup"><span data-stu-id="cd791-116">Value</span></span>  | <span data-ttu-id="cd791-117">説明</span><span class="sxs-lookup"><span data-stu-id="cd791-117">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cd791-118">if-none-match</span><span class="sxs-lookup"><span data-stu-id="cd791-118">if-none-match</span></span> | <span data-ttu-id="cd791-119">String</span><span class="sxs-lookup"><span data-stu-id="cd791-119">String</span></span> | <span data-ttu-id="cd791-120">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="cd791-120">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <span data-ttu-id="cd791-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd791-121">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="cd791-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cd791-122">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="cd791-123">応答</span><span class="sxs-lookup"><span data-stu-id="cd791-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="cd791-124">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="cd791-124">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="cd791-125">例</span><span class="sxs-lookup"><span data-stu-id="cd791-125">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="cd791-126">要求</span><span class="sxs-lookup"><span data-stu-id="cd791-126">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="cd791-127">以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd791-127">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <span data-ttu-id="cd791-128">応答</span><span class="sxs-lookup"><span data-stu-id="cd791-128">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="cd791-129">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cd791-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <span data-ttu-id="cd791-130">メモ</span><span class="sxs-lookup"><span data-stu-id="cd791-130">Notes</span></span>
<a id="notes" class="xliff"></a>

<span data-ttu-id="cd791-131">アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cd791-131">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->
