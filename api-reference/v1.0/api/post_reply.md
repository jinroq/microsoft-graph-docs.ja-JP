# <a name="post-reply"></a><span data-ttu-id="df93d-101">投稿: 返信</span><span class="sxs-lookup"><span data-stu-id="df93d-101">post: reply</span></span>

<span data-ttu-id="df93d-p101">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="df93d-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df93d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="df93d-104">Prerequisites</span></span>
<span data-ttu-id="df93d-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="df93d-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="df93d-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="df93d-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="df93d-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df93d-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="df93d-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df93d-108">Request headers</span></span>
| <span data-ttu-id="df93d-109">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df93d-109">Header</span></span>       | <span data-ttu-id="df93d-110">値</span><span class="sxs-lookup"><span data-stu-id="df93d-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df93d-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="df93d-111">Authorization</span></span>  | <span data-ttu-id="df93d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="df93d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df93d-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="df93d-114">Request body</span></span>
<span data-ttu-id="df93d-115">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="df93d-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="df93d-116">パラメーター</span><span class="sxs-lookup"><span data-stu-id="df93d-116">Parameter</span></span>    | <span data-ttu-id="df93d-117">型</span><span class="sxs-lookup"><span data-stu-id="df93d-117">Type</span></span>   |<span data-ttu-id="df93d-118">説明</span><span class="sxs-lookup"><span data-stu-id="df93d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df93d-119">post</span><span class="sxs-lookup"><span data-stu-id="df93d-119">post</span></span>|[<span data-ttu-id="df93d-120">post</span><span class="sxs-lookup"><span data-stu-id="df93d-120">post</span></span>](../resources/post.md)|<span data-ttu-id="df93d-121">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="df93d-121">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="df93d-122">応答</span><span class="sxs-lookup"><span data-stu-id="df93d-122">Response</span></span>

<span data-ttu-id="df93d-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="df93d-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df93d-125">例</span><span class="sxs-lookup"><span data-stu-id="df93d-125">Example</span></span>
<span data-ttu-id="df93d-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="df93d-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="df93d-127">要求</span><span class="sxs-lookup"><span data-stu-id="df93d-127">Request</span></span>
<span data-ttu-id="df93d-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df93d-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="df93d-129">応答</span><span class="sxs-lookup"><span data-stu-id="df93d-129">Response</span></span>
##### <a name="response"></a><span data-ttu-id="df93d-130">応答</span><span class="sxs-lookup"><span data-stu-id="df93d-130">Response</span></span>
<span data-ttu-id="df93d-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="df93d-131">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
