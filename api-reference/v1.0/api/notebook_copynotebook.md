# <a name="notebook-copynotebook"></a><span data-ttu-id="3656d-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="3656d-101">notebook: copyNotebook</span></span>
<span data-ttu-id="3656d-p101">コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="3656d-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="3656d-104">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次いで結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="3656d-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3656d-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="3656d-105">Prerequisites</span></span>
<span data-ttu-id="3656d-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="3656d-106">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="3656d-107">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3656d-107">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="3656d-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3656d-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="3656d-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3656d-109">Request headers</span></span>
| <span data-ttu-id="3656d-110">名前</span><span class="sxs-lookup"><span data-stu-id="3656d-110">Name</span></span>       | <span data-ttu-id="3656d-111">型</span><span class="sxs-lookup"><span data-stu-id="3656d-111">Type</span></span> | <span data-ttu-id="3656d-112">説明</span><span class="sxs-lookup"><span data-stu-id="3656d-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3656d-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="3656d-113">Authorization</span></span>  | <span data-ttu-id="3656d-114">string</span><span class="sxs-lookup"><span data-stu-id="3656d-114">string</span></span>  | <span data-ttu-id="3656d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3656d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3656d-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3656d-117">Content-Type</span></span> | <span data-ttu-id="3656d-118">string</span><span class="sxs-lookup"><span data-stu-id="3656d-118">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3656d-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="3656d-119">Request body</span></span>
<span data-ttu-id="3656d-p103">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。パラメーターが必要ない場合は、空の要求本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="3656d-p103">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="3656d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3656d-122">Parameter</span></span>    | <span data-ttu-id="3656d-123">型</span><span class="sxs-lookup"><span data-stu-id="3656d-123">Type</span></span>   |<span data-ttu-id="3656d-124">説明</span><span class="sxs-lookup"><span data-stu-id="3656d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3656d-125">groupId</span><span class="sxs-lookup"><span data-stu-id="3656d-125">groupId</span></span>|<span data-ttu-id="3656d-126">String</span><span class="sxs-lookup"><span data-stu-id="3656d-126">String</span></span>|<span data-ttu-id="3656d-p104">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="3656d-p104">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="3656d-129">renameAs</span><span class="sxs-lookup"><span data-stu-id="3656d-129">renameAs</span></span>|<span data-ttu-id="3656d-130">String</span><span class="sxs-lookup"><span data-stu-id="3656d-130">String</span></span>|<span data-ttu-id="3656d-p105">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="3656d-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="3656d-133">応答</span><span class="sxs-lookup"><span data-stu-id="3656d-133">Response</span></span>

<span data-ttu-id="3656d-p106">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteOperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="3656d-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="3656d-136">例</span><span class="sxs-lookup"><span data-stu-id="3656d-136">Example</span></span>
<span data-ttu-id="3656d-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3656d-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3656d-138">要求</span><span class="sxs-lookup"><span data-stu-id="3656d-138">Request</span></span>
<span data-ttu-id="3656d-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3656d-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="3656d-140">応答</span><span class="sxs-lookup"><span data-stu-id="3656d-140">Response</span></span>
<span data-ttu-id="3656d-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3656d-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
