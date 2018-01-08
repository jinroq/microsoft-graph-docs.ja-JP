# <a name="create-conversation-thread"></a><span data-ttu-id="71845-101">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="71845-101">Create conversation thread</span></span>
<span data-ttu-id="71845-102">最初にスレッドを作成して、新しいグループ会話を開始します。</span><span class="sxs-lookup"><span data-stu-id="71845-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="71845-p101">グループには、新しい会話、会話スレッド、および投稿が作成されます。[スレッドに返信](conversationthread_reply.md) または [投稿に返信](post_reply.md) を使い、そのスレッドへの投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="71845-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="71845-105">注:[既存の会話内に新しいスレッドを開始する](conversation_post_threads.md) こともできます。</span><span class="sxs-lookup"><span data-stu-id="71845-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="71845-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71845-106">Permissions</span></span>
<span data-ttu-id="71845-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71845-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71845-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71845-109">Permission type</span></span>      | <span data-ttu-id="71845-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71845-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71845-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71845-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71845-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71845-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="71845-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71845-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71845-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71845-114">Not supported.</span></span>    |
|<span data-ttu-id="71845-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71845-115">Application</span></span> | <span data-ttu-id="71845-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71845-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71845-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71845-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="71845-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71845-118">Request headers</span></span>
| <span data-ttu-id="71845-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71845-119">Header</span></span>       | <span data-ttu-id="71845-120">値</span><span class="sxs-lookup"><span data-stu-id="71845-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71845-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71845-121">Authorization</span></span>  | <span data-ttu-id="71845-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71845-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71845-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71845-124">Content-Type</span></span>  | <span data-ttu-id="71845-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71845-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71845-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71845-126">Request body</span></span>
<span data-ttu-id="71845-127">要求の本文に、[投稿](../resources/post.md) を含む[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="71845-127">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="71845-128">応答</span><span class="sxs-lookup"><span data-stu-id="71845-128">Response</span></span>
<span data-ttu-id="71845-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71845-129">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71845-130">例</span><span class="sxs-lookup"><span data-stu-id="71845-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="71845-131">要求</span><span class="sxs-lookup"><span data-stu-id="71845-131">Request</span></span>
<span data-ttu-id="71845-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71845-132">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
#### <a name="response"></a><span data-ttu-id="71845-133">応答</span><span class="sxs-lookup"><span data-stu-id="71845-133">Response</span></span>
<span data-ttu-id="71845-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71845-134">The following is an example of a response.</span></span>
><span data-ttu-id="71845-135">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="71845-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="71845-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="71845-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
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
