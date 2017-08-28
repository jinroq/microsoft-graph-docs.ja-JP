# <a name="create-a-new-folder"></a><span data-ttu-id="e2361-101">新しいフォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="e2361-101">Create a new folder</span></span>

<span data-ttu-id="e2361-102">新しいフォルダーまたは [DriveItem](../resources/driveitem.md) を、指定された親アイテムやパスと共に[ドライブ](../resources/drive.md)内に作成します。</span><span class="sxs-lookup"><span data-stu-id="e2361-102">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2361-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2361-103">Permissions</span></span>
<span data-ttu-id="e2361-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2361-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e2361-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2361-106">Permission type</span></span>      | <span data-ttu-id="e2361-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2361-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2361-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2361-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e2361-109">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2361-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2361-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2361-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2361-111">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2361-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2361-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2361-112">Application</span></span> | <span data-ttu-id="e2361-113">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2361-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2361-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2361-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/children
POST /me/drive/items/{parent-item-id}/children
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="e2361-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2361-115">Request body</span></span>
<span data-ttu-id="e2361-116">要求本文で、作成する [DriveItem](../resources/driveitem.md) リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2361-116">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="e2361-117">応答</span><span class="sxs-lookup"><span data-stu-id="e2361-117">Response</span></span>

<span data-ttu-id="e2361-118">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Driveitem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="e2361-118">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2361-119">例</span><span class="sxs-lookup"><span data-stu-id="e2361-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2361-120">要求</span><span class="sxs-lookup"><span data-stu-id="e2361-120">Request</span></span>
<span data-ttu-id="e2361-121">以下は、ユーザーの OneDrive のルートに新しいフォルダーを作成する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2361-121">Here is an example of the request to create a new folder in the user's OneDrive root.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_from_item"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { }
}
```

##### <a name="response"></a><span data-ttu-id="e2361-122">応答</span><span class="sxs-lookup"><span data-stu-id="e2361-122">Response</span></span>

<span data-ttu-id="e2361-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e2361-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "20160920T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "20160920T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create children",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
