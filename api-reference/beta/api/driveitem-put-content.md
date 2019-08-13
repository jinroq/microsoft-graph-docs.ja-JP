---
author: JeremyKelley
description: '簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。 '
ms.date: 09/10/2017
title: サイズの小さいファイルをアップロードする
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 31f5c5b472ffa17e643bd118a0111915ab2bf67a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320946"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="d87df-103">DriveItem の内容をアップロードまたは置換する</span><span class="sxs-lookup"><span data-stu-id="d87df-103">Upload or replace the contents of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d87df-p101">簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。このメソッドは、サイズが 4MB までのファイルのみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d87df-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="d87df-106">大きなファイルをアップロードする場合は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](driveitem-createuploadsession.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d87df-106">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d87df-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d87df-107">Permissions</span></span>

<span data-ttu-id="d87df-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d87df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d87df-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d87df-110">Permission type</span></span>      | <span data-ttu-id="d87df-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d87df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d87df-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d87df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d87df-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87df-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d87df-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d87df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d87df-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87df-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d87df-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d87df-116">Application</span></span> | <span data-ttu-id="d87df-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87df-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="d87df-118">HTTP 要求 (既存アイテムを置換する場合)</span><span class="sxs-lookup"><span data-stu-id="d87df-118">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="d87df-119">HTTP 要求 (新しいファイルをアップロードする場合)</span><span class="sxs-lookup"><span data-stu-id="d87df-119">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="d87df-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="d87df-120">Request body</span></span>

<span data-ttu-id="d87df-121">要求の本文の内容は、アップロードするファイルのバイナリ ストリームである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d87df-121">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="d87df-122">応答</span><span class="sxs-lookup"><span data-stu-id="d87df-122">Response</span></span>

<span data-ttu-id="d87df-123">成功した場合、このメソッドは、新しく作成されたファイルまたは更新されたファイルの応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d87df-123">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="d87df-124">例 (新しいファイルのアップロード)</span><span class="sxs-lookup"><span data-stu-id="d87df-124">Example (upload a new file)</span></span>

<span data-ttu-id="d87df-125">この例では、"The contents of the file goes here."(ファイルの内容がここに入ります。) という文字列を、</span><span class="sxs-lookup"><span data-stu-id="d87df-125">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="d87df-126">サインインしたユーザーのドライブの FolderA の下の FileB.txt という名前のファイルにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="d87df-126">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="d87df-127">応答</span><span class="sxs-lookup"><span data-stu-id="d87df-127">Response</span></span>

<span data-ttu-id="d87df-128">成功した場合、このメソッド[][item-resource]は、新しく作成または更新されたファイルの応答本文で、ファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="d87df-128">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created or updated file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="d87df-129">例 (既存ファイルの更新)</span><span class="sxs-lookup"><span data-stu-id="d87df-129">Example (updating an existing file)</span></span>

<span data-ttu-id="d87df-130">この例では、既知の ID を持つファイルの内容を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="d87df-130">This example replaces the contents of a file with a known ID.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d87df-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d87df-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d87df-132">C#</span><span class="sxs-lookup"><span data-stu-id="d87df-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upload-via-put-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d87df-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d87df-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upload-via-put-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d87df-134">応答</span><span class="sxs-lookup"><span data-stu-id="d87df-134">Response</span></span>

<span data-ttu-id="d87df-135">成功した場合、このメソッドは、新しく作成されたファイルの応答本文で [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="d87df-135">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="d87df-136">エラー応答</span><span class="sxs-lookup"><span data-stu-id="d87df-136">Error responses</span></span>

<span data-ttu-id="d87df-137">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d87df-137">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
  ]
}
-->
