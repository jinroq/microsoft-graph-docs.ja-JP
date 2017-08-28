# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="5cdba-101">アップロード セッションを使ってサイズの大きなファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="5cdba-101">Upload large files with an upload session</span></span>

<span data-ttu-id="5cdba-p101">アプリで最大ファイル サイズまでファイルをアップロードできるようにするには、アップロード セッションを作成します。アップロード セッションにより、アプリは一連の API 要求で広範なファイルをアップロードでき、このため、アップロードの進行中に接続が切れた場合に転送を再開できます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequental API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="5cdba-104">アップロード セッションを使ってファイルをアップロードするには、次の 2 つの手順を行います。</span><span class="sxs-lookup"><span data-stu-id="5cdba-104">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="5cdba-105">アップロード セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="5cdba-105">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="5cdba-106">アップロード セッションにバイトをアップロードする</span><span class="sxs-lookup"><span data-stu-id="5cdba-106">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="prerequisites"></a><span data-ttu-id="5cdba-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5cdba-107">Prerequisites</span></span>
<span data-ttu-id="5cdba-108">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="5cdba-108">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="5cdba-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cdba-109">Files.ReadWrite</span></span>
* <span data-ttu-id="5cdba-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cdba-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="5cdba-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cdba-111">Sites.ReadWrite.All</span></span>

> <span data-ttu-id="5cdba-p102">**注**:この API では、Files.ReadWrite.All のアプリケーション アクセス許可は、まだサポートされていません。近日中のフルサポートが予定されています。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p102">**Note**: The Files.ReadWrite.All application permission is not yet supported on this API. Full support is planned soon.</span></span> 

## <a name="create-an-upload-session"></a><span data-ttu-id="5cdba-114">アップロード セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="5cdba-114">Create an upload session</span></span>

<span data-ttu-id="5cdba-p103">サイズが大きいファイルのアップロードを開始するには、アプリがまず新しいアップロード セッションを要求する必要があります。これにより、完全なファイルがアップロードされるまでファイルのバイトが保存される、一時的な保存場所が作成されます。ファイルの最後のバイトがアップロードされると、アップロード セッションは完了し、最終的なファイルがアップロード先のフォルダーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p103">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="5cdba-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5cdba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="5cdba-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="5cdba-119">Request body</span></span>
<span data-ttu-id="5cdba-p104">要求の本文は必要ありません。ただし、アップロードされているファイルに関する追加データを提供する要求本文を指定できます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p104">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="5cdba-122">たとえば、ファイル名が既に取得されている場合の動作を制御するために、要求本文で競合動作のプロパティを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-122">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="5cdba-123">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cdba-123">Optional request headers</span></span>

| <span data-ttu-id="5cdba-124">名前</span><span class="sxs-lookup"><span data-stu-id="5cdba-124">Name</span></span>       | <span data-ttu-id="5cdba-125">値</span><span class="sxs-lookup"><span data-stu-id="5cdba-125">Value</span></span> | <span data-ttu-id="5cdba-126">説明</span><span class="sxs-lookup"><span data-stu-id="5cdba-126">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5cdba-127">*if-match*</span><span class="sxs-lookup"><span data-stu-id="5cdba-127">*if-match*</span></span> | <span data-ttu-id="5cdba-128">etag</span><span class="sxs-lookup"><span data-stu-id="5cdba-128">etag</span></span>  | <span data-ttu-id="5cdba-129">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がアイテムの現在の etag に一致しない場合には、`412 Precondition Failed` エラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-129">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |


### <a name="response"></a><span data-ttu-id="5cdba-130">応答</span><span class="sxs-lookup"><span data-stu-id="5cdba-130">Response</span></span>
<span data-ttu-id="5cdba-131">この要求への応答により、新たに作成された [uploadSession](../resources/uploadsession.md) の詳細 (ファイルの各部分をアップロードするために使用される URL など) が指定されます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-131">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

### <a name="example"></a><span data-ttu-id="5cdba-132">例</span><span class="sxs-lookup"><span data-stu-id="5cdba-132">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a><span data-ttu-id="5cdba-133">応答</span><span class="sxs-lookup"><span data-stu-id="5cdba-133">Response</span></span> 

<span data-ttu-id="5cdba-134">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5cdba-134">The following example shows the response from the server with the search results.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://tenant-my.sharepoint.com/alkjl1kjklna",
  "expirationDateTime": "2020-08-24T10:58:00Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="5cdba-135">アップロード セッションにバイトをアップロードする</span><span class="sxs-lookup"><span data-stu-id="5cdba-135">Upload bytes to the upload session</span></span>

<span data-ttu-id="5cdba-p105">ファイル、またはファイルの一部をアップロードするために、アプリは **createUploadSession** 応答で受け取った **uploadUrl** の値に PUT 要求を行います。すべての要求の最大バイト数が 60 MiB 未満である限り、ファイル全体をアップロードすることも、ファイルをいくつかに分割することも可能です。分割されたファイルのフラグメントは順番にアップロードする必要があります。誤った順序でアップロードすると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p105">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response. You can upload the entire file, or split the file into fragments, as long as the maximum bytes in any given request is less than 60 MiB. The fragments of the file must be uploaded sequentally in order. Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="5cdba-p106">**注:**アプリがファイルを複数に分割する場合、各フラグメントは、各フラグメントのサイズは 320 KiB の倍数である**必要があります**。使用するフラグメントのサイズが 320 によって均等に分割されていない場合、一部のファイルのコミット中にエラーになります。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p106">**Note:** If your app splits a file into multiple fragments, the size of each fragment **MUST** be a multiple of 320 KiB. Using a fragment size that does not divide evenly by 320 will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="5cdba-142">例</span><span class="sxs-lookup"><span data-stu-id="5cdba-142">Example</span></span>

<span data-ttu-id="5cdba-p107">次の例では、128 バイトのファイルのうち、最初の 26 バイトをアップロードしています。**Content-Length** ヘッダーは、現在の要求のサイズを指定します。**Content-Range** ヘッダーは、この要求が表すファイル全体の中のバイトの範囲を示します。ファイルの長さの合計は、ファイルの最初のフラグメントをアップロードする前にわかっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p107">This example is uploading the first 26 bytes of a 128 byte file. The **Content-Length** header specifies the size of the current request. The **Content-Range** header indicates the range of bytes in the overall file that this request represents. The total length of the file must be known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="5cdba-p108">**重要:****Content-Range** ヘッダーで指定されたファイル サイズの合計は、すべての要求で同じである必要があります。異なるファイル サイズのフラグメントがあった場合、要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p108">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests. If a fragment declares a different file size, the request will fail.</span></span>

##### <a name="response"></a><span data-ttu-id="5cdba-149">応答</span><span class="sxs-lookup"><span data-stu-id="5cdba-149">Response</span></span>

<span data-ttu-id="5cdba-150">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5cdba-150">The following example shows the response from the server with the search results.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="5cdba-p109">アプリは **nextExpectedRanges** の値を使用して、次のフラグメント開始点を決定できます。サーバーがまだ受信していないファイルの部分を示す、複数の指定範囲が表示されることがあります。これは、中断された転送を再開する必要があり、クライアント側でサービスの状態が不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p109">Your app can use the **nextExpectedRanges** value to determine where to start the next fragment. You may see multiple ranges specified, indicating parts of the file that the server has not yet received. This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="5cdba-p110">常に以下のベスト プラクティスに従って、フラグメント サイズを決定する必要があります。**nextExpectedRanges** がアップロード フラグメントの正しいサイズの範囲を返すと想定しないでください。**extExpectedRanges** プロパティは、まだ受信されていないファイルの範囲を示すもので、ファイルのアップロード方法のパターンを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p110">You should always determine the fragment size according to the best practices below. Do not assume that **nextExpectedRanges** will return reanges of proper size for an upload fragment. The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how you should upload the file.</span></span>

<span data-ttu-id="5cdba-157">**メモ:**</span><span class="sxs-lookup"><span data-stu-id="5cdba-157">**Notes:**</span></span>

* <span data-ttu-id="5cdba-158">`nextExpectedRanges` プロパティはアップロードされていない範囲すべての一覧を必ず示すわけではありません。</span><span class="sxs-lookup"><span data-stu-id="5cdba-158">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="5cdba-p111">フラグメントの書き込みが成功すると、次の開始点の範囲が返されます (例: "523-")。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p111">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="5cdba-p112">サーバーが既に受信していたフラグメントをクライアントが送信した場合のエラーでは、サーバーから `HTTP 416 Requested Range Not Satisfiable` の応答が返されます。受信されていない範囲のより詳細なリストを取得するために、[アップロード ステータスを要求](#resuming-an-in-progress-upload)できます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p112">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="5cdba-p113">`PUT` の呼び出しを発行するときに、承認ヘッダーを含めると、`HTTP 401 Unauthorized` 応答が発生する可能性があります。承認ヘッダーとベアラー トークンは、最初の手順で `POST` を発行するときにのみ送信する必要があります。`PUT` を発行する場合は、含めないようにします。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p113">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authoization header and bearer token should only be sent when issueing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>   


## <a name="completing-a-file"></a><span data-ttu-id="5cdba-166">ファイルの完成</span><span class="sxs-lookup"><span data-stu-id="5cdba-166">Completing a file</span></span>

<span data-ttu-id="5cdba-p114">ファイルの最後のフラグメントが受信されると、サーバーは `HTTP 201 Created` または `HTTP 200 OK` の応答を返します。応答本文には完全なファイルを表す **driveItem** の既定のプロパティ セットも含まれます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p114">When the last fragment of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`. The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
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
<span data-ttu-id="5cdba-169">**注:**説明をわかりやすくするために、アイテムの応答は一部省略されています。</span><span class="sxs-lookup"><span data-stu-id="5cdba-169">**Note:** The item response is truncated for documentation clarity.</span></span>

## <a name="cancel-an-upload-session"></a><span data-ttu-id="5cdba-170">アップロード セッションを取り消す</span><span class="sxs-lookup"><span data-stu-id="5cdba-170">Cancel an upload session</span></span>

<span data-ttu-id="5cdba-p115">アップロード セッションを取り消すには、アップロード URL に DELETE 要求を送信します。これにより、以前にアップロードしたデータを格納している一時ファイルがクリーンアップされます。これは、たとえばユーザーが転送を取り消した場合など、アップロードが中断される場合に使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p115">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="5cdba-174">一時ファイルとそれに伴うアップロード セッションは、**expirationDateTime** が経過した後、自動的にクリーンアップされます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-174">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="example"></a><span data-ttu-id="5cdba-175">例</span><span class="sxs-lookup"><span data-stu-id="5cdba-175">Example</span></span>

<span data-ttu-id="5cdba-176">DELETE 要求は即時にアップロード セッションを終了し、それ以前にアップロードされたすべてのデータを削除します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-176">The DELETE request will immedately expire the upload session and remove any previously uploaded bytes.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a><span data-ttu-id="5cdba-177">応答</span><span class="sxs-lookup"><span data-stu-id="5cdba-177">Response</span></span> 

<span data-ttu-id="5cdba-178">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5cdba-178">The following example shows the response from the server with the search results.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="5cdba-179">進行中のアップロードを再開する</span><span class="sxs-lookup"><span data-stu-id="5cdba-179">Resuming an in-progress upload</span></span>

<span data-ttu-id="5cdba-p116">あるアップロード要求が完了する前に、要求が切断されるか失敗すると、その要求のすべてのバイトが無視されます。これは、アプリとサービス間の接続が切断された場合に発生することがあります。このような場合、アプリは直前に完了したフラグメントからファイル転送を再開できます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p116">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="5cdba-183">以前受信されたバイト範囲を知るために、アプリはアップロード セッションのステータスを要求できます。</span><span class="sxs-lookup"><span data-stu-id="5cdba-183">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="5cdba-184">例</span><span class="sxs-lookup"><span data-stu-id="5cdba-184">Example</span></span>
<span data-ttu-id="5cdba-185">`uploadUrl` に GET 要求を送信して、アップロードのステータスを照会します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-185">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

<span data-ttu-id="5cdba-186">サーバーは応答で、アップロードが必要な、送信されなかったバイトの範囲のリストと、アップロード セッションの有効期限を返します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-186">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="5cdba-187">残りのデータをアップロードする</span><span class="sxs-lookup"><span data-stu-id="5cdba-187">Upload remaining data</span></span>
<span data-ttu-id="5cdba-188">アプリにアップロードの開始点がわかると、[「アップロード セッションにバイトをアップロードする」](#upload-bytes-to-the-upload-session)の次の手順でアップロードを再開します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-188">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>


## <a name="best-practices"></a><span data-ttu-id="5cdba-189">ベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="5cdba-189">Best practices</span></span>

* <span data-ttu-id="5cdba-190">接続の中断や 5xx エラーにより失敗したアップロードは、次のように再開または再試行します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-190">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="5cdba-191">アップロード要求を再開または再試行するときに 5xx サーバー エラーが返された場合には、指数近似バックオフを使用します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-191">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="5cdba-192">その他のエラーの場合は指数近似バックオフは使わず、再試行回数を制限する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cdba-192">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="5cdba-193">再開可能なアップロードを実行中の `404 Not Found` エラーは、アップロード全体を最初からやり直して処理します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-193">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span>
* <span data-ttu-id="5cdba-194">10 MiB (10 \* 1024 \* 1024 バイト) を超えるサイズのファイルには、再開可能なファイル転送を使用します。</span><span class="sxs-lookup"><span data-stu-id="5cdba-194">Use resumable file transfers for files larger than 10 MiB (10 \* 1024 \* 1024 bytes).</span></span>
* <span data-ttu-id="5cdba-p117">安定した高速接続では 10 MiB が最適のフラグメント サイズです。より低速な、または信頼性の低い接続では、フラグメント サイズをより小さくした方が良い結果を得られます。推奨されるフラグメント サイズは、5-10 MiB です。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p117">A fragment size of 10 MiB for stable high speed connections is optimal. For slower or less reliable connections you may get better results from a smaller fragment size. The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="5cdba-p118">320 KiB の倍数のフラグメント サイズを使用してください (320 \* 1024 バイト)。320 KiB の倍数ではないフラグメント サイズを使用した場合、最後のフラグメントをアップロードした後にサイズの大きなファイルの転送が失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5cdba-p118">Use a fragment size that is a multiple of 320 KiB (320 \* 1024 bytes). Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last fragment is uploaded.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
