---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 新しいフォルダーを作成する
localization_priority: Priority
ms.prod: sharepoint
description: 指定された親アイテムまたはパスを使用して、ドライブに新しいフォルダーまたは DriveItem を作成します。
doc_type: apiPageType
ms.openlocfilehash: a522ee90a09dabeba2cb5bf94a3393b8392e1c1d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015384"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="4be66-103">ドライブに新しいフォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="4be66-103">Create a new folder in a drive</span></span>

<span data-ttu-id="4be66-104">新しいフォルダーまたは [DriveItem](../resources/driveitem.md) を、親アイテムやパスを指定して[ドライブ](../resources/drive.md)に作成します。</span><span class="sxs-lookup"><span data-stu-id="4be66-104">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be66-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4be66-105">Permissions</span></span>

<span data-ttu-id="4be66-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4be66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be66-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4be66-108">Permission type</span></span>      | <span data-ttu-id="4be66-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4be66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be66-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4be66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4be66-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be66-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4be66-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4be66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be66-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be66-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4be66-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4be66-114">Application</span></span> | <span data-ttu-id="4be66-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be66-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be66-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4be66-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="4be66-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="4be66-117">Request body</span></span>

<span data-ttu-id="4be66-118">要求本文で、作成する [DriveItem](../resources/driveitem.md) リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4be66-118">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="4be66-119">応答</span><span class="sxs-lookup"><span data-stu-id="4be66-119">Response</span></span>

<span data-ttu-id="4be66-120">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Driveitem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="4be66-120">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be66-121">例</span><span class="sxs-lookup"><span data-stu-id="4be66-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="4be66-122">要求</span><span class="sxs-lookup"><span data-stu-id="4be66-122">Request</span></span>

<span data-ttu-id="4be66-123">以下は、サインイン ユーザーの OneDrive のルート フォルダーに新しいフォルダーを作成する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4be66-123">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="4be66-124">使用されている `@microsoft.graph.conflictBehavior` プロパティは、同じ名前のアイテムが既に存在する場合に、サービスはフォルダーを作成する際にフォルダーの新しい名前を選択する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="4be66-124">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4be66-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="4be66-125">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-folder", "scopes": "files.readwrite" } -->

```http
POST /me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { },
  "@microsoft.graph.conflictBehavior": "rename"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4be66-126">C#</span><span class="sxs-lookup"><span data-stu-id="4be66-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4be66-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="4be66-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4be66-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4be66-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4be66-129">Java</span><span class="sxs-lookup"><span data-stu-id="4be66-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4be66-130">応答</span><span class="sxs-lookup"><span data-stu-id="4be66-130">Response</span></span>

<span data-ttu-id="4be66-131">成功した場合、このメソッドでは新しく作成されたフォルダーを [DriveItem][item-resource] リソースとして返します。</span><span class="sxs-lookup"><span data-stu-id="4be66-131">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

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
  "createdDateTime": "2016-09-20T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "2016-09-20T14:34:00Z",
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

## <a name="error-response"></a><span data-ttu-id="4be66-132">エラー応答</span><span class="sxs-lookup"><span data-stu-id="4be66-132">Error response</span></span>

<span data-ttu-id="4be66-133">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4be66-133">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
  ]
} -->
