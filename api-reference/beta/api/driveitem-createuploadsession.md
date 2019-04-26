---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 再開可能なファイル アップロード
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3801be631ab64c6ab2cb25ce48b4e846f9d77287
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325337"
---
# <a name="upload-large-files-with-an-upload-session"></a>アップロード セッションを使ってサイズが大きいファイルをアップロードする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリで最大ファイル サイズまでファイルをアップロードできるようにするには、アップロード セッションを作成します。アップロード セッションにより、アプリは一連の API 要求で広範なファイルをアップロードでき、このため、アップロードの進行中に接続が切れた場合に転送を再開できます。

アップロード セッションを使ってファイルをアップロードするには、次の 2 つの手順を行います。

1. [アップロード セッションを作成する](#create-an-upload-session)
2. [アップロード セッションにバイトをアップロードする](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Sites.ReadWrite.All |

## <a name="create-an-upload-session"></a>アップロード セッションを作成する

サイズが大きいファイルのアップロードを開始するには、アプリがまず新しいアップロード セッションを要求する必要があります。
これにより、完全なファイルがアップロードされるまでファイルのバイトが保存される、一時的な保存場所が作成されます。
ファイルの最後のバイトがアップロードされると、アップロード セッションは完了し、最終的なファイルがアップロード先のフォルダーに表示されます。
または、要求の引数にプロパティを`deferCommit`設定することによって、アップロードの完了要求を明示的に行うまで、移行先でのファイルの最終的な作成を遅延させることができます。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a>要求本文

要求の本文は必要ありません。
ただし、要求本文でプロパティを指定して、アップロードされるファイルに関する追加データを提供したり、アップロード操作のセマンティクスをカスタマイズしたりすることができます。

たとえば、 `item`プロパティで次のパラメーターを設定できます。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } -->
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

次の例では、filename が既に取得されている場合の動作を制御し、明示的な完了要求が行われるまで最終的なファイルを作成しないように指定しています。

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前       | 値 | 説明                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | この要求ヘッダーが含まれていて、指定された eTag (または cTag) がアイテムの現在の etag に一致しない場合には、`412 Precondition Failed` エラー応答が返されます。 |

## <a name="parameters"></a>パラメーター

| パラメーター            | 型                          | 説明
|:---------------------|:------------------------------|:---------------------------------
| item                 | ドライブ itemuploadableproperties | アップロードされるファイルに関するデータ
| deferCommit          | Boolean                       | true に設定されている場合、コピー先でのファイルの最終作成では明示的な要求が必要になります。 OneDrive for business でのみ使用できます。

## <a name="item-properties"></a>アイテムのプロパティ

| プロパティ             | 型               | 説明
|:---------------------|:-------------------|:---------------------------------
| description          | String             | ユーザーに表示されるアイテムの説明を提供します。 読み取り/書き込み。 OneDrive Personal のみ
| name                 | String             | アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。

### <a name="request"></a>要求

この要求への応答により、新たに作成された [uploadSession](../resources/uploadsession.md) の詳細 (ファイルの各部分をアップロードするために使用される URL など) が指定されます。 

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

### <a name="response"></a>応答

成功した場合、この要求への応答では残りの要求を送信する場所に関する詳細が [UploadSession](../resources/uploadsession.md) リソースとして提示されます。

このリソースは、ファイルのバイト範囲をどこにアップロードするか、およびアップロード セッションがいつ期限切れになるかに関する詳細を提供します。

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

## <a name="upload-bytes-to-the-upload-session"></a>アップロード セッションにバイトをアップロードする

ファイル、またはファイルの一部をアップロードするために、アプリは **createUploadSession** 応答で受け取った **uploadUrl** の値に PUT 要求を行います。
どの要求の最大バイト数も 60 MiB 未満である限り、ファイル全体をアップロードすることも、ファイルをいくつかのバイト範囲に分割することも可能です。

分割されたファイルのフラグメントは順番にアップロードされる必要があります。
誤った順序でアップロードすると、エラーが発生します。

**注:** アプリがファイルを複数のバイト範囲に分割する場合、各バイト範囲のサイズは 320 KiB (327,680 バイト) の倍数である**必要があります**。 320 KiB で均等に分割できないフラグメント サイズを使用した場合、一部のファイルのコミット中にエラーになります。

### <a name="example"></a>例

この例では、128 バイトのファイルのうち、最初の 26 バイトをアプリがアップロードします。

* **Content-Length** ヘッダーは、現在の要求のサイズを指定します。
* **Content-Range** ヘッダーは、ファイル全体の中でこの要求が表すバイト範囲を示します。
* ファイルの最初のフラグメントをアップロードする前に、ファイルの長さの合計がわかっています。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**重要:****Content-Range** ヘッダーで指定されたファイル サイズの合計は、すべての要求で同じである必要があります。
異なるファイル サイズのバイト範囲が宣言された場合、要求は失敗します。

### <a name="response"></a>応答

要求の完了時に、アップロードする必要のあるバイト範囲がまだ存在している場合、サーバーは `202 Accepted` で応答します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

アプリは **nextExpectedRanges** の値を使用して、次のバイト範囲の開始点を判断できます。
サーバーがまだ受信していないファイルの部分を示す、複数の指定範囲が表示されることがあります。 これは、中断された転送を再開する必要があり、クライアント側でサービスの状態が不明な場合に便利です。

常に以下のベスト プラクティスに従って、バイト範囲のサイズを決定してください。 アップロードするバイト範囲の正しいサイズの範囲を **nextExpectedRanges** が返すことを想定しないでください。
**nextExpectedRanges** プロパティは、まだ受信されていないファイルの範囲を示します。アプリによるファイル アップロード方法のパターンを示すものではありません。

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

## <a name="remarks"></a>備考

* `nextExpectedRanges` プロパティは、欠落してするすべての範囲の一覧を必ずしも示すわけではありません。
* フラグメントの書き込みが成功すると、次の開始点の範囲が返されます (例: "523-")。
* サーバーが既に受信していたフラグメントをクライアントが送信した場合のエラーでは、サーバーから `HTTP 416 Requested Range Not Satisfiable` の応答が返されます。受信されていない範囲のより詳細なリストを取得するために、[アップロード ステータスを要求](#resuming-an-in-progress-upload)できます。
* `PUT` の呼び出しを発行するときに、承認ヘッダーを含めると、`HTTP 401 Unauthorized` 応答が発生する可能性があります。承認ヘッダーとベアラー トークンは、最初の手順で `POST` を発行するときにのみ送信する必要があります。`PUT` を発行する場合は、含めないようにします。

## <a name="completing-a-file"></a>ファイルの完成

が`deferCommit` false または unset の場合は、ファイルの最後のバイト範囲がアップロード URL に格納されると、アップロードが自動的に完了します。
が`deferCommit` true の場合は、ファイルの最後のバイト範囲がアップロード url に配置された後に、長さがゼロのコンテンツを含むアップロード url への最終 POST 要求によってアップロードが明示的に完了する必要があります。

アップロードが完了すると、サーバーは、 `HTTP 201 Created`または`HTTP 200 OK`の最後の要求に応答します。
応答本文には完全なファイルを表す **driveItem** の既定のプロパティ セットも含まれます。

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

## <a name="handling-upload-conflicts"></a>アップロード競合の処理

ファイルのアップロード後に競合が発生した場合 (たとえば、アップロード セッション中に同じ名前のアイテムが作成された場合) には、最後のバイト範囲がアップロードされたときにエラーが返されます。

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

## <a name="cancel-the-upload-session"></a>アップロード セッションを取り消す

アップロード セッションを取り消すには、アップロード URL に DELETE 要求を送信します。これにより、以前にアップロードしたデータを格納している一時ファイルがクリーンアップされます。これは、たとえばユーザーが転送を取り消した場合など、アップロードが中断される場合に使用する必要があります。

一時ファイルとそれに伴うアップロード セッションは、**expirationDateTime** が経過した後、自動的にクリーンアップされます。
期限が経過しても、一時ファイルはただちに削除されるとは限りません。

### <a name="request"></a>要求

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a>応答

次の例は応答を示しています。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>進行中のアップロードを再開する

あるアップロード要求が完了する前に、要求が切断されるか失敗すると、その要求のすべてのバイトが無視されます。これは、アプリとサービス間の接続が切断された場合に発生することがあります。このような場合、アプリは直前に完了したフラグメントからファイル転送を再開できます。

以前受信されたバイト範囲を知るために、アプリはアップロード セッションのステータスを要求できます。

### <a name="example"></a>例

`uploadUrl` に GET 要求を送信して、アップロードのステータスを照会します。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

サーバーは応答で、アップロードが必要な、送信されなかったバイトの範囲のリストと、アップロード セッションの有効期限を返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>残りのデータをアップロードする

アプリにアップロードの開始点がわかると、[「アップロード セッションにバイトをアップロードする」](#upload-bytes-to-the-upload-session)の次の手順でアップロードを再開します。

## <a name="handle-upload-errors"></a>アップロード エラーの処理

ファイルの最後のバイト範囲がアップロードされるときに、エラーが発生する可能性があります。 この原因として、名前の競合またはクォータ制限の超過が考えられます。
アップロード セッションは有効期限が切れるまで保持されるので、アプリはアップロード セッションを明示的にコミットすることで、アップロードを回復することができます。

アプリでアップロード セッションを明示的にコミットするには、アップロード セッションのコミット時に使用される新しい **driveItem** リソースを使って PUT 要求を送信する必要があります。
この新しい要求により、元のアップロード エラーの原因となったエラーが修正されるはずです。

既存のアップロード セッションをアプリでコミットすることを示すために、アップロード セッション URL の値を指定した `@microsoft.graph.sourceUrl` プロパティを PUT 要求に含める必要があります。

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

**注:** この呼び出しでは、期待どおりに `@microsoft.graph.conflictBehavior` と `if-match` ヘッダーを使用できます。

### <a name="response"></a>応答

新しいメタデータを使用してファイルをコミットできる場合は、`HTTP 201 Created` または `HTTP 200 OK` の応答が、アップロードしたファイルのアイテム メタデータとともに返されます。

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

## <a name="best-practices"></a>ベスト プラクティス

* 接続の中断や 5xx エラーにより失敗したアップロードは、次のように再開または再試行します。
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* アップロード要求を再開または再試行するときに 5xx サーバー エラーが返された場合には、指数近似バックオフを使用します。
* その他のエラーの場合は指数近似バックオフは使わず、再試行回数を制限する必要があります。
* 再開可能なアップロードを実行中の `404 Not Found` エラーは、アップロード全体を最初からやり直して処理します。 これは、アップロード セッションがもはや存在しなくなったことを示します。
* 10 MiB (10,485,760 バイト) を超えるサイズのファイルには、再開可能なファイル転送を使用します。
* 安定した高速接続で最適なバイト範囲サイズは 10 MiB です。 より低速な、または信頼性の低い接続では、フラグメント サイズをより小さくした方が良い結果を得られます。 推奨されるフラグメント サイズは、5 から 10 MiB です。
* 320 KiB (327,680 バイト) の倍数のバイト範囲サイズを使用してください。 320 KiB の倍数ではないフラグメント サイズを使用した場合、最後のバイト範囲をアップロードした後に、サイズの大きなファイルの転送が失敗する可能性があります。

## <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」のトピックを参照してください。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation",
  "suppressions": []
}
-->
