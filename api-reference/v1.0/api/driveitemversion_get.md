# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="f46cd-101">DriveItemVersion リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="f46cd-101">Get a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="f46cd-102">[DriveItem](../resources/driveitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="f46cd-102">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f46cd-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f46cd-103">Permissions</span></span>

<span data-ttu-id="f46cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f46cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f46cd-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f46cd-106">Permission type</span></span>      | <span data-ttu-id="f46cd-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f46cd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f46cd-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f46cd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f46cd-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f46cd-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f46cd-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f46cd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f46cd-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f46cd-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f46cd-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f46cd-112">Application</span></span> | <span data-ttu-id="f46cd-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f46cd-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f46cd-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f46cd-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="f46cd-115">応答</span><span class="sxs-lookup"><span data-stu-id="f46cd-115">Response</span></span>

<span data-ttu-id="f46cd-116">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f46cd-116">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f46cd-117">例</span><span class="sxs-lookup"><span data-stu-id="f46cd-117">Example</span></span>

<span data-ttu-id="f46cd-118">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="f46cd-118">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="f46cd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f46cd-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="f46cd-120">応答</span><span class="sxs-lookup"><span data-stu-id="f46cd-120">Response</span></span>

<span data-ttu-id="f46cd-121">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f46cd-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="f46cd-122">備考</span><span class="sxs-lookup"><span data-stu-id="f46cd-122">Remarks</span></span>

<span data-ttu-id="f46cd-123">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="f46cd-123">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="f46cd-124">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveItemVersion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="f46cd-124">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
