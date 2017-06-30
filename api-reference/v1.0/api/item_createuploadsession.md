# <a name="upload-large-files-with-an-upload-session"></a>アップロード セッションを使ってサイズの大きなファイルをアップロードする

アプリで最大ファイル サイズまでファイルをアップロードできるようにするには、アップロード セッションを作成します。アップロード セッションにより、アプリは一連の API 要求で広範なファイルをアップロードでき、このため、アップロードの進行中に接続が切れた場合に転送を再開できます。

アップロード セッションを使ってファイルをアップロードするには、次の 2 つの手順を行います。

1. [アップロード セッションを作成する](#create-an-upload-session)
2. [アップロード セッションにバイトをアップロードする](#upload-bytes-to-the-upload-session)

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All

> **注**:この API では、Files.ReadWrite.All のアプリケーション アクセス許可は、まだサポートされていません。近日中のフルサポートが予定されています。 

## <a name="create-an-upload-session"></a>アップロード セッションを作成する

サイズが大きいファイルのアップロードを開始するには、アプリがまず新しいアップロード セッションを要求する必要があります。これにより、完全なファイルがアップロードされるまでファイルのバイトが保存される、一時的な保存場所が作成されます。ファイルの最後のバイトがアップロードされると、アップロード セッションは完了し、最終的なファイルがアップロード先のフォルダーに表示されます。

### <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a>要求本文
要求の本文は必要ありません。ただし、アップロードされているファイルに関する追加データを提供する要求本文を指定できます。

たとえば、ファイル名が既に取得されている場合の動作を制御するために、要求本文で競合動作のプロパティを指定できます。

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前       | 値 | 説明                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | この要求ヘッダーが含まれていて、指定された eTag (または cTag) がアイテムの現在の etag に一致しない場合には、`412 Precondition Failed` エラー応答が返されます。 |


### <a name="response"></a>応答
この要求への応答により、新たに作成された [uploadSession](../resources/uploadsession.md) の詳細 (ファイルの各部分をアップロードするために使用される URL など) が指定されます。 

### <a name="example"></a>例

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

### <a name="response"></a>応答
以下は、応答の例です。

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

## <a name="upload-bytes-to-the-upload-session"></a>アップロード セッションにバイトをアップロードする

ファイル、またはファイルの一部をアップロードするために、アプリは **createUploadSession** 応答で受け取った **uploadUrl** の値に PUT 要求を行います。すべての要求の最大バイト数が 60 MiB 未満である限り、ファイル全体をアップロードすることも、ファイルをいくつかに分割することも可能です。分割されたファイルのフラグメントは順番にアップロードする必要があります。誤った順序でアップロードすると、エラーが発生します。

**注:**アプリがファイルを複数に分割する場合、各フラグメントは、各フラグメントのサイズは 320 KiB の倍数である**必要があります**。使用するフラグメントのサイズが 320 によって均等に分割されていない場合、一部のファイルのコミット中にエラーになります。

### <a name="example"></a>例

次の例では、128 バイトのファイルのうち、最初の 26 バイトをアップロードしています。**Content-Length** ヘッダーは、現在の要求のサイズを指定します。**Content-Range** ヘッダーは、この要求が表すファイル全体の中のバイトの範囲を示します。ファイルの長さの合計は、ファイルの最初のフラグメントをアップロードする前にわかっている必要があります。

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**重要:****Content-Range** ヘッダーで指定されたファイル サイズの合計は、すべての要求で同じである必要があります。異なるファイル サイズのフラグメントがあった場合、要求は失敗します。

### <a name="response"></a>応答
<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

アプリは **nextExpectedRanges** の値を使用して、次のフラグメント開始点を決定できます。サーバーがまだ受信していないファイルの部分を示す、複数の指定範囲が表示されることがあります。これは、中断された転送を再開する必要があり、クライアント側でサービスの状態が不明な場合に便利です。

常に以下のベスト プラクティスに従って、フラグメント サイズを決定する必要があります。**nextExpectedRanges** がアップロード フラグメントの正しいサイズの範囲を返すと想定しないでください。**extExpectedRanges** プロパティは、まだ受信されていないファイルの範囲を示すもので、ファイルのアップロード方法のパターンを示すものではありません。

**メモ:**

* `nextExpectedRanges` プロパティはアップロードされていない範囲すべての一覧を必ず示すわけではありません。
* フラグメントの書き込みが成功すると、次の開始点の範囲が返されます (例: "523-")。
* サーバーが既に受信していたフラグメントをクライアントが送信した場合のエラーでは、サーバーから `HTTP 416 Requested Range Not Satisfiable` の応答が返されます。受信されていない範囲のより詳細なリストを取得するために、[アップロード ステータスを要求](#resuming-an-in-progress-upload)できます。
* `PUT` の呼び出しを発行するときに、承認ヘッダーを含めると、`HTTP 401 Unauthoized` 応答が発生する可能性があります。承認ヘッダーとベアラー トークンは、最初の手順で `POST` を発行するときにのみ送信する必要があります。`PUT` を発行する場合は、含めないようにします。   


## <a name="completing-a-file"></a>ファイルの完成

ファイルの最後のフラグメントが受信されると、サーバーは `HTTP 201 Created` または `HTTP 200 OK` の応答を返します。応答本文には完全なファイルを表す **driveItem** の既定のプロパティ セットも含まれます。

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
**注:**説明をわかりやすくするために、アイテムの応答は一部省略されています。

## <a name="cancel-an-upload-session"></a>アップロード セッションを取り消す

アップロード セッションを取り消すには、アップロード URL に DELETE 要求を送信します。これにより、以前にアップロードしたデータを格納している一時ファイルがクリーンアップされます。これは、たとえばユーザーが転送を取り消した場合など、アップロードが中断される場合に使用する必要があります。

一時ファイルとそれに伴うアップロード セッションは、**expirationDateTime** が経過した後、自動的にクリーンアップされます。

### <a name="example"></a>例

DELETE 要求は即時にアップロード セッションを終了し、それ以前にアップロードされたすべてのデータを削除します。

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

### <a name="response"></a>応答

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>進行中のアップロードを再開する

あるアップロード要求が完了する前に、要求が切断されるか失敗すると、その要求のすべてのバイトが無視されます。これは、アプリとサービス間の接続が切断された場合に発生することがあります。このような場合、アプリは直前に完了したフラグメントからファイル転送を再開できます。

以前受信されたバイト範囲を知るために、アプリはアップロード セッションのステータスを要求できます。

### <a name="example"></a>例
`uploadUrl` に GET 要求を送信して、アップロードのステータスを照会します。

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

サーバーは応答で、アップロードが必要な、送信されなかったバイトの範囲のリストと、アップロード セッションの有効期限を返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>残りのデータをアップロードする
アプリにアップロードの開始点がわかると、[「アップロード セッションにバイトをアップロードする」](#upload-bytes-to-the-upload-session)の次の手順でアップロードを再開します。


## <a name="best-practices"></a>ベスト プラクティス

* 接続の中断や 5xx エラーにより失敗したアップロードは、次のように再開または再試行します。
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* アップロード要求を再開または再試行するときに 5xx サーバー エラーが返された場合には、指数近似バックオフを使用します。
* その他のエラーの場合は指数近似バックオフは使わず、再試行回数を制限する必要があります。
* 再開可能なアップロードを実行中の `404 Not Found` エラーは、アップロード全体を最初からやり直して処理します。
* 10 MiB (10 \* 1024 \* 1024 バイト) を超えるサイズのファイルには、再開可能なファイル転送を使用します。
* 安定した高速接続では 10 MiB が最適のフラグメント サイズです。より低速な、または信頼性の低い接続では、フラグメント サイズをより小さくした方が良い結果を得られます。推奨されるフラグメント サイズは、5-10 MiB です。
* 320 KiB の倍数のフラグメント サイズを使用してください (320 \* 1024 バイト)。320 KiB の倍数ではないフラグメント サイズを使用した場合、最後のフラグメントをアップロードした後にサイズの大きなファイルの転送が失敗する可能性があります。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
