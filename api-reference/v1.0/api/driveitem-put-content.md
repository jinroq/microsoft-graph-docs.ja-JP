---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サイズの小さいファイルをアップロードする
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 30899a94783018580227e0d753169bf391ac081d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991546"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="01566-102">DriveItem の内容をアップロードまたは置換する</span><span class="sxs-lookup"><span data-stu-id="01566-102">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="01566-p101">簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。このメソッドは、サイズが 4MB までのファイルのみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="01566-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="01566-105">大きなファイルをアップロードする場合は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](driveitem-createuploadsession.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01566-105">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01566-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="01566-106">Permissions</span></span>

<span data-ttu-id="01566-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01566-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01566-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="01566-109">Permission type</span></span>      | <span data-ttu-id="01566-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="01566-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01566-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="01566-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01566-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01566-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="01566-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="01566-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01566-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01566-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="01566-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="01566-115">Application</span></span> | <span data-ttu-id="01566-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01566-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="01566-117">HTTP 要求 (既存アイテムを置換する)</span><span class="sxs-lookup"><span data-stu-id="01566-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="01566-118">HTTP 要求 (新しいファイルをアップロードする)</span><span class="sxs-lookup"><span data-stu-id="01566-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="01566-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="01566-119">Request body</span></span>

<span data-ttu-id="01566-120">要求の本文の内容は、アップロードするファイルのバイナリ ストリームである必要があります。</span><span class="sxs-lookup"><span data-stu-id="01566-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="01566-121">応答</span><span class="sxs-lookup"><span data-stu-id="01566-121">Response</span></span>

<span data-ttu-id="01566-122">成功した場合、このメソッドは新しく作成された、または更新されたファイルの応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="01566-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="01566-123">例 (新しいファイルのアップロード)</span><span class="sxs-lookup"><span data-stu-id="01566-123">Example (upload a new file)</span></span>

<span data-ttu-id="01566-124">この例では、"The contents of the file goes here."(ファイルの内容がここに入ります。) という文字列を、</span><span class="sxs-lookup"><span data-stu-id="01566-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="01566-125">サインインしたユーザーのドライブにある FolderA 下の FileB.txt という名前のファイルにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="01566-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="01566-126">応答</span><span class="sxs-lookup"><span data-stu-id="01566-126">Response</span></span>

<span data-ttu-id="01566-127">成功した場合、このメソッドは、応答本文で新しく作成したファイルの [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="01566-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="01566-128">例 (既存ファイルの更新)</span><span class="sxs-lookup"><span data-stu-id="01566-128">Example (updating an existing file)</span></span>

<span data-ttu-id="01566-129">この例では、既知の ID を持つファイルの内容を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="01566-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="01566-130">応答</span><span class="sxs-lookup"><span data-stu-id="01566-130">Response</span></span>

<span data-ttu-id="01566-131">成功した場合、このメソッドは、新しく作成されたファイルの応答本文で [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="01566-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="01566-132">エラー応答</span><span class="sxs-lookup"><span data-stu-id="01566-132">Error responses</span></span>

<span data-ttu-id="01566-133">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01566-133">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
