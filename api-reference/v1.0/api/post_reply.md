# <a name="post-reply"></a><span data-ttu-id="f01a7-101">投稿: 返信</span><span class="sxs-lookup"><span data-stu-id="f01a7-101">post: reply</span></span>

<span data-ttu-id="f01a7-p101">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="f01a7-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f01a7-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f01a7-104">Permissions</span></span>
<span data-ttu-id="f01a7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f01a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f01a7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f01a7-107">Permission type</span></span>      | <span data-ttu-id="f01a7-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f01a7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f01a7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f01a7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f01a7-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f01a7-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f01a7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f01a7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f01a7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f01a7-112">Not supported.</span></span>    |
|<span data-ttu-id="f01a7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f01a7-113">Application</span></span> | <span data-ttu-id="f01a7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f01a7-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f01a7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f01a7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="f01a7-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f01a7-116">Request headers</span></span>
| <span data-ttu-id="f01a7-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f01a7-117">Header</span></span>       | <span data-ttu-id="f01a7-118">値</span><span class="sxs-lookup"><span data-stu-id="f01a7-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f01a7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f01a7-119">Authorization</span></span>  | <span data-ttu-id="f01a7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f01a7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f01a7-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="f01a7-122">Request body</span></span>
<span data-ttu-id="f01a7-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f01a7-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f01a7-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f01a7-124">Parameter</span></span>    | <span data-ttu-id="f01a7-125">型</span><span class="sxs-lookup"><span data-stu-id="f01a7-125">Type</span></span>   |<span data-ttu-id="f01a7-126">説明</span><span class="sxs-lookup"><span data-stu-id="f01a7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f01a7-127">post</span><span class="sxs-lookup"><span data-stu-id="f01a7-127">post</span></span>|[<span data-ttu-id="f01a7-128">post</span><span class="sxs-lookup"><span data-stu-id="f01a7-128">post</span></span>](../resources/post.md)|<span data-ttu-id="f01a7-129">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="f01a7-129">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="f01a7-130">応答</span><span class="sxs-lookup"><span data-stu-id="f01a7-130">Response</span></span>

<span data-ttu-id="f01a7-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f01a7-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f01a7-133">例</span><span class="sxs-lookup"><span data-stu-id="f01a7-133">Example</span></span>
<span data-ttu-id="f01a7-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f01a7-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f01a7-135">要求</span><span class="sxs-lookup"><span data-stu-id="f01a7-135">Request</span></span>
<span data-ttu-id="f01a7-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f01a7-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f01a7-137">応答</span><span class="sxs-lookup"><span data-stu-id="f01a7-137">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f01a7-138">応答</span><span class="sxs-lookup"><span data-stu-id="f01a7-138">Response</span></span>
<span data-ttu-id="f01a7-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f01a7-139">Here is an example of the response.</span></span>
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
