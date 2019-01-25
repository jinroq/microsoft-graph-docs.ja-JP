---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 新しいフォルダーを作成する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ac78cc2e223f532c8c97fd413b799bd5cfd594cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522988"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="514fa-102">ドライブに新しいフォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="514fa-102">Create a new folder in a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="514fa-103">新しいフォルダーまたは [DriveItem](../resources/driveitem.md) を、指定された親アイテムやパスと共に[ドライブ](../resources/drive.md)内に作成します。</span><span class="sxs-lookup"><span data-stu-id="514fa-103">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="514fa-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="514fa-104">Permissions</span></span>

<span data-ttu-id="514fa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="514fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="514fa-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="514fa-107">Permission type</span></span>      | <span data-ttu-id="514fa-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="514fa-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="514fa-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="514fa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="514fa-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514fa-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="514fa-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="514fa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="514fa-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514fa-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="514fa-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="514fa-113">Application</span></span> | <span data-ttu-id="514fa-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514fa-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="514fa-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="514fa-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="514fa-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="514fa-116">Request body</span></span>

<span data-ttu-id="514fa-117">要求本文で、作成する [DriveItem](../resources/driveitem.md) リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="514fa-117">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="514fa-118">応答</span><span class="sxs-lookup"><span data-stu-id="514fa-118">Response</span></span>

<span data-ttu-id="514fa-119">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Driveitem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="514fa-119">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="514fa-120">例</span><span class="sxs-lookup"><span data-stu-id="514fa-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="514fa-121">要求</span><span class="sxs-lookup"><span data-stu-id="514fa-121">Request</span></span>

<span data-ttu-id="514fa-122">以下は、サインイン ユーザーの OneDrive のルート フォルダーに新しいフォルダーを作成する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="514fa-122">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="514fa-123">使用されている `@microsoft.graph.conflictBehavior` プロパティは、アイテムが同じ名前ですでに存在する場合に、サービスはフォルダーを作成する際にフォルダーの新しい名前を選択する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="514fa-123">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>

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

### <a name="response"></a><span data-ttu-id="514fa-124">応答</span><span class="sxs-lookup"><span data-stu-id="514fa-124">Response</span></span>

<span data-ttu-id="514fa-125">成功した場合、このメソッドは新しく作成されたフォルダーを [DriveItem] [item-resource] リソースとして返します。</span><span class="sxs-lookup"><span data-stu-id="514fa-125">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="514fa-126">エラー応答</span><span class="sxs-lookup"><span data-stu-id="514fa-126">Error response</span></span>

<span data-ttu-id="514fa-127">エラーがどのように返されるかについては、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="514fa-127">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>
[エラー応答]: 項目のリソースのエラー/グラフ/:./resources/driveitem.md フォルダーとファセット。.. 説明。/resources/folder.md
[error-response]: /graph/errors [item-resource]: ../resources/driveitem.md [folder-facet]: ../resources/folder.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-post-children.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
