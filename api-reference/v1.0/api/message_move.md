# <a name="message-move"></a><span data-ttu-id="b13bf-101">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="b13bf-101">message: move</span></span>

<span data-ttu-id="b13bf-p101">メッセージをフォルダーに移動します。これにより、宛先フォルダーにメッセージの新しいコピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="b13bf-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b13bf-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b13bf-104">Prerequisites</span></span>
<span data-ttu-id="b13bf-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="b13bf-105">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="b13bf-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b13bf-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="b13bf-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b13bf-107">Request headers</span></span>
| <span data-ttu-id="b13bf-108">名前</span><span class="sxs-lookup"><span data-stu-id="b13bf-108">Name</span></span>       | <span data-ttu-id="b13bf-109">型</span><span class="sxs-lookup"><span data-stu-id="b13bf-109">Type</span></span> | <span data-ttu-id="b13bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="b13bf-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b13bf-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="b13bf-111">Authorization</span></span>  | <span data-ttu-id="b13bf-112">string</span><span class="sxs-lookup"><span data-stu-id="b13bf-112">string</span></span>  | <span data-ttu-id="b13bf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b13bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b13bf-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b13bf-115">Content-Type</span></span> | <span data-ttu-id="b13bf-116">string</span><span class="sxs-lookup"><span data-stu-id="b13bf-116">string</span></span>  | <span data-ttu-id="b13bf-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="b13bf-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b13bf-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="b13bf-119">Request body</span></span>
<span data-ttu-id="b13bf-120">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b13bf-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b13bf-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b13bf-121">Parameter</span></span>    | <span data-ttu-id="b13bf-122">型</span><span class="sxs-lookup"><span data-stu-id="b13bf-122">Type</span></span>   |<span data-ttu-id="b13bf-123">説明</span><span class="sxs-lookup"><span data-stu-id="b13bf-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b13bf-124">DestinationId</span><span class="sxs-lookup"><span data-stu-id="b13bf-124">DestinationId</span></span>|<span data-ttu-id="b13bf-125">String</span><span class="sxs-lookup"><span data-stu-id="b13bf-125">String</span></span>|<span data-ttu-id="b13bf-126">宛先フォルダーの ID、あるいは `Inbox`、`Drafts`、`SentItems` または `DeletedItems` の既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="b13bf-126">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="b13bf-127">応答</span><span class="sxs-lookup"><span data-stu-id="b13bf-127">Response</span></span>

<span data-ttu-id="b13bf-128">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b13bf-128">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b13bf-129">例</span><span class="sxs-lookup"><span data-stu-id="b13bf-129">Example</span></span>
<span data-ttu-id="b13bf-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b13bf-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b13bf-131">要求</span><span class="sxs-lookup"><span data-stu-id="b13bf-131">Request</span></span>
<span data-ttu-id="b13bf-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b13bf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/move
Content-type: application/json
Content-length: 44

{
  "DestinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="b13bf-133">応答</span><span class="sxs-lookup"><span data-stu-id="b13bf-133">Response</span></span>
<span data-ttu-id="b13bf-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b13bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
