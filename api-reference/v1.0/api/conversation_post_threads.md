# <a name="create-thread"></a><span data-ttu-id="94bab-101">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="94bab-101">Create thread</span></span>

<span data-ttu-id="94bab-102">指定した会話に新しいスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="94bab-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="94bab-p101">指定したとおりにスレッドと投稿を作成します。[スレッドに返信](conversationthread_reply.md) を使用して、そのスレッドへの投稿を続けます。また、投稿 ID を取得している場合は、そのスレッドのその投稿にも[返信](post_reply.md)できます。</span><span class="sxs-lookup"><span data-stu-id="94bab-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="94bab-106">注:[最初にスレッドを作成して、新しい会話を開始](group_post_threads.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="94bab-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94bab-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94bab-107">Permissions</span></span>
<span data-ttu-id="94bab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94bab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94bab-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94bab-110">Permission type</span></span>      | <span data-ttu-id="94bab-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94bab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94bab-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94bab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94bab-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94bab-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="94bab-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94bab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94bab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94bab-115">Not supported.</span></span>    |
|<span data-ttu-id="94bab-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94bab-116">Application</span></span> | <span data-ttu-id="94bab-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94bab-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94bab-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94bab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="94bab-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94bab-119">Request headers</span></span>
| <span data-ttu-id="94bab-120">名前</span><span class="sxs-lookup"><span data-stu-id="94bab-120">Name</span></span>       | <span data-ttu-id="94bab-121">型</span><span class="sxs-lookup"><span data-stu-id="94bab-121">Type</span></span> | <span data-ttu-id="94bab-122">説明</span><span class="sxs-lookup"><span data-stu-id="94bab-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94bab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94bab-123">Authorization</span></span>  | <span data-ttu-id="94bab-124">string</span><span class="sxs-lookup"><span data-stu-id="94bab-124">string</span></span>  | <span data-ttu-id="94bab-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94bab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94bab-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="94bab-127">Request body</span></span>
<span data-ttu-id="94bab-128">要求の本文に、[ConversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94bab-128">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94bab-129">応答</span><span class="sxs-lookup"><span data-stu-id="94bab-129">Response</span></span>

<span data-ttu-id="94bab-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94bab-130">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94bab-131">例</span><span class="sxs-lookup"><span data-stu-id="94bab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94bab-132">要求</span><span class="sxs-lookup"><span data-stu-id="94bab-132">Request</span></span>
<span data-ttu-id="94bab-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94bab-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="94bab-134">要求の本文に、[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94bab-134">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="94bab-135">応答</span><span class="sxs-lookup"><span data-stu-id="94bab-135">Response</span></span>

<span data-ttu-id="94bab-p104">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新しいスレッドの `id` を返します。以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="94bab-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
