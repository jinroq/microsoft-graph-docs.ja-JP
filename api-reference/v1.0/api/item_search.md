# <a name="search-for-a-driveitem-within-a-drive"></a><span data-ttu-id="ad3d2-101">ドライブ内の DriveItem を検索する</span><span class="sxs-lookup"><span data-stu-id="ad3d2-101">Search for a DriveItem within a drive</span></span>

<span data-ttu-id="ad3d2-p101">クエリと一致するアイテムを対象にアイテムの階層を検索します。フォルダー階層内、ドライブ全体、または現在のユーザーと共有されるファイル内で検索できます。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p101">Search the hierarchy of items for items matching a query. You can search within a folder hierarhcy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad3d2-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad3d2-104">Permissions</span></span>
<span data-ttu-id="ad3d2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad3d2-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad3d2-107">Permission type</span></span>      | <span data-ttu-id="ad3d2-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad3d2-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ad3d2-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad3d2-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ad3d2-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3d2-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="ad3d2-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad3d2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad3d2-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3d2-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="ad3d2-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad3d2-113">Application</span></span> | <span data-ttu-id="ad3d2-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad3d2-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ad3d2-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad3d2-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```
GET /me/drive/root/search(q='{search-text}')
GET /me/drive/items/{item-id}/search(q='{search-text}')
GET /me/drive/root:/{item-path}:/search(q='{search-text}')
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad3d2-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad3d2-116">Optional query parameters</span></span>
<span data-ttu-id="ad3d2-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="ad3d2-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad3d2-118">Request body</span></span>
<span data-ttu-id="ad3d2-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-119">Do not supply a request body for this method.</span></span>

#### <a name="function-parameters"></a><span data-ttu-id="ad3d2-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad3d2-120">Function parameters</span></span>

| <span data-ttu-id="ad3d2-121">名前</span><span class="sxs-lookup"><span data-stu-id="ad3d2-121">Name</span></span> | <span data-ttu-id="ad3d2-122">値</span><span class="sxs-lookup"><span data-stu-id="ad3d2-122">Value</span></span>  | <span data-ttu-id="ad3d2-123">説明</span><span class="sxs-lookup"><span data-stu-id="ad3d2-123">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| `q`  | <span data-ttu-id="ad3d2-124">string</span><span class="sxs-lookup"><span data-stu-id="ad3d2-124">string</span></span> | <span data-ttu-id="ad3d2-p103">アイテムの検索に使用するクエリ テキスト。値は、ファイル名、メタデータ、およびファイルのコンテンツを含む複数のフィールドに渡って照合できます。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="ad3d2-127">例</span><span class="sxs-lookup"><span data-stu-id="ad3d2-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ad3d2-128">要求</span><span class="sxs-lookup"><span data-stu-id="ad3d2-128">Request</span></span>

<span data-ttu-id="ad3d2-129">ここでは、現在のユーザーの OneDrive を検索する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-129">Here is an example of the request searching the current user's OneDrive</span></span>
<!-- {
  "blockType": "request",
  "name": "item_search"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/search(q='{search-query}')
```

##### <a name="response"></a><span data-ttu-id="ad3d2-130">応答</span><span class="sxs-lookup"><span data-stu-id="ad3d2-130">Response</span></span>
<span data-ttu-id="ad3d2-p104">このメソッドは、検索条件に一致する [DriveItems](../resources/driveitem.md) のコレクション含んでいるオブジェクトを返します。アイテムが見つからない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="ad3d2-p105">一致が多すぎる場合は、応答はページ化され、**@odata.nextLink** プロパティには、後続の結果ページへの URL が含まれます。`$top` クエリ パラメーターを使用すると、ページ内のアイテム数を指定できます。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="ad3d2-135">ユーザーがアクセスできるアイテムの検索</span><span class="sxs-lookup"><span data-stu-id="ad3d2-135">Searching for items a user can access</span></span>

<span data-ttu-id="ad3d2-p106">ドライブ内のアイテムの検索に加えて、アプリでは現在のユーザーと共有されるアイテムを含めるように、検索範囲を広げることができます。検索範囲を広げるには、[Drive](../resources/drive.md) リソースの **search** メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

##### <a name="request"></a><span data-ttu-id="ad3d2-138">要求</span><span class="sxs-lookup"><span data-stu-id="ad3d2-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_search_all"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/search(q='{search-query}')
```

##### <a name="response"></a><span data-ttu-id="ad3d2-139">応答</span><span class="sxs-lookup"><span data-stu-id="ad3d2-139">Response</span></span>
<span data-ttu-id="ad3d2-p107">**ドライブ** リソースからの検索時の応答には、ドライブの外部のアイテム (現在のユーザーと共有されているアイテム) が含まれていることがあります。こうしたアイテムには、それらが対象のドライブの外部に保存されていることを示す、[**remoteItem**](../resources/remoteitem.md) ファセットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ad3d2-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: search",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Items/Search items"
}-->
