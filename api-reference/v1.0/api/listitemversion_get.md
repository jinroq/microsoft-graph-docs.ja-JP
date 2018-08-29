# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="fff7c-101">ListItemVersion リソースを取得</span><span class="sxs-lookup"><span data-stu-id="fff7c-101">Get a ListItemVersion resource (preview)</span></span>

<span data-ttu-id="fff7c-102">[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="fff7c-102">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fff7c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fff7c-103">Permissions</span></span>

<span data-ttu-id="fff7c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fff7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="fff7c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fff7c-106">Permission type</span></span>             | <span data-ttu-id="fff7c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fff7c-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fff7c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fff7c-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="fff7c-109">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fff7c-109">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="fff7c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fff7c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fff7c-111">該当なし</span><span class="sxs-lookup"><span data-stu-id="fff7c-111">n/a</span></span>                                         |
| <span data-ttu-id="fff7c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fff7c-112">Application</span></span>                            | <span data-ttu-id="fff7c-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fff7c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="fff7c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fff7c-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="fff7c-115">応答</span><span class="sxs-lookup"><span data-stu-id="fff7c-115">Response</span></span>

<span data-ttu-id="fff7c-116">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fff7c-116">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="fff7c-117">例</span><span class="sxs-lookup"><span data-stu-id="fff7c-117">Example</span></span>

<span data-ttu-id="fff7c-118">この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。</span><span class="sxs-lookup"><span data-stu-id="fff7c-118">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="fff7c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fff7c-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="fff7c-120">応答</span><span class="sxs-lookup"><span data-stu-id="fff7c-120">Response</span></span>

<span data-ttu-id="fff7c-121">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fff7c-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
