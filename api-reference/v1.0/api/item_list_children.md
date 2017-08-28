# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="6067b-101">driveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6067b-101">List children of a driveItem</span></span>

<span data-ttu-id="6067b-102">DriveItem の**子**リレーションシップで [DriveItems](../resources/driveitem.md) のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6067b-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="6067b-103">NULL でない **folder** または **package** ファセットがある DriveItems は、1 つ以上の子 DriveItems を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="6067b-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="6067b-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6067b-104">Permissions</span></span>
<span data-ttu-id="6067b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6067b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6067b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6067b-107">Permission type</span></span>      | <span data-ttu-id="6067b-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6067b-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6067b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6067b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6067b-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6067b-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6067b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6067b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6067b-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6067b-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6067b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6067b-113">Application</span></span> | <span data-ttu-id="6067b-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6067b-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6067b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6067b-115">HTTP request</span></span>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6067b-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6067b-116">Optional query parameters</span></span>
<span data-ttu-id="6067b-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6067b-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6067b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6067b-118">Request headers</span></span>

| <span data-ttu-id="6067b-119">名前</span><span class="sxs-lookup"><span data-stu-id="6067b-119">Name</span></span>          | <span data-ttu-id="6067b-120">型</span><span class="sxs-lookup"><span data-stu-id="6067b-120">Type</span></span>   | <span data-ttu-id="6067b-121">説明</span><span class="sxs-lookup"><span data-stu-id="6067b-121">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6067b-122">if-none-match</span><span class="sxs-lookup"><span data-stu-id="6067b-122">if-none-match</span></span> | <span data-ttu-id="6067b-123">String</span><span class="sxs-lookup"><span data-stu-id="6067b-123">String</span></span> | <span data-ttu-id="6067b-124">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6067b-124">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6067b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6067b-125">Request body</span></span>
<span data-ttu-id="6067b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6067b-126">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="6067b-127">例</span><span class="sxs-lookup"><span data-stu-id="6067b-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6067b-128">要求</span><span class="sxs-lookup"><span data-stu-id="6067b-128">Request</span></span>
<span data-ttu-id="6067b-129">現在のユーザーの OneDrive のルート フォルダーで DriveItems を返す要求の例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="6067b-129">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a><span data-ttu-id="6067b-130">応答</span><span class="sxs-lookup"><span data-stu-id="6067b-130">Response</span></span>

<span data-ttu-id="6067b-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6067b-131">Here is an example of the response.</span></span>
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

<span data-ttu-id="6067b-132">**注:**コレクションが既定のページ サイズ (200 アイテム) を超えた場合は、応答で **@odata.nextLink** プロパティが返され、より多くのアイテムが使用できることが示されます。また、アイテムの次のページの要求 URL も提供されます。</span><span class="sxs-lookup"><span data-stu-id="6067b-132">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="6067b-133">ページのサイズは[オプションのクエリ文字列パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)で制御できます。</span><span class="sxs-lookup"><span data-stu-id="6067b-133">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
