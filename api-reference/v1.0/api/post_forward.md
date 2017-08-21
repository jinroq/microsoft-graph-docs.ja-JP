# <a name="post-forward"></a><span data-ttu-id="d4e83-101">投稿: 転送</span><span class="sxs-lookup"><span data-stu-id="d4e83-101">post: forward</span></span>

<span data-ttu-id="d4e83-p101">受信者に投稿を転送します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="d4e83-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="d4e83-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4e83-104">Prerequisites</span></span>
<span data-ttu-id="d4e83-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4e83-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="d4e83-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="d4e83-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="d4e83-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4e83-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="d4e83-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4e83-108">Request headers</span></span>
| <span data-ttu-id="d4e83-109">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4e83-109">Header</span></span>       | <span data-ttu-id="d4e83-110">値</span><span class="sxs-lookup"><span data-stu-id="d4e83-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4e83-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e83-111">Authorization</span></span>  | <span data-ttu-id="d4e83-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4e83-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4e83-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4e83-114">Request body</span></span>
<span data-ttu-id="d4e83-115">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4e83-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4e83-116">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4e83-116">Parameter</span></span>    | <span data-ttu-id="d4e83-117">型</span><span class="sxs-lookup"><span data-stu-id="d4e83-117">Type</span></span>   |<span data-ttu-id="d4e83-118">説明</span><span class="sxs-lookup"><span data-stu-id="d4e83-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4e83-119">comment</span><span class="sxs-lookup"><span data-stu-id="d4e83-119">comment</span></span>|<span data-ttu-id="d4e83-120">String</span><span class="sxs-lookup"><span data-stu-id="d4e83-120">String</span></span>|<span data-ttu-id="d4e83-121">投稿と共に転送されるオプションのコメント。</span><span class="sxs-lookup"><span data-stu-id="d4e83-121">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="d4e83-122">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d4e83-122">toRecipients</span></span>|<span data-ttu-id="d4e83-123">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="d4e83-123">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="d4e83-124">スレッドの転送先となる受信者。</span><span class="sxs-lookup"><span data-stu-id="d4e83-124">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="d4e83-125">応答</span><span class="sxs-lookup"><span data-stu-id="d4e83-125">Response</span></span>

<span data-ttu-id="d4e83-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d4e83-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e83-128">例</span><span class="sxs-lookup"><span data-stu-id="d4e83-128">Example</span></span>
<span data-ttu-id="d4e83-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d4e83-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4e83-130">要求</span><span class="sxs-lookup"><span data-stu-id="d4e83-130">Request</span></span>
<span data-ttu-id="d4e83-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4e83-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="d4e83-132">応答</span><span class="sxs-lookup"><span data-stu-id="d4e83-132">Response</span></span>
<span data-ttu-id="d4e83-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d4e83-133">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
