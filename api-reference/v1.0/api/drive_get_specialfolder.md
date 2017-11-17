---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "特殊フォルダーを取得する"
ms.openlocfilehash: 894c0dc2c41441ab8006f58dcf5ccbc9d0043b0a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="e3349-102">名前で特殊フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="e3349-102">Get a special folder by name</span></span>

<span data-ttu-id="e3349-103">特殊なコレクションを使用して、名前で特殊フォルダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="e3349-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="e3349-p101">特殊フォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、OneDrive の既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊フォルダーの名前が変更されたりドライブ内の別の場所に移動されたりした場合でも、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="e3349-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="e3349-p102">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="e3349-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="e3349-108">**注:**読み取り専用のアクセス許可が付与されているときに、存在していない特殊フォルダーを要求すると、`403 Forbidden` エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3349-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3349-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3349-109">Permissions</span></span>

<span data-ttu-id="e3349-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3349-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="e3349-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3349-112">Permission type</span></span>             |                                           <span data-ttu-id="e3349-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3349-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e3349-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3349-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3349-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3349-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="e3349-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3349-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3349-117">Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3349-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="e3349-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3349-118">Application</span></span>                            | <span data-ttu-id="e3349-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3349-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="e3349-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3349-120">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="e3349-121">特殊フォルダー名</span><span class="sxs-lookup"><span data-stu-id="e3349-121">Special folder names</span></span>

<span data-ttu-id="e3349-122">以下の特殊フォルダー名は、OneDrive および OneDrive for Business で使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3349-122">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="e3349-123">名前</span><span class="sxs-lookup"><span data-stu-id="e3349-123">Name</span></span>        | <span data-ttu-id="e3349-124">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="e3349-124">Folder id</span></span>    | <span data-ttu-id="e3349-125">説明</span><span class="sxs-lookup"><span data-stu-id="e3349-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="e3349-126">Documents</span><span class="sxs-lookup"><span data-stu-id="e3349-126">Documents</span></span>   | `documents`  | <span data-ttu-id="e3349-127">ドキュメント フォルダー。</span><span class="sxs-lookup"><span data-stu-id="e3349-127">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="e3349-128">Photos</span><span class="sxs-lookup"><span data-stu-id="e3349-128">Photos</span></span>      | `photos`     | <span data-ttu-id="e3349-129">フォト フォルダー。</span><span class="sxs-lookup"><span data-stu-id="e3349-129">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="e3349-130">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="e3349-130">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="e3349-131">カメラ ロールのバックアップ フォルダー。</span><span class="sxs-lookup"><span data-stu-id="e3349-131">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="e3349-132">App Root</span><span class="sxs-lookup"><span data-stu-id="e3349-132">App Root</span></span>    | `approot`    | <span data-ttu-id="e3349-p104">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="e3349-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="e3349-135">Music</span><span class="sxs-lookup"><span data-stu-id="e3349-135">Music</span></span>       | `music`      | <span data-ttu-id="e3349-136">ミュージック フォルダー。</span><span class="sxs-lookup"><span data-stu-id="e3349-136">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="e3349-137">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3349-137">Optional query parameters</span></span>

<span data-ttu-id="e3349-138">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3349-138">This method supports the `$expand` and `$select` [OData query parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>

## <a name="http-response"></a><span data-ttu-id="e3349-139">HTTP 応答</span><span class="sxs-lookup"><span data-stu-id="e3349-139">HTTP Response</span></span>

<span data-ttu-id="e3349-140">このメソッドは `200 OK` 応答コードと、応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3349-140">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="e3349-141">driveItem のプロパティまたはリレーションシップの追加の呼び出しと合わせて、特殊フォルダーのアドレス指定のメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3349-141">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="e3349-142">特殊フォルダーの子を取得する</span><span class="sxs-lookup"><span data-stu-id="e3349-142">Get direct children of a folder</span></span>

<span data-ttu-id="e3349-143">特殊フォルダーの子を要求する場合は、`children` コレクションを要求するか、子コレクションを展開する [expand](../../../concepts/query_parameters.md) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="e3349-143">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="e3349-144">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3349-144">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="http-response"></a><span data-ttu-id="e3349-145">HTTP 応答</span><span class="sxs-lookup"><span data-stu-id="e3349-145">HTTP response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="e3349-146">備考</span><span class="sxs-lookup"><span data-stu-id="e3349-146">Remarks</span></span>

> <span data-ttu-id="e3349-147">**注:** `specialFolder` ファセットを伴う DriveItem は、アイテムが特殊フォルダーであり、`special` コレクションを介してアクセスできることを示しています。</span><span class="sxs-lookup"><span data-stu-id="e3349-147">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="e3349-148">アプリに読み取り専用アクセス許可が付与されている場合、特殊フォルダーまたは特殊フォルダーの子を取得する要求は、その特殊フォルダーが存在していないと、`404 Not Found` エラーまたは `403 Forbidden` エラーで失敗します。</span><span class="sxs-lookup"><span data-stu-id="e3349-148">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
