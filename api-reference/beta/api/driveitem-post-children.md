---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 新しいフォルダーを作成する
localization_priority: Normal
ms.openlocfilehash: 113c9adaa54979fb4c80b23fd2c4cd4c69f8d09a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887396"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="81575-102">ドライブに新しいフォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="81575-102">Create a new folder in a drive</span></span>

> <span data-ttu-id="81575-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81575-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81575-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81575-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81575-105">新しいフォルダーまたは [DriveItem](../resources/driveitem.md) を、指定された親アイテムやパスと共に[ドライブ](../resources/drive.md)内に作成します。</span><span class="sxs-lookup"><span data-stu-id="81575-105">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="81575-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81575-106">Permissions</span></span>

<span data-ttu-id="81575-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81575-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81575-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81575-109">Permission type</span></span>      | <span data-ttu-id="81575-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81575-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81575-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81575-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81575-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81575-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="81575-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81575-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81575-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81575-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="81575-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81575-115">Application</span></span> | <span data-ttu-id="81575-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81575-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81575-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81575-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="81575-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="81575-118">Request body</span></span>

<span data-ttu-id="81575-119">要求本文で、作成する [DriveItem](../resources/driveitem.md) リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81575-119">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="81575-120">応答</span><span class="sxs-lookup"><span data-stu-id="81575-120">Response</span></span>

<span data-ttu-id="81575-121">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Driveitem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="81575-121">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81575-122">例</span><span class="sxs-lookup"><span data-stu-id="81575-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="81575-123">要求</span><span class="sxs-lookup"><span data-stu-id="81575-123">Request</span></span>

<span data-ttu-id="81575-124">以下は、サインイン ユーザーの OneDrive のルート フォルダーに新しいフォルダーを作成する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81575-124">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="81575-125">使用されている `@microsoft.graph.conflictBehavior` プロパティは、アイテムが同じ名前ですでに存在する場合に、サービスはフォルダーを作成する際にフォルダーの新しい名前を選択する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="81575-125">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>

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

### <a name="response"></a><span data-ttu-id="81575-126">応答</span><span class="sxs-lookup"><span data-stu-id="81575-126">Response</span></span>

<span data-ttu-id="81575-127">成功した場合、このメソッドは新しく作成されたフォルダーを [DriveItem] [item-resource] リソースとして返します。</span><span class="sxs-lookup"><span data-stu-id="81575-127">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="81575-128">エラー応答</span><span class="sxs-lookup"><span data-stu-id="81575-128">Error response</span></span>

<span data-ttu-id="81575-129">エラーがどのように返されるかについては、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="81575-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>
[エラー応答]: 項目のリソースのエラー/グラフ/:./resources/driveitem.md フォルダーとファセット。.. 説明。/resources/folder.md
[error-response]: /graph/errors [item-resource]: ../resources/driveitem.md [folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder"
} -->
