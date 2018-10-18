# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="3b1c8-101">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="3b1c8-101">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="3b1c8-102">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="3b1c8-102">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="3b1c8-103">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="3b1c8-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b1c8-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b1c8-104">Permissions</span></span>

<span data-ttu-id="3b1c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b1c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b1c8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b1c8-107">Permission type</span></span>      | <span data-ttu-id="3b1c8-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b1c8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b1c8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b1c8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3b1c8-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1c8-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b1c8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b1c8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b1c8-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1c8-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b1c8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b1c8-113">Application</span></span> | <span data-ttu-id="3b1c8-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1c8-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b1c8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b1c8-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="3b1c8-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b1c8-116">Request body</span></span>

<span data-ttu-id="3b1c8-117">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="3b1c8-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="3b1c8-118">例</span><span class="sxs-lookup"><span data-stu-id="3b1c8-118">Example</span></span>

<span data-ttu-id="3b1c8-119">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="3b1c8-119">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="3b1c8-120">応答</span><span class="sxs-lookup"><span data-stu-id="3b1c8-120">Response</span></span>

<span data-ttu-id="3b1c8-121">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="3b1c8-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
