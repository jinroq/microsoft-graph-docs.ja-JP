# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="f25aa-101">DriveItemVersion リソースのコンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="f25aa-101">Download contents of a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="f25aa-102">[DriveItem](../resources/driveitem.md) の特定のバージョンのコンテンツを取得します。</span><span class="sxs-lookup"><span data-stu-id="f25aa-102">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f25aa-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f25aa-103">Permissions</span></span>

<span data-ttu-id="f25aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f25aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f25aa-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f25aa-106">Permission type</span></span>      | <span data-ttu-id="f25aa-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f25aa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f25aa-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f25aa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f25aa-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25aa-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f25aa-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f25aa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f25aa-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25aa-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f25aa-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f25aa-112">Application</span></span> | <span data-ttu-id="f25aa-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25aa-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f25aa-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f25aa-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="f25aa-115">応答</span><span class="sxs-lookup"><span data-stu-id="f25aa-115">Response</span></span>

<span data-ttu-id="f25aa-116">ファイルのバイトの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="f25aa-116">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="f25aa-p102">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="f25aa-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="f25aa-119">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="f25aa-119">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="f25aa-120">例</span><span class="sxs-lookup"><span data-stu-id="f25aa-120">Example</span></span>

<span data-ttu-id="f25aa-121">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="f25aa-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="f25aa-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f25aa-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="f25aa-123">応答</span><span class="sxs-lookup"><span data-stu-id="f25aa-123">Response</span></span>

<span data-ttu-id="f25aa-124">そのバージョンのコンテンツをダウンロードできる場所へのリダイレクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f25aa-124">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="f25aa-125">備考</span><span class="sxs-lookup"><span data-stu-id="f25aa-125">Remarks</span></span>

<span data-ttu-id="f25aa-126">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="f25aa-126">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="f25aa-127">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveItemVersion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="f25aa-127">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
