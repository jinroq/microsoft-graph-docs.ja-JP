---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 再開可能なファイル アップロード
ms.openlocfilehash: 09f76b4427df446b2f063827029473a11dba6341
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067080"
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="94435-102">アップロード セッションを使ってサイズが大きいファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="94435-102">Upload large files with an upload session</span></span>

> <span data-ttu-id="94435-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94435-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94435-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94435-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94435-p102">アプリで最大ファイル サイズまでファイルをアップロードできるようにするには、アップロード セッションを作成します。アップロード セッションにより、アプリは一連の API 要求で広範なファイルをアップロードでき、このため、アップロードの進行中に接続が切れた場合に転送を再開できます。</span><span class="sxs-lookup"><span data-stu-id="94435-p102">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="94435-107">アップロード セッションを使ってファイルをアップロードするには、次の 2 つの手順を行います。</span><span class="sxs-lookup"><span data-stu-id="94435-107">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="94435-108">アップロード セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="94435-108">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="94435-109">アップロード セッションにバイトをアップロードする</span><span class="sxs-lookup"><span data-stu-id="94435-109">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="94435-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94435-110">Permissions</span></span>

<span data-ttu-id="94435-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94435-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94435-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94435-113">Permission type</span></span>      | <span data-ttu-id="94435-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94435-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94435-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94435-115">Delegated (work or school account)</span></span> | <span data-ttu-id="94435-116">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94435-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="94435-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94435-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94435-118">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94435-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="94435-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94435-119">Application</span></span> | <span data-ttu-id="94435-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94435-120">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="94435-121">アップロード セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="94435-121">Create an upload session</span></span>

<span data-ttu-id="94435-122">大きなファイルのアップロードを開始するには、アプリはまず新しいアップロード セッションを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-122">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="94435-123">これは、完全なファイルがアップロードされるまで、ファイルのバイト数が保存される場所の一時的な保存場所を作成します。</span><span class="sxs-lookup"><span data-stu-id="94435-123">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="94435-124">ファイルの最後のバイトがアップロードされた後は、アップロード セッションが完了し、最終的なファイルがコピー先のフォルダーに表示されています。</span><span class="sxs-lookup"><span data-stu-id="94435-124">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="94435-125">明示的に設定することにより、アップロードを完了する要求を行うまで、宛先のファイルの最後の作成を延期できます代わりに、`deferCommit`要求の引数のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="94435-125">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="94435-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94435-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="94435-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="94435-127">Request body</span></span>

<span data-ttu-id="94435-128">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="94435-128">No request body is required.</span></span>
<span data-ttu-id="94435-129">ただし、アップロードされているファイルに関する追加データを提供する要求の本文内のプロパティと、アップロード操作のセマンティクスをカスタマイズするを指定できます。</span><span class="sxs-lookup"><span data-stu-id="94435-129">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="94435-130">などの`item`プロパティは、次のパラメーターを設定することができます。<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span><span class="sxs-lookup"><span data-stu-id="94435-130">For example, the `item` property allows setting the following parameters: <!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span></span>
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

<span data-ttu-id="94435-131">次の使用例が動作を制御するは、ファイル名は既に使用され、場合も、明示的な終了の要求が行われるまでは、最終的なファイルを作成できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-131">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="94435-132">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94435-132">Optional request headers</span></span>

| <span data-ttu-id="94435-133">名前</span><span class="sxs-lookup"><span data-stu-id="94435-133">Name</span></span>       | <span data-ttu-id="94435-134">値</span><span class="sxs-lookup"><span data-stu-id="94435-134">Value</span></span> | <span data-ttu-id="94435-135">説明</span><span class="sxs-lookup"><span data-stu-id="94435-135">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="94435-136">*if-match*</span><span class="sxs-lookup"><span data-stu-id="94435-136">*if-match*</span></span> | <span data-ttu-id="94435-137">etag</span><span class="sxs-lookup"><span data-stu-id="94435-137">etag</span></span>  | <span data-ttu-id="94435-138">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がアイテムの現在の etag に一致しない場合には、`412 Precondition Failed` エラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="94435-138">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="94435-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="94435-139">Parameters</span></span>

| <span data-ttu-id="94435-140">パラメーター</span><span class="sxs-lookup"><span data-stu-id="94435-140">Parameter</span></span>            | <span data-ttu-id="94435-141">型</span><span class="sxs-lookup"><span data-stu-id="94435-141">Type</span></span>                          | <span data-ttu-id="94435-142">説明</span><span class="sxs-lookup"><span data-stu-id="94435-142">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="94435-143">item</span><span class="sxs-lookup"><span data-stu-id="94435-143">item</span></span>                 | <span data-ttu-id="94435-144">driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="94435-144">driveItemUploadableProperties</span></span> | <span data-ttu-id="94435-145">アップロードされているファイルに関するデータ</span><span class="sxs-lookup"><span data-stu-id="94435-145">Data about the file being uploaded</span></span>
| <span data-ttu-id="94435-146">deferCommit</span><span class="sxs-lookup"><span data-stu-id="94435-146">deferCommit</span></span>          | <span data-ttu-id="94435-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="94435-147">Boolean</span></span>                       | <span data-ttu-id="94435-148">場合はコピー先のファイルの場合は true、最終の作成に設定するには、明示的な要求が必要となります。</span><span class="sxs-lookup"><span data-stu-id="94435-148">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="94435-149">ビジネスの OneDrive でのみ。</span><span class="sxs-lookup"><span data-stu-id="94435-149">Only on OneDrive for Business.</span></span>

## <a name="item-properties"></a><span data-ttu-id="94435-150">アイテムのプロパティ</span><span class="sxs-lookup"><span data-stu-id="94435-150">Item properties</span></span>

| <span data-ttu-id="94435-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94435-151">Property</span></span>             | <span data-ttu-id="94435-152">型</span><span class="sxs-lookup"><span data-stu-id="94435-152">Type</span></span>               | <span data-ttu-id="94435-153">説明</span><span class="sxs-lookup"><span data-stu-id="94435-153">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="94435-154">説明</span><span class="sxs-lookup"><span data-stu-id="94435-154">description</span></span>          | <span data-ttu-id="94435-155">String</span><span class="sxs-lookup"><span data-stu-id="94435-155">String</span></span>             | <span data-ttu-id="94435-156">ユーザーに表示されている項目の説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="94435-156">Provides a user-visible description of the item.</span></span> <span data-ttu-id="94435-157">読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="94435-157">Read-write.</span></span> <span data-ttu-id="94435-158">上でのみ OneDrive 個人。</span><span class="sxs-lookup"><span data-stu-id="94435-158">Only on OneDrive Personal.</span></span>
| <span data-ttu-id="94435-159">名前</span><span class="sxs-lookup"><span data-stu-id="94435-159">name</span></span>                 | <span data-ttu-id="94435-160">String</span><span class="sxs-lookup"><span data-stu-id="94435-160">String</span></span>             | <span data-ttu-id="94435-p108">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="94435-p108">The name of the item (filename and extension). Read-write.</span></span>

### <a name="request"></a><span data-ttu-id="94435-163">要求</span><span class="sxs-lookup"><span data-stu-id="94435-163">Request</span></span>

<span data-ttu-id="94435-164">この要求への応答により、新たに作成された [uploadSession](../resources/uploadsession.md) の詳細 (ファイルの各部分をアップロードするために使用される URL など) が指定されます。</span><span class="sxs-lookup"><span data-stu-id="94435-164">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

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

### <a name="response"></a><span data-ttu-id="94435-165">応答</span><span class="sxs-lookup"><span data-stu-id="94435-165">Response</span></span>

<span data-ttu-id="94435-166">成功した場合、この要求への応答では残りの要求を送信する場所に関する詳細が [UploadSession](../resources/uploadsession.md) リソースとして提示されます。</span><span class="sxs-lookup"><span data-stu-id="94435-166">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="94435-167">このリソースは、ファイルのバイト範囲をどこにアップロードするか、およびアップロード セッションがいつ期限切れになるかに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="94435-167">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

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

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="94435-168">アップロード セッションにバイトをアップロードする</span><span class="sxs-lookup"><span data-stu-id="94435-168">Upload bytes to the upload session</span></span>

<span data-ttu-id="94435-169">ファイル、またはファイルの一部をアップロードするために、アプリは **createUploadSession** 応答で受け取った **uploadUrl** 値への PUT 要求を出します。</span><span class="sxs-lookup"><span data-stu-id="94435-169">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="94435-170">どの要求の最大バイト数も 60 MiB 未満である限り、ファイル全体をアップロードすることも、ファイルをいくつかのバイト範囲に分割することも可能です。</span><span class="sxs-lookup"><span data-stu-id="94435-170">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="94435-171">ファイルのフラグメントは、順に順番にアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-171">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="94435-172">誤った順序でアップロードすると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="94435-172">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="94435-173">**注:** アプリがファイルを複数のバイト範囲に分割する場合、各バイト範囲のサイズは 320 KiB (327,680 バイト) の倍数である**必要があります**。</span><span class="sxs-lookup"><span data-stu-id="94435-173">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="94435-174">320 KiB で均等に分割できないフラグメント サイズを使用した場合、一部のファイルのコミット中にエラーになります。</span><span class="sxs-lookup"><span data-stu-id="94435-174">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="94435-175">例</span><span class="sxs-lookup"><span data-stu-id="94435-175">Example</span></span>

<span data-ttu-id="94435-176">この例では、128 バイトのファイルのうち、最初の 26 バイトをアプリがアップロードします。</span><span class="sxs-lookup"><span data-stu-id="94435-176">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="94435-177">**Content-Length** ヘッダーは、現在の要求のサイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="94435-177">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="94435-178">**Content-Range** ヘッダーは、ファイル全体の中でこの要求が表すバイト範囲を示します。</span><span class="sxs-lookup"><span data-stu-id="94435-178">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="94435-179">ファイルの最初のフラグメントをアップロードする前に、ファイルの長さの合計がわかっています。</span><span class="sxs-lookup"><span data-stu-id="94435-179">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="94435-180">**重要:** アプリは、**Content-Range** ヘッダーで指定されるファイル サイズ合計をすべての要求で同じに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-180">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="94435-181">異なるファイル サイズのバイト範囲が宣言された場合、要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="94435-181">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="94435-182">応答</span><span class="sxs-lookup"><span data-stu-id="94435-182">Response</span></span>

<span data-ttu-id="94435-183">要求の完了時に、アップロードする必要のあるバイト範囲がまだ存在している場合、サーバーは `202 Accepted` で応答します。</span><span class="sxs-lookup"><span data-stu-id="94435-183">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="94435-184">アプリは **nextExpectedRanges** の値を使用して、次のバイト範囲の開始点を判断できます。</span><span class="sxs-lookup"><span data-stu-id="94435-184">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="94435-185">サーバーがまだ受信していないファイル部分を示す、複数の範囲指定が表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94435-185">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="94435-186">これは、中断された転送を再開する必要があり、クライアント側にとってサービスの状態が不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="94435-186">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="94435-187">常に以下のベスト プラクティスに従って、バイト範囲のサイズを決定してください。</span><span class="sxs-lookup"><span data-stu-id="94435-187">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="94435-188">アップロードするバイト範囲の正しいサイズの範囲を **nextExpectedRanges** が返すことを想定しないでください。</span><span class="sxs-lookup"><span data-stu-id="94435-188">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="94435-189">**nextExpectedRanges** プロパティは、まだ受信されていないファイルの範囲を示します。アプリによるファイル アップロード方法のパターンを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="94435-189">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="94435-190">備考</span><span class="sxs-lookup"><span data-stu-id="94435-190">Remarks</span></span>

* <span data-ttu-id="94435-191">`nextExpectedRanges` プロパティは、欠落してするすべての範囲の一覧を必ずしも示すわけではありません。</span><span class="sxs-lookup"><span data-stu-id="94435-191">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="94435-p115">フラグメントの書き込みが成功すると、次の開始点の範囲が返されます (例: "523-")。</span><span class="sxs-lookup"><span data-stu-id="94435-p115">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="94435-p116">サーバーが既に受信していたフラグメントをクライアントが送信した場合のエラーでは、サーバーから `HTTP 416 Requested Range Not Satisfiable` の応答が返されます。受信されていない範囲のより詳細なリストを取得するために、[アップロード ステータスを要求](#resuming-an-in-progress-upload)できます。</span><span class="sxs-lookup"><span data-stu-id="94435-p116">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="94435-p117">`PUT` の呼び出しを発行するときに、承認ヘッダーを含めると、`HTTP 401 Unauthorized` 応答が発生する可能性があります。承認ヘッダーとベアラー トークンは、最初の手順で `POST` を発行するときにのみ送信する必要があります。`PUT` を発行する場合は、含めないようにします。</span><span class="sxs-lookup"><span data-stu-id="94435-p117">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="94435-199">ファイルの完成</span><span class="sxs-lookup"><span data-stu-id="94435-199">Completing a file</span></span>

<span data-ttu-id="94435-200">場合`deferCommit`は false または設定を解除すると、ファイルの最後のバイトの範囲はアップロード URL に配置すると、アップロードが自動的に入力し、します。</span><span class="sxs-lookup"><span data-stu-id="94435-200">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>
<span data-ttu-id="94435-201">場合`deferCommit`が true の場合、アップロードをアップロードする最終的な POST 要求を明示的に完了する必要がありますアップロード URL をファイルの最後のバイトの範囲を配置すると後、に長さ 0 のコンテンツの url。</span><span class="sxs-lookup"><span data-stu-id="94435-201">If `deferCommit` is true, then after the final byte range of the file is PUT to the upload URL, the upload should be explicitly completed by a final POST request to the upload url with zero-length content.</span></span>

<span data-ttu-id="94435-202">アップロードが完了したら、サーバー要求に応答、最後に、`HTTP 201 Created`または`HTTP 200 OK`。</span><span class="sxs-lookup"><span data-stu-id="94435-202">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="94435-203">また、応答本文には、完成したファイルを表す **driveItem** の既定のプロパティ セットも含まれます。</span><span class="sxs-lookup"><span data-stu-id="94435-203">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

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

## <a name="handling-upload-conflicts"></a><span data-ttu-id="94435-204">アップロード競合の処理</span><span class="sxs-lookup"><span data-stu-id="94435-204">Handling upload conflicts</span></span>

<span data-ttu-id="94435-205">ファイルのアップロード後に競合が発生した場合 (たとえば、アップロード セッション中に同じ名前のアイテムが作成された場合) には、最後のバイト範囲がアップロードされたときにエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="94435-205">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

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

## <a name="cancel-the-upload-session"></a><span data-ttu-id="94435-206">アップロード セッションを取り消す</span><span class="sxs-lookup"><span data-stu-id="94435-206">Cancel the upload session</span></span>

<span data-ttu-id="94435-p120">アップロード セッションを取り消すには、アップロード URL に DELETE 要求を送信します。これにより、以前にアップロードしたデータを格納している一時ファイルがクリーンアップされます。これは、たとえばユーザーが転送を取り消した場合など、アップロードが中断される場合に使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-p120">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="94435-210">一時ファイルとそれに伴うアップロード セッションは、**expirationDateTime** が経過した後、自動的にクリーンアップされます。</span><span class="sxs-lookup"><span data-stu-id="94435-210">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="94435-211">期限が経過しても、一時ファイルはただちに削除されるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="94435-211">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="94435-212">要求</span><span class="sxs-lookup"><span data-stu-id="94435-212">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="94435-213">応答</span><span class="sxs-lookup"><span data-stu-id="94435-213">Response</span></span>

<span data-ttu-id="94435-214">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="94435-214">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="94435-215">進行中のアップロードを再開する</span><span class="sxs-lookup"><span data-stu-id="94435-215">Resuming an in-progress upload</span></span>

<span data-ttu-id="94435-p122">あるアップロード要求が完了する前に、要求が切断されるか失敗すると、その要求のすべてのバイトが無視されます。これは、アプリとサービス間の接続が切断された場合に発生することがあります。このような場合、アプリは直前に完了したフラグメントからファイル転送を再開できます。</span><span class="sxs-lookup"><span data-stu-id="94435-p122">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="94435-219">以前受信されたバイト範囲を知るために、アプリはアップロード セッションのステータスを要求できます。</span><span class="sxs-lookup"><span data-stu-id="94435-219">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="94435-220">例</span><span class="sxs-lookup"><span data-stu-id="94435-220">Example</span></span>

<span data-ttu-id="94435-221">`uploadUrl` に GET 要求を送信して、アップロードのステータスを照会します。</span><span class="sxs-lookup"><span data-stu-id="94435-221">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="94435-222">サーバーは応答で、アップロードが必要な、送信されなかったバイトの範囲のリストと、アップロード セッションの有効期限を返します。</span><span class="sxs-lookup"><span data-stu-id="94435-222">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="94435-223">残りのデータをアップロードする</span><span class="sxs-lookup"><span data-stu-id="94435-223">Upload remaining data</span></span>

<span data-ttu-id="94435-224">アプリにアップロードの開始点がわかると、[「アップロード セッションにバイトをアップロードする」](#upload-bytes-to-the-upload-session)の次の手順でアップロードを再開します。</span><span class="sxs-lookup"><span data-stu-id="94435-224">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="94435-225">アップロード エラーの処理</span><span class="sxs-lookup"><span data-stu-id="94435-225">Handle upload errors</span></span>

<span data-ttu-id="94435-226">ファイルの最後のバイト範囲がアップロードされるときに、エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="94435-226">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="94435-227">この原因として、名前の競合またはクォータ制限の超過が考えられます。</span><span class="sxs-lookup"><span data-stu-id="94435-227">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="94435-228">アップロード セッションは有効期限が切れるまで保持されるので、アプリはアップロード セッションを明示的にコミットすることで、アップロードを回復することができます。</span><span class="sxs-lookup"><span data-stu-id="94435-228">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="94435-229">アプリでアップロード セッションを明示的にコミットするには、アップロード セッションのコミット時に使用される新しい **driveItem** リソースを使って PUT 要求を出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-229">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="94435-230">この新しい要求により、元のアップロード エラーの原因となったエラーが修正されるはずです。</span><span class="sxs-lookup"><span data-stu-id="94435-230">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="94435-231">既存のアップロード セッションをアプリでコミットすることを示すために、アップロード セッション URL の値を指定する `@microsoft.graph.sourceUrl` プロパティを PUT 要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-231">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

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

<span data-ttu-id="94435-232">**注:** この呼び出しでは、想定どおりに `@microsoft.graph.conflictBehavior` ヘッダーと `if-match` ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="94435-232">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="http-response"></a><span data-ttu-id="94435-233">HTTP 応答</span><span class="sxs-lookup"><span data-stu-id="94435-233">HTTP response</span></span>

<span data-ttu-id="94435-234">新しいメタデータを使用してファイルをコミットできる場合は、`HTTP 201 Created` または `HTTP 200 OK` の応答が、アップロードしたファイルのアイテム メタデータとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="94435-234">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

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

## <a name="best-practices"></a><span data-ttu-id="94435-235">ベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="94435-235">Best practices</span></span>

* <span data-ttu-id="94435-236">接続の中断や 5xx エラーにより失敗したアップロードは、次のように再開または再試行します。</span><span class="sxs-lookup"><span data-stu-id="94435-236">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="94435-237">アップロード要求を再開または再試行するときに 5xx サーバー エラーが返された場合には、指数近似バックオフを使用します。</span><span class="sxs-lookup"><span data-stu-id="94435-237">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="94435-238">その他のエラーの場合は指数近似バックオフは使わず、再試行回数を制限する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94435-238">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="94435-239">再開可能なアップロードの実行中に発生した `404 Not Found` エラーに対処するには、アップロード全体を最初からやり直します。</span><span class="sxs-lookup"><span data-stu-id="94435-239">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="94435-240">これは、アップロード セッションがもはや存在しなくなったことを示します。</span><span class="sxs-lookup"><span data-stu-id="94435-240">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="94435-241">10 MiB (10,485,760 バイト) を超えるサイズのファイルには、再開可能なファイル転送を使用します。</span><span class="sxs-lookup"><span data-stu-id="94435-241">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="94435-242">安定した高速接続で最適なバイト範囲サイズは 10 MiB です。</span><span class="sxs-lookup"><span data-stu-id="94435-242">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="94435-243">より低速な、または信頼性の低い接続では、フラグメント サイズをより小さくした方が良い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="94435-243">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="94435-244">推奨されるフラグメント サイズは、5～10 MiB です。</span><span class="sxs-lookup"><span data-stu-id="94435-244">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="94435-245">320 KiB (327,680 バイト) の倍数のバイト範囲サイズを使用してください。</span><span class="sxs-lookup"><span data-stu-id="94435-245">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="94435-246">320 KiB の倍数ではないフラグメント サイズを使用した場合、最後のバイト範囲をアップロードした後に、サイズの大きなファイルの転送が失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="94435-246">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="94435-247">エラー応答</span><span class="sxs-lookup"><span data-stu-id="94435-247">Error responses</span></span>

<span data-ttu-id="94435-248">エラーがどのように返されるかについては、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="94435-248">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation"
} -->
