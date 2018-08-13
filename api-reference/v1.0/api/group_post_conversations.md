# <a name="create-conversation"></a><span data-ttu-id="a7bba-101">会話を作成する</span><span class="sxs-lookup"><span data-stu-id="a7bba-101">Create conversation</span></span>
<span data-ttu-id="a7bba-102">スレッドと投稿を含めて、新しい[会話](../resources/conversation.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="a7bba-102">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="a7bba-103">[スレッドに返信](conversationthread_reply.md)または[投稿に返信](post_reply.md)を使い、その会話への投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="a7bba-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7bba-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7bba-104">Permissions</span></span>
<span data-ttu-id="a7bba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7bba-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7bba-107">Permission type</span></span>      | <span data-ttu-id="a7bba-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7bba-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7bba-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7bba-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a7bba-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7bba-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7bba-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7bba-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7bba-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7bba-112">Not supported.</span></span>    |
|<span data-ttu-id="a7bba-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7bba-113">Application</span></span> | <span data-ttu-id="a7bba-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7bba-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7bba-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7bba-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="a7bba-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7bba-116">Request headers</span></span>
| <span data-ttu-id="a7bba-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7bba-117">Header</span></span>       | <span data-ttu-id="a7bba-118">値</span><span class="sxs-lookup"><span data-stu-id="a7bba-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7bba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7bba-119">Authorization</span></span>  | <span data-ttu-id="a7bba-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7bba-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7bba-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7bba-122">Content-Type</span></span>  | <span data-ttu-id="a7bba-123">application/json</span><span class="sxs-lookup"><span data-stu-id="a7bba-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7bba-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7bba-124">Request body</span></span>
<span data-ttu-id="a7bba-125">要求の本文に、[conversationThread](../resources/conversationThread.md) と [投稿](../resources/post.md) を含む [会話](../resources/conversation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7bba-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="a7bba-126">応答</span><span class="sxs-lookup"><span data-stu-id="a7bba-126">Response</span></span>
<span data-ttu-id="a7bba-127">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[会話](../resources/conversation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a7bba-127">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="a7bba-128">応答には、新しい会話とスレッドの ID が含まれます。これらの ID は、[投稿の一覧表示](conversationthread_list_posts.md)の操作時の新しい投稿の取得に使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="a7bba-128">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread_list_posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="a7bba-129">例</span><span class="sxs-lookup"><span data-stu-id="a7bba-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a7bba-130">要求</span><span class="sxs-lookup"><span data-stu-id="a7bba-130">Request</span></span>
<span data-ttu-id="a7bba-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7bba-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
Content-type: application/json

{
    "topic":"New locations for this quarter",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"What do we know so far?"
                    },
                    "newParticipants":[
                        {
                            "emailAddress":{
                                "name":"Adele Vance",
                                "address":"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="a7bba-132">応答</span><span class="sxs-lookup"><span data-stu-id="a7bba-132">Response</span></span>
<span data-ttu-id="a7bba-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7bba-133">The following is an example of the response.</span></span>
><span data-ttu-id="a7bba-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a7bba-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADDVKtMlRp4Txc6k=",
    "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
    "threads":[
        {
            "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->