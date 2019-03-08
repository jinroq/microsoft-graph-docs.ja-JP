---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 再開可能なファイルアップロード
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0495a0c63400d6476c1ad9312e708b9ac880e42
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482393"
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="69c18-102">アップロード セッションを使ってサイズの大きなファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="69c18-102">Upload large files with an upload session</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69c18-p101">アプリで最大ファイル サイズまでファイルをアップロードできるようにするには、アップロード セッションを作成します。アップロード セッションにより、アプリは一連の API 要求で広範なファイルをアップロードでき、このため、アップロードの進行中に接続が切れた場合に転送を再開できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="69c18-105">アップロード セッションを使ってファイルをアップロードするには、次の 2 つの手順を行います。</span><span class="sxs-lookup"><span data-stu-id="69c18-105">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="69c18-106">アップロード セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="69c18-106">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="69c18-107">アップロード セッションにバイトをアップロードする</span><span class="sxs-lookup"><span data-stu-id="69c18-107">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="69c18-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69c18-108">Permissions</span></span>

<span data-ttu-id="69c18-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69c18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69c18-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69c18-111">Permission type</span></span>      | <span data-ttu-id="69c18-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69c18-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69c18-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69c18-113">Delegated (work or school account)</span></span> | <span data-ttu-id="69c18-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c18-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="69c18-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69c18-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69c18-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c18-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="69c18-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69c18-117">Application</span></span> | <span data-ttu-id="69c18-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c18-118">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="69c18-119">アップロード セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="69c18-119">Create an upload session</span></span>

<span data-ttu-id="69c18-120">サイズが大きいファイルのアップロードを開始するには、アプリがまず新しいアップロード セッションを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-120">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="69c18-121">これにより、完全なファイルがアップロードされるまでファイルのバイトが保存される、一時的な保存場所が作成されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-121">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="69c18-122">ファイルの最後のバイトがアップロードされると、アップロード セッションは完了し、最終的なファイルがアップロード先のフォルダーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-122">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="69c18-123">または、要求の引数にプロパティを`deferCommit`設定することによって、アップロードの完了要求を明示的に行うまで、移行先でのファイルの最終的な作成を遅延させることができます。</span><span class="sxs-lookup"><span data-stu-id="69c18-123">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="69c18-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69c18-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="69c18-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="69c18-125">Request body</span></span>

<span data-ttu-id="69c18-126">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="69c18-126">No request body is required.</span></span>
<span data-ttu-id="69c18-127">ただし、要求本文でプロパティを指定して、アップロードされるファイルに関する追加データを提供したり、アップロード操作のセマンティクスをカスタマイズしたりすることができます。</span><span class="sxs-lookup"><span data-stu-id="69c18-127">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="69c18-128">たとえば、 `item`プロパティで次のパラメーターを設定できます。<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span><span class="sxs-lookup"><span data-stu-id="69c18-128">For example, the `item` property allows setting the following parameters: <!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span></span>
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

<span data-ttu-id="69c18-129">次の例では、filename が既に取得されている場合の動作を制御し、明示的な完了要求が行われるまで最終的なファイルを作成しないように指定しています。</span><span class="sxs-lookup"><span data-stu-id="69c18-129">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="69c18-130">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69c18-130">Optional request headers</span></span>

| <span data-ttu-id="69c18-131">名前</span><span class="sxs-lookup"><span data-stu-id="69c18-131">Name</span></span>       | <span data-ttu-id="69c18-132">値</span><span class="sxs-lookup"><span data-stu-id="69c18-132">Value</span></span> | <span data-ttu-id="69c18-133">説明</span><span class="sxs-lookup"><span data-stu-id="69c18-133">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="69c18-134">*if-match*</span><span class="sxs-lookup"><span data-stu-id="69c18-134">*if-match*</span></span> | <span data-ttu-id="69c18-135">etag</span><span class="sxs-lookup"><span data-stu-id="69c18-135">etag</span></span>  | <span data-ttu-id="69c18-136">この要求ヘッダーが含まれていて、指定された etag (または ctag) がアイテムの現在の`412 Precondition Failed` etag に一致しない場合は、エラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-136">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="69c18-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="69c18-137">Parameters</span></span>

| <span data-ttu-id="69c18-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="69c18-138">Parameter</span></span>            | <span data-ttu-id="69c18-139">型</span><span class="sxs-lookup"><span data-stu-id="69c18-139">Type</span></span>                          | <span data-ttu-id="69c18-140">説明</span><span class="sxs-lookup"><span data-stu-id="69c18-140">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="69c18-141">item</span><span class="sxs-lookup"><span data-stu-id="69c18-141">item</span></span>                 | <span data-ttu-id="69c18-142">ドライブ itemuploadableproperties</span><span class="sxs-lookup"><span data-stu-id="69c18-142">driveItemUploadableProperties</span></span> | <span data-ttu-id="69c18-143">アップロードされるファイルに関するデータ</span><span class="sxs-lookup"><span data-stu-id="69c18-143">Data about the file being uploaded</span></span>
| <span data-ttu-id="69c18-144">deferCommit</span><span class="sxs-lookup"><span data-stu-id="69c18-144">deferCommit</span></span>          | <span data-ttu-id="69c18-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="69c18-145">Boolean</span></span>                       | <span data-ttu-id="69c18-146">true に設定されている場合、コピー先でのファイルの最終作成では明示的な要求が必要になります。</span><span class="sxs-lookup"><span data-stu-id="69c18-146">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="69c18-147">OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-147">Only on OneDrive for Business.</span></span>

## <a name="item-properties"></a><span data-ttu-id="69c18-148">アイテムのプロパティ</span><span class="sxs-lookup"><span data-stu-id="69c18-148">Item properties</span></span>

| <span data-ttu-id="69c18-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69c18-149">Property</span></span>             | <span data-ttu-id="69c18-150">種類</span><span class="sxs-lookup"><span data-stu-id="69c18-150">Type</span></span>               | <span data-ttu-id="69c18-151">説明</span><span class="sxs-lookup"><span data-stu-id="69c18-151">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="69c18-152">description</span><span class="sxs-lookup"><span data-stu-id="69c18-152">description</span></span>          | <span data-ttu-id="69c18-153">String</span><span class="sxs-lookup"><span data-stu-id="69c18-153">String</span></span>             | <span data-ttu-id="69c18-154">ユーザーに表示されるアイテムの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="69c18-154">Provides a user-visible description of the item.</span></span> <span data-ttu-id="69c18-155">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="69c18-155">Read-write.</span></span> <span data-ttu-id="69c18-156">OneDrive Personal のみ</span><span class="sxs-lookup"><span data-stu-id="69c18-156">Only on OneDrive Personal.</span></span>
| <span data-ttu-id="69c18-157">name</span><span class="sxs-lookup"><span data-stu-id="69c18-157">name</span></span>                 | <span data-ttu-id="69c18-158">文字列</span><span class="sxs-lookup"><span data-stu-id="69c18-158">String</span></span>             | <span data-ttu-id="69c18-p107">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="69c18-p107">The name of the item (filename and extension). Read-write.</span></span>

### <a name="request"></a><span data-ttu-id="69c18-161">要求</span><span class="sxs-lookup"><span data-stu-id="69c18-161">Request</span></span>

<span data-ttu-id="69c18-162">この要求への応答により、新たに作成された [uploadSession](../resources/uploadsession.md) の詳細 (ファイルの各部分をアップロードするために使用される URL など) が指定されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-162">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="69c18-163">応答</span><span class="sxs-lookup"><span data-stu-id="69c18-163">Response</span></span>

<span data-ttu-id="69c18-164">成功した場合、この要求への応答では残りの要求を送信する場所に関する詳細が [UploadSession](../resources/uploadsession.md) リソースとして提示されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-164">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="69c18-165">このリソースは、ファイルのバイト範囲をどこにアップロードするか、およびアップロード セッションがいつ期限切れになるかに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="69c18-165">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="69c18-166">アップロード セッションにバイトをアップロードする</span><span class="sxs-lookup"><span data-stu-id="69c18-166">Upload bytes to the upload session</span></span>

<span data-ttu-id="69c18-167">ファイル、またはファイルの一部をアップロードするために、アプリは **createUploadSession** 応答で受け取った **uploadUrl** 値への PUT 要求を出します。</span><span class="sxs-lookup"><span data-stu-id="69c18-167">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="69c18-168">どの要求の最大バイト数も 60 MiB 未満である限り、ファイル全体をアップロードすることも、ファイルをいくつかのバイト範囲に分割することも可能です。</span><span class="sxs-lookup"><span data-stu-id="69c18-168">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="69c18-169">ファイルのフラグメントは、順番にアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-169">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="69c18-170">誤った順序でアップロードすると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="69c18-170">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="69c18-171">**注:** アプリがファイルを複数のバイト範囲に分割する場合、各バイト範囲のサイズは 320 KiB (327,680 バイト) の倍数である**必要があります**。</span><span class="sxs-lookup"><span data-stu-id="69c18-171">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="69c18-172">320 KiB で均等に分割できないフラグメント サイズを使用した場合、一部のファイルのコミット中にエラーになります。</span><span class="sxs-lookup"><span data-stu-id="69c18-172">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="69c18-173">例</span><span class="sxs-lookup"><span data-stu-id="69c18-173">Example</span></span>

<span data-ttu-id="69c18-174">この例では、128 バイトのファイルのうち、最初の 26 バイトをアプリがアップロードします。</span><span class="sxs-lookup"><span data-stu-id="69c18-174">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="69c18-175">**Content-Length** ヘッダーは、現在の要求のサイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="69c18-175">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="69c18-176">**Content-Range** ヘッダーは、ファイル全体の中でこの要求が表すバイト範囲を示します。</span><span class="sxs-lookup"><span data-stu-id="69c18-176">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="69c18-177">ファイルの最初のフラグメントをアップロードする前に、ファイルの長さの合計がわかっています。</span><span class="sxs-lookup"><span data-stu-id="69c18-177">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="69c18-178">**重要:** アプリは、**Content-Range** ヘッダーで指定されるファイル サイズ合計をすべての要求で同じに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-178">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="69c18-179">異なるファイル サイズのバイト範囲が宣言された場合、要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="69c18-179">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="69c18-180">応答</span><span class="sxs-lookup"><span data-stu-id="69c18-180">Response</span></span>

<span data-ttu-id="69c18-181">要求の完了時に、アップロードする必要のあるバイト範囲がまだ存在している場合、サーバーは `202 Accepted` で応答します。</span><span class="sxs-lookup"><span data-stu-id="69c18-181">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="69c18-182">アプリは **nextExpectedRanges** の値を使用して、次のバイト範囲の開始点を判断できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-182">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="69c18-183">サーバーがまだ受信していないファイル部分を示す、複数の範囲指定が表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="69c18-183">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="69c18-184">これは、中断された転送を再開する必要があり、クライアント側にとってサービスの状態が不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="69c18-184">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="69c18-185">常に以下のベスト プラクティスに従って、バイト範囲のサイズを決定してください。</span><span class="sxs-lookup"><span data-stu-id="69c18-185">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="69c18-186">アップロードするバイト範囲の正しいサイズの範囲を **nextExpectedRanges** が返すことを想定しないでください。</span><span class="sxs-lookup"><span data-stu-id="69c18-186">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="69c18-187">**nextExpectedRanges** プロパティは、まだ受信されていないファイルの範囲を示します。アプリによるファイル アップロード方法のパターンを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="69c18-187">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="69c18-188">備考</span><span class="sxs-lookup"><span data-stu-id="69c18-188">Remarks</span></span>

* <span data-ttu-id="69c18-189">`nextExpectedRanges` プロパティは、欠落してするすべての範囲の一覧を必ずしも示すわけではありません。</span><span class="sxs-lookup"><span data-stu-id="69c18-189">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="69c18-p114">フラグメントの書き込みが成功すると、次の開始点の範囲が返されます (例: "523-")。</span><span class="sxs-lookup"><span data-stu-id="69c18-p114">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="69c18-p115">サーバーが既に受信していたフラグメントをクライアントが送信した場合のエラーでは、サーバーから `HTTP 416 Requested Range Not Satisfiable` の応答が返されます。受信されていない範囲のより詳細なリストを取得するために、[アップロード ステータスを要求](#resuming-an-in-progress-upload)できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-p115">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="69c18-p116">`PUT` の呼び出しを発行するときに、承認ヘッダーを含めると、`HTTP 401 Unauthorized` 応答が発生する可能性があります。承認ヘッダーとベアラー トークンは、最初の手順で `POST` を発行するときにのみ送信する必要があります。`PUT` を発行する場合は、含めないようにします。</span><span class="sxs-lookup"><span data-stu-id="69c18-p116">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="69c18-197">ファイルの完成</span><span class="sxs-lookup"><span data-stu-id="69c18-197">Completing a file</span></span>

<span data-ttu-id="69c18-198">が`deferCommit` false または unset の場合は、ファイルの最後のバイト範囲がアップロード URL に格納されると、アップロードが自動的に完了します。</span><span class="sxs-lookup"><span data-stu-id="69c18-198">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>
<span data-ttu-id="69c18-199">が`deferCommit` true の場合は、ファイルの最後のバイト範囲がアップロード url に配置された後に、長さがゼロのコンテンツを含むアップロード url への最終 POST 要求によってアップロードが明示的に完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-199">If `deferCommit` is true, then after the final byte range of the file is PUT to the upload URL, the upload should be explicitly completed by a final POST request to the upload url with zero-length content.</span></span>

<span data-ttu-id="69c18-200">アップロードが完了すると、サーバーは、 `HTTP 201 Created`または`HTTP 200 OK`の最後の要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="69c18-200">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="69c18-201">また、応答本文には、完成したファイルを表す **driveItem** の既定のプロパティ セットも含まれます。</span><span class="sxs-lookup"><span data-stu-id="69c18-201">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```


<!-- { "blockType": "request", "opaqueUrl": true, "name": "commit-upload", "scopes": "files.readwrite" } -->

```
POST https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 0
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="handling-upload-conflicts"></a><span data-ttu-id="69c18-202">アップロード競合の処理</span><span class="sxs-lookup"><span data-stu-id="69c18-202">Handling upload conflicts</span></span>

<span data-ttu-id="69c18-203">ファイルのアップロード後に競合が発生した場合 (たとえば、アップロード セッション中に同じ名前のアイテムが作成された場合) には、最後のバイト範囲がアップロードされたときにエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-203">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="69c18-204">アップロード セッションを取り消す</span><span class="sxs-lookup"><span data-stu-id="69c18-204">Cancel the upload session</span></span>

<span data-ttu-id="69c18-p119">アップロード セッションを取り消すには、アップロード URL に DELETE 要求を送信します。これにより、以前にアップロードしたデータを格納している一時ファイルがクリーンアップされます。これは、たとえばユーザーが転送を取り消した場合など、アップロードが中断される場合に使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-p119">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="69c18-208">一時ファイルとそれに伴うアップロード セッションは、**expirationDateTime** が経過した後、自動的にクリーンアップされます。</span><span class="sxs-lookup"><span data-stu-id="69c18-208">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="69c18-209">期限が経過しても、一時ファイルはただちに削除されるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="69c18-209">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="69c18-210">要求</span><span class="sxs-lookup"><span data-stu-id="69c18-210">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="69c18-211">応答</span><span class="sxs-lookup"><span data-stu-id="69c18-211">Response</span></span>

<span data-ttu-id="69c18-212">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="69c18-212">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="69c18-213">進行中のアップロードを再開する</span><span class="sxs-lookup"><span data-stu-id="69c18-213">Resuming an in-progress upload</span></span>

<span data-ttu-id="69c18-p121">あるアップロード要求が完了する前に、要求が切断されるか失敗すると、その要求のすべてのバイトが無視されます。これは、アプリとサービス間の接続が切断された場合に発生することがあります。このような場合、アプリは直前に完了したフラグメントからファイル転送を再開できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-p121">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="69c18-217">以前受信されたバイト範囲を知るために、アプリはアップロード セッションのステータスを要求できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-217">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="69c18-218">例</span><span class="sxs-lookup"><span data-stu-id="69c18-218">Example</span></span>

<span data-ttu-id="69c18-219">`uploadUrl` に GET 要求を送信して、アップロードのステータスを照会します。</span><span class="sxs-lookup"><span data-stu-id="69c18-219">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="69c18-220">サーバーは応答で、アップロードが必要な、送信されなかったバイトの範囲のリストと、アップロード セッションの有効期限を返します。</span><span class="sxs-lookup"><span data-stu-id="69c18-220">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="69c18-221">残りのデータをアップロードする</span><span class="sxs-lookup"><span data-stu-id="69c18-221">Upload remaining data</span></span>

<span data-ttu-id="69c18-222">アプリにアップロードの開始点がわかると、[「アップロード セッションにバイトをアップロードする」](#upload-bytes-to-the-upload-session)の次の手順でアップロードを再開します。</span><span class="sxs-lookup"><span data-stu-id="69c18-222">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="69c18-223">アップロード エラーの処理</span><span class="sxs-lookup"><span data-stu-id="69c18-223">Handle upload errors</span></span>

<span data-ttu-id="69c18-224">ファイルの最後のバイト範囲がアップロードされるときに、エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-224">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="69c18-225">この原因として、名前の競合またはクォータ制限の超過が考えられます。</span><span class="sxs-lookup"><span data-stu-id="69c18-225">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="69c18-226">アップロード セッションは有効期限が切れるまで保持されるので、アプリはアップロード セッションを明示的にコミットすることで、アップロードを回復することができます。</span><span class="sxs-lookup"><span data-stu-id="69c18-226">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="69c18-227">アプリでアップロード セッションを明示的にコミットするには、アップロード セッションのコミット時に使用される新しい **driveItem** リソースを使って PUT 要求を出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-227">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="69c18-228">この新しい要求により、元のアップロード エラーの原因となったエラーが修正されるはずです。</span><span class="sxs-lookup"><span data-stu-id="69c18-228">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="69c18-229">既存のアップロード セッションをアプリでコミットすることを示すために、アップロード セッション URL の値を指定する `@microsoft.graph.sourceUrl` プロパティを PUT 要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-229">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="69c18-230">**注:** この呼び出しでは、想定どおりに `@microsoft.graph.conflictBehavior` ヘッダーと `if-match` ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="69c18-230">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="response"></a><span data-ttu-id="69c18-231">応答</span><span class="sxs-lookup"><span data-stu-id="69c18-231">Response</span></span>

<span data-ttu-id="69c18-232">新しいメタデータを使用してファイルをコミットできる場合は、`HTTP 201 Created` または `HTTP 200 OK` の応答が、アップロードしたファイルのアイテム メタデータとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="69c18-232">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="best-practices"></a><span data-ttu-id="69c18-233">ベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="69c18-233">Best practices</span></span>

* <span data-ttu-id="69c18-234">接続の中断や 5xx エラーにより失敗したアップロードは、次のように再開または再試行します。</span><span class="sxs-lookup"><span data-stu-id="69c18-234">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="69c18-235">アップロード要求を再開または再試行するときに 5xx サーバー エラーが返された場合には、指数近似バックオフを使用します。</span><span class="sxs-lookup"><span data-stu-id="69c18-235">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="69c18-236">その他のエラーの場合は指数近似バックオフは使わず、再試行回数を制限する必要があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-236">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="69c18-237">再開可能なアップロードの実行中に発生した `404 Not Found` エラーに対処するには、アップロード全体を最初からやり直します。</span><span class="sxs-lookup"><span data-stu-id="69c18-237">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="69c18-238">これは、アップロード セッションがもはや存在しなくなったことを示します。</span><span class="sxs-lookup"><span data-stu-id="69c18-238">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="69c18-239">10 MiB (10,485,760 バイト) を超えるサイズのファイルには、再開可能なファイル転送を使用します。</span><span class="sxs-lookup"><span data-stu-id="69c18-239">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="69c18-240">安定した高速接続で最適なバイト範囲サイズは 10 MiB です。</span><span class="sxs-lookup"><span data-stu-id="69c18-240">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="69c18-241">より低速な、または信頼性の低い接続では、フラグメント サイズをより小さくした方が良い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="69c18-241">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="69c18-242">推奨されるフラグメント サイズは、5～10 MiB です。</span><span class="sxs-lookup"><span data-stu-id="69c18-242">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="69c18-243">320 KiB (327,680 バイト) の倍数のバイト範囲サイズを使用してください。</span><span class="sxs-lookup"><span data-stu-id="69c18-243">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="69c18-244">320 KiB の倍数ではないフラグメント サイズを使用した場合、最後のバイト範囲をアップロードした後に、サイズの大きなファイルの転送が失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="69c18-244">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="69c18-245">エラー応答</span><span class="sxs-lookup"><span data-stu-id="69c18-245">Error responses</span></span>

<span data-ttu-id="69c18-246">エラーがどのように返されるかについては、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="69c18-246">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createuploadsession.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
