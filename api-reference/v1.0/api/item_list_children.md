# <span data-ttu-id="21065-101">driveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="21065-101">List children of a driveItem</span></span>
<a id="list-children-of-a-driveitem" class="xliff"></a>

<span data-ttu-id="21065-102">DriveItem の**子**リレーションシップで [DriveItems](../resources/driveitem.md) のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="21065-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="21065-103">NULL でない **folder** または **package** ファセットがある DriveItems は、1 つ以上の子 DriveItems を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="21065-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <span data-ttu-id="21065-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="21065-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="21065-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="21065-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="21065-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="21065-106">Files.Read</span></span>
* <span data-ttu-id="21065-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21065-107">Files.ReadWrite</span></span>
* <span data-ttu-id="21065-108">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="21065-108">Files.Read.All</span></span>
* <span data-ttu-id="21065-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21065-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="21065-110">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="21065-110">Sites.Read.All</span></span>
* <span data-ttu-id="21065-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21065-111">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="21065-112">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21065-112">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="21065-113">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="21065-113">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="21065-114">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="21065-114">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="21065-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21065-115">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="21065-116">名前</span><span class="sxs-lookup"><span data-stu-id="21065-116">Name</span></span>          | <span data-ttu-id="21065-117">型</span><span class="sxs-lookup"><span data-stu-id="21065-117">Type</span></span>   | <span data-ttu-id="21065-118">説明</span><span class="sxs-lookup"><span data-stu-id="21065-118">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="21065-119">if-none-match</span><span class="sxs-lookup"><span data-stu-id="21065-119">if-none-match</span></span> | <span data-ttu-id="21065-120">String</span><span class="sxs-lookup"><span data-stu-id="21065-120">String</span></span> | <span data-ttu-id="21065-121">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="21065-121">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <span data-ttu-id="21065-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="21065-122">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="21065-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="21065-123">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="21065-124">例</span><span class="sxs-lookup"><span data-stu-id="21065-124">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="21065-125">要求</span><span class="sxs-lookup"><span data-stu-id="21065-125">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="21065-126">現在のユーザーの OneDrive のルート フォルダーで DriveItems を返す要求の例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="21065-126">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <span data-ttu-id="21065-127">応答</span><span class="sxs-lookup"><span data-stu-id="21065-127">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="21065-128">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="21065-128">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="21065-129">**注:**コレクションが既定のページ サイズ (200 アイテム) を超えた場合は、応答で **@odata.nextLink** プロパティが返され、より多くのアイテムが使用できることが示されます。また、アイテムの次のページの要求 URL も提供されます。</span><span class="sxs-lookup"><span data-stu-id="21065-129">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="21065-130">ページのサイズは[オプションのクエリ文字列パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)で制御できます。</span><span class="sxs-lookup"><span data-stu-id="21065-130">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
