# <a name="create-thread"></a><span data-ttu-id="a4aeb-101">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="a4aeb-101">Create thread</span></span>

<span data-ttu-id="a4aeb-102">指定した会話に新しいスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="a4aeb-p101">指定したとおりにスレッドと投稿を作成します。[スレッドに返信](conversationthread_reply.md) を使用して、そのスレッドへの投稿を続けます。また、投稿 ID を取得している場合は、そのスレッドのその投稿にも[返信](post_reply.md)できます。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="a4aeb-106">メモ:[最初にスレッドを作成して、新しい会話を開始](group_post_threads.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4aeb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4aeb-107">Prerequisites</span></span>
<span data-ttu-id="a4aeb-108">この API を実行するために必要な**スコープ**は、次のとおりです。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="a4aeb-108">The following **scopes** are required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="a4aeb-109">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4aeb-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="a4aeb-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4aeb-110">Request headers</span></span>
| <span data-ttu-id="a4aeb-111">名前</span><span class="sxs-lookup"><span data-stu-id="a4aeb-111">Name</span></span>       | <span data-ttu-id="a4aeb-112">型</span><span class="sxs-lookup"><span data-stu-id="a4aeb-112">Type</span></span> | <span data-ttu-id="a4aeb-113">説明</span><span class="sxs-lookup"><span data-stu-id="a4aeb-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a4aeb-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4aeb-114">Authorization</span></span>  | <span data-ttu-id="a4aeb-115">string</span><span class="sxs-lookup"><span data-stu-id="a4aeb-115">string</span></span>  | <span data-ttu-id="a4aeb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4aeb-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4aeb-118">Request body</span></span>
<span data-ttu-id="a4aeb-119">要求の本文に、[ConversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-119">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a4aeb-120">応答</span><span class="sxs-lookup"><span data-stu-id="a4aeb-120">Response</span></span>

<span data-ttu-id="a4aeb-121">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-121">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4aeb-122">例</span><span class="sxs-lookup"><span data-stu-id="a4aeb-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4aeb-123">要求</span><span class="sxs-lookup"><span data-stu-id="a4aeb-123">Request</span></span>
<span data-ttu-id="a4aeb-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="a4aeb-125">要求の本文に、[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-125">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a4aeb-126">応答</span><span class="sxs-lookup"><span data-stu-id="a4aeb-126">Response</span></span>

<span data-ttu-id="a4aeb-p103">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で新しいスレッドの `id` を返します。以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a4aeb-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
