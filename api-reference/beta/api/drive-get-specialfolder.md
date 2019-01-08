---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 特殊フォルダーを取得する
ms.openlocfilehash: 8b8b1186682421a5ab564272fd473cb72819202d
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748501"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="19e92-102">名前で特殊フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="19e92-102">Get a special folder by name</span></span>

> <span data-ttu-id="19e92-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19e92-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19e92-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19e92-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19e92-105">特殊なコレクションを使用して、名前で特殊フォルダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="19e92-105">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="19e92-p102">特殊フォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、OneDrive の既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊フォルダーの名前が変更されたりドライブ内の別の場所に移動されたりした場合でも、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="19e92-p102">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="19e92-p103">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="19e92-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="19e92-110">**注:** 読み取り専用のアクセス許可が付与されているときに、存在していない特殊フォルダーを要求すると、`403 Forbidden` エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="19e92-110">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="19e92-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19e92-111">Permissions</span></span>

<span data-ttu-id="19e92-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19e92-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="19e92-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19e92-114">Permission type</span></span>             |                                           <span data-ttu-id="19e92-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19e92-115">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="19e92-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19e92-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="19e92-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e92-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="19e92-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19e92-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e92-119">Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e92-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="19e92-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19e92-120">Application</span></span>                            | <span data-ttu-id="19e92-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e92-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="19e92-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19e92-122">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="19e92-123">特殊フォルダー名</span><span class="sxs-lookup"><span data-stu-id="19e92-123">Special folder names</span></span>

<span data-ttu-id="19e92-124">以下の特殊フォルダー名は、OneDrive および OneDrive for Business で使用できます。</span><span class="sxs-lookup"><span data-stu-id="19e92-124">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="19e92-125">名前</span><span class="sxs-lookup"><span data-stu-id="19e92-125">Name</span></span>        | <span data-ttu-id="19e92-126">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="19e92-126">Folder id</span></span>    | <span data-ttu-id="19e92-127">説明</span><span class="sxs-lookup"><span data-stu-id="19e92-127">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="19e92-128">Documents</span><span class="sxs-lookup"><span data-stu-id="19e92-128">Documents</span></span>   | `documents`  | <span data-ttu-id="19e92-129">ドキュメント フォルダー。</span><span class="sxs-lookup"><span data-stu-id="19e92-129">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="19e92-130">Photos</span><span class="sxs-lookup"><span data-stu-id="19e92-130">Photos</span></span>      | `photos`     | <span data-ttu-id="19e92-131">フォト フォルダー。</span><span class="sxs-lookup"><span data-stu-id="19e92-131">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="19e92-132">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="19e92-132">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="19e92-133">カメラ ロールのバックアップ フォルダー。</span><span class="sxs-lookup"><span data-stu-id="19e92-133">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="19e92-134">App Root</span><span class="sxs-lookup"><span data-stu-id="19e92-134">App Root</span></span>    | `approot`    | <span data-ttu-id="19e92-p105">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="19e92-p105">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="19e92-137">Music</span><span class="sxs-lookup"><span data-stu-id="19e92-137">Music</span></span>       | `music`      | <span data-ttu-id="19e92-138">ミュージック フォルダー。</span><span class="sxs-lookup"><span data-stu-id="19e92-138">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="19e92-139">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="19e92-139">Optional query parameters</span></span>

<span data-ttu-id="19e92-140">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="19e92-140">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="19e92-141">応答</span><span class="sxs-lookup"><span data-stu-id="19e92-141">Response</span></span>

<span data-ttu-id="19e92-142">このメソッドは `200 OK` 応答コードと、応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19e92-142">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="19e92-143">プロパティや driveItem 上のリレーションシップへの付加的な呼び出しを伴う、特殊フォルダーのインラインのアドレス指定のメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="19e92-143">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="19e92-144">特殊フォルダーの子を取得します。</span><span class="sxs-lookup"><span data-stu-id="19e92-144">Get children of a special folder</span></span>

<span data-ttu-id="19e92-145">特殊フォルダーの子を要求する場合は、`children` コレクションを要求するか、子コレクションを展開する [expand](/graph/query-parameters) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="19e92-145">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="19e92-146">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19e92-146">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="response"></a><span data-ttu-id="19e92-147">応答</span><span class="sxs-lookup"><span data-stu-id="19e92-147">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="19e92-148">備考</span><span class="sxs-lookup"><span data-stu-id="19e92-148">Remarks</span></span>

> <span data-ttu-id="19e92-149">**注:** `specialFolder` ファセットを伴う DriveItem は、アイテムが特殊フォルダーであり、`special` コレクション経由でアクセスできることを示しています。</span><span class="sxs-lookup"><span data-stu-id="19e92-149">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="19e92-150">アプリに読み取り専用アクセス許可が付与されている場合、特殊フォルダーまたは特殊フォルダーの子を取得する要求は、その特殊フォルダーが存在していないと、`404 Not Found` エラーまたは `403 Forbidden` エラーで失敗します。</span><span class="sxs-lookup"><span data-stu-id="19e92-150">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
