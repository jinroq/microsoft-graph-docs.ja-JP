---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サイズの小さいファイルをアップロードする
localization_priority: Normal
ms.openlocfilehash: 3549850f66c3a46eac49b4bac8040b876fc5509b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883231"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="d8744-102">DriveItem の内容をアップロードまたは置換する</span><span class="sxs-lookup"><span data-stu-id="d8744-102">Upload or replace the contents of a DriveItem</span></span>

> <span data-ttu-id="d8744-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8744-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8744-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8744-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8744-p102">簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。このメソッドは、サイズが 4MB までのファイルのみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d8744-p102">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="d8744-107">大きなファイルをアップロードする場合は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](driveitem-createuploadsession.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8744-107">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8744-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d8744-108">Permissions</span></span>

<span data-ttu-id="d8744-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8744-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8744-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8744-111">Permission type</span></span>      | <span data-ttu-id="d8744-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8744-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8744-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8744-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d8744-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8744-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8744-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8744-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8744-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8744-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8744-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8744-117">Application</span></span> | <span data-ttu-id="d8744-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8744-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="d8744-119">HTTP 要求 (既存アイテムを置換する)</span><span class="sxs-lookup"><span data-stu-id="d8744-119">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="d8744-120">HTTP 要求 (新しいファイルをアップロードする)</span><span class="sxs-lookup"><span data-stu-id="d8744-120">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="d8744-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8744-121">Request body</span></span>

<span data-ttu-id="d8744-122">要求の本文の内容は、アップロードするファイルのバイナリ ストリームである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8744-122">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="d8744-123">応答</span><span class="sxs-lookup"><span data-stu-id="d8744-123">Response</span></span>

<span data-ttu-id="d8744-124">成功した場合、このメソッドは新しく作成された、または更新されたファイルの応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d8744-124">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="d8744-125">例 (新しいファイルのアップロード)</span><span class="sxs-lookup"><span data-stu-id="d8744-125">Example (upload a new file)</span></span>

<span data-ttu-id="d8744-126">この例では、"The contents of the file goes here."(ファイルの内容がここに入ります。) という文字列を、</span><span class="sxs-lookup"><span data-stu-id="d8744-126">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="d8744-127">サインインしたユーザーのドライブにある FolderA 下の FileB.txt という名前のファイルにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="d8744-127">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="d8744-128">応答</span><span class="sxs-lookup"><span data-stu-id="d8744-128">Response</span></span>

<span data-ttu-id="d8744-129">成功した場合、このメソッドは、応答本文で新しく作成したファイルの [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="d8744-129">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="d8744-130">例 (既存ファイルの更新)</span><span class="sxs-lookup"><span data-stu-id="d8744-130">Example (updating an existing file)</span></span>

<span data-ttu-id="d8744-131">この例では、既知の ID を持つファイルの内容を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="d8744-131">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="d8744-132">応答</span><span class="sxs-lookup"><span data-stu-id="d8744-132">Response</span></span>

<span data-ttu-id="d8744-133">成功した場合、このメソッドは、新しく作成されたファイルの応答本文で [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="d8744-133">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="d8744-134">エラー応答</span><span class="sxs-lookup"><span data-stu-id="d8744-134">Error responses</span></span>

<span data-ttu-id="d8744-135">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8744-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
