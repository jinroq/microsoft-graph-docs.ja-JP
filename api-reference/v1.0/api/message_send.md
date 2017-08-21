# <a name="message-send"></a><span data-ttu-id="0f11e-101">メッセージ: send</span><span class="sxs-lookup"><span data-stu-id="0f11e-101">message: send</span></span>

<span data-ttu-id="0f11e-p101">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="0f11e-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f11e-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f11e-105">Prerequisites</span></span>
<span data-ttu-id="0f11e-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="0f11e-106">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="0f11e-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f11e-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="0f11e-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f11e-108">Request headers</span></span>
| <span data-ttu-id="0f11e-109">名前</span><span class="sxs-lookup"><span data-stu-id="0f11e-109">Name</span></span>       | <span data-ttu-id="0f11e-110">型</span><span class="sxs-lookup"><span data-stu-id="0f11e-110">Type</span></span> | <span data-ttu-id="0f11e-111">説明</span><span class="sxs-lookup"><span data-stu-id="0f11e-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f11e-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f11e-112">Authorization</span></span>  | <span data-ttu-id="0f11e-113">string</span><span class="sxs-lookup"><span data-stu-id="0f11e-113">string</span></span>  | <span data-ttu-id="0f11e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0f11e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f11e-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f11e-116">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0f11e-117">応答</span><span class="sxs-lookup"><span data-stu-id="0f11e-117">Response</span></span>

<span data-ttu-id="0f11e-p103">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0f11e-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f11e-120">例</span><span class="sxs-lookup"><span data-stu-id="0f11e-120">Example</span></span>
<span data-ttu-id="0f11e-121">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0f11e-121">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0f11e-122">要求</span><span class="sxs-lookup"><span data-stu-id="0f11e-122">Request</span></span>
<span data-ttu-id="0f11e-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f11e-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="0f11e-124">応答</span><span class="sxs-lookup"><span data-stu-id="0f11e-124">Response</span></span>
##### <a name="response"></a><span data-ttu-id="0f11e-125">応答</span><span class="sxs-lookup"><span data-stu-id="0f11e-125">Response</span></span>
<span data-ttu-id="0f11e-126">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0f11e-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
