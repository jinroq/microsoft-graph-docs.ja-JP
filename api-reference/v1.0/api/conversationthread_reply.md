# <a name="conversationthread-reply"></a><span data-ttu-id="c4a31-101">conversationThread: 返信</span><span class="sxs-lookup"><span data-stu-id="c4a31-101">conversationThread: reply</span></span>

<span data-ttu-id="c4a31-p101">グループ会話のスレッドに返信して、新しい投稿を追加します。要求内で親の会話を指定したり、親の会話なしにスレッドだけを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="c4a31-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4a31-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="c4a31-104">Prerequisites</span></span>
<span data-ttu-id="c4a31-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c4a31-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="c4a31-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4a31-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="c4a31-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4a31-107">Request headers</span></span>
| <span data-ttu-id="c4a31-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4a31-108">Header</span></span>       | <span data-ttu-id="c4a31-109">値</span><span class="sxs-lookup"><span data-stu-id="c4a31-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4a31-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4a31-110">Authorization</span></span>  | <span data-ttu-id="c4a31-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4a31-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4a31-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4a31-113">Content-Type</span></span>  | <span data-ttu-id="c4a31-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c4a31-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4a31-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4a31-116">Request body</span></span>
<span data-ttu-id="c4a31-117">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c4a31-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4a31-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c4a31-118">Parameter</span></span>    | <span data-ttu-id="c4a31-119">型</span><span class="sxs-lookup"><span data-stu-id="c4a31-119">Type</span></span>   |<span data-ttu-id="c4a31-120">説明</span><span class="sxs-lookup"><span data-stu-id="c4a31-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4a31-121">post</span><span class="sxs-lookup"><span data-stu-id="c4a31-121">post</span></span>|[<span data-ttu-id="c4a31-122">post</span><span class="sxs-lookup"><span data-stu-id="c4a31-122">post</span></span>](../resources/post.md)|<span data-ttu-id="c4a31-123">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="c4a31-123">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="c4a31-124">応答</span><span class="sxs-lookup"><span data-stu-id="c4a31-124">Response</span></span>

<span data-ttu-id="c4a31-p104">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c4a31-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a31-127">例</span><span class="sxs-lookup"><span data-stu-id="c4a31-127">Example</span></span>
<span data-ttu-id="c4a31-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c4a31-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4a31-129">要求</span><span class="sxs-lookup"><span data-stu-id="c4a31-129">Request</span></span>
<span data-ttu-id="c4a31-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4a31-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="c4a31-131">応答</span><span class="sxs-lookup"><span data-stu-id="c4a31-131">Response</span></span>
<span data-ttu-id="c4a31-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c4a31-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
