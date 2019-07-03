---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 特別なフォルダーを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3c47db615852f7acfd5e3c63a4abbcb1c5e254a4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461205"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="145b6-102">名前で特殊フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="145b6-102">Get a special folder by name</span></span>

<span data-ttu-id="145b6-103">特殊なコレクションを使用して、名前で特殊フォルダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="145b6-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="145b6-p101">特殊フォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、OneDrive の既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊フォルダーの名前が変更されたりドライブ内の別の場所に移動されたりした場合でも、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="145b6-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="145b6-p102">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="145b6-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="145b6-108">**注:** 読み取り専用のアクセス許可が付与されているときに、存在していない特殊フォルダーを要求すると、`403 Forbidden` エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="145b6-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="145b6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="145b6-109">Permissions</span></span>

<span data-ttu-id="145b6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="145b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="145b6-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="145b6-112">Permission type</span></span>             |                                           <span data-ttu-id="145b6-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="145b6-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="145b6-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="145b6-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="145b6-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145b6-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="145b6-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="145b6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="145b6-117">Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145b6-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="145b6-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="145b6-118">Application</span></span>                            | <span data-ttu-id="145b6-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145b6-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="145b6-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="145b6-120">HTTP Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="145b6-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="145b6-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="145b6-122">C#</span><span class="sxs-lookup"><span data-stu-id="145b6-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="145b6-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="145b6-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="145b6-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="145b6-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a><span data-ttu-id="145b6-125">特殊フォルダー名</span><span class="sxs-lookup"><span data-stu-id="145b6-125">Special folder names</span></span>

<span data-ttu-id="145b6-126">以下の特殊フォルダー名は、OneDrive および OneDrive for Business で使用できます。</span><span class="sxs-lookup"><span data-stu-id="145b6-126">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="145b6-127">名前</span><span class="sxs-lookup"><span data-stu-id="145b6-127">Name</span></span>        | <span data-ttu-id="145b6-128">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="145b6-128">Folder id</span></span>    | <span data-ttu-id="145b6-129">説明</span><span class="sxs-lookup"><span data-stu-id="145b6-129">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="145b6-130">Documents</span><span class="sxs-lookup"><span data-stu-id="145b6-130">Documents</span></span>   | `documents`  | <span data-ttu-id="145b6-131">ドキュメント フォルダー。</span><span class="sxs-lookup"><span data-stu-id="145b6-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="145b6-132">Photos</span><span class="sxs-lookup"><span data-stu-id="145b6-132">Photos</span></span>      | `photos`     | <span data-ttu-id="145b6-133">フォト フォルダー。</span><span class="sxs-lookup"><span data-stu-id="145b6-133">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="145b6-134">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="145b6-134">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="145b6-135">カメラ ロールのバックアップ フォルダー。</span><span class="sxs-lookup"><span data-stu-id="145b6-135">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="145b6-136">App Root</span><span class="sxs-lookup"><span data-stu-id="145b6-136">App Root</span></span>    | `approot`    | <span data-ttu-id="145b6-p104">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="145b6-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="145b6-139">Music</span><span class="sxs-lookup"><span data-stu-id="145b6-139">Music</span></span>       | `music`      | <span data-ttu-id="145b6-140">ミュージック フォルダー。</span><span class="sxs-lookup"><span data-stu-id="145b6-140">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="145b6-141">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="145b6-141">Optional query parameters</span></span>

<span data-ttu-id="145b6-142">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="145b6-142">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="145b6-143">応答</span><span class="sxs-lookup"><span data-stu-id="145b6-143">Response</span></span>

<span data-ttu-id="145b6-144">このメソッドは `200 OK` 応答コードと、応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="145b6-144">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="145b6-145">プロパティや driveItem 上のリレーションシップへの付加的な呼び出しを伴う、特殊フォルダーのインラインのアドレス指定のメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="145b6-145">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="145b6-146">特殊フォルダーの子を取得します。</span><span class="sxs-lookup"><span data-stu-id="145b6-146">Get children of a special folder</span></span>

<span data-ttu-id="145b6-147">特殊フォルダーの子を要求する場合は、`children` コレクションを要求するか、子コレクションを展開する [expand](/graph/query-parameters) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="145b6-147">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="145b6-148">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="145b6-148">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="145b6-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="145b6-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="145b6-150">C#</span><span class="sxs-lookup"><span data-stu-id="145b6-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="145b6-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="145b6-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="145b6-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="145b6-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="145b6-153">応答</span><span class="sxs-lookup"><span data-stu-id="145b6-153">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="145b6-154">注釈</span><span class="sxs-lookup"><span data-stu-id="145b6-154">Remarks</span></span>

> <span data-ttu-id="145b6-155">**注:** `specialFolder` ファセットを伴う DriveItem は、アイテムが特殊フォルダーであり、`special` コレクション経由でアクセスできることを示しています。</span><span class="sxs-lookup"><span data-stu-id="145b6-155">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="145b6-156">アプリに読み取り専用アクセス許可が付与されている場合、特殊フォルダーまたは特殊フォルダーの子を取得する要求は、その特殊フォルダーが存在していないと、`404 Not Found` エラーまたは `403 Forbidden` エラーで失敗します。</span><span class="sxs-lookup"><span data-stu-id="145b6-156">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
} -->
