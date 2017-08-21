# <a name="message-reply"></a><span data-ttu-id="2751a-101">メッセージ: reply</span><span class="sxs-lookup"><span data-stu-id="2751a-101">message: reply</span></span>

<span data-ttu-id="2751a-p101">メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="2751a-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2751a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2751a-104">Prerequisites</span></span>
<span data-ttu-id="2751a-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="2751a-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="2751a-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2751a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="2751a-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2751a-107">Request headers</span></span>
| <span data-ttu-id="2751a-108">名前</span><span class="sxs-lookup"><span data-stu-id="2751a-108">Name</span></span>       | <span data-ttu-id="2751a-109">型</span><span class="sxs-lookup"><span data-stu-id="2751a-109">Type</span></span> | <span data-ttu-id="2751a-110">説明</span><span class="sxs-lookup"><span data-stu-id="2751a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2751a-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="2751a-111">Authorization</span></span>  | <span data-ttu-id="2751a-112">string</span><span class="sxs-lookup"><span data-stu-id="2751a-112">string</span></span>  | <span data-ttu-id="2751a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2751a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2751a-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2751a-115">Content-Type</span></span> | <span data-ttu-id="2751a-116">string</span><span class="sxs-lookup"><span data-stu-id="2751a-116">string</span></span>  | <span data-ttu-id="2751a-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="2751a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2751a-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="2751a-119">Request body</span></span>
<span data-ttu-id="2751a-120">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2751a-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2751a-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2751a-121">Parameter</span></span>    | <span data-ttu-id="2751a-122">型</span><span class="sxs-lookup"><span data-stu-id="2751a-122">Type</span></span>   |<span data-ttu-id="2751a-123">説明</span><span class="sxs-lookup"><span data-stu-id="2751a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2751a-124">comment</span><span class="sxs-lookup"><span data-stu-id="2751a-124">comment</span></span>|<span data-ttu-id="2751a-125">String</span><span class="sxs-lookup"><span data-stu-id="2751a-125">String</span></span>|<span data-ttu-id="2751a-p104">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2751a-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="2751a-128">応答</span><span class="sxs-lookup"><span data-stu-id="2751a-128">Response</span></span>

<span data-ttu-id="2751a-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2751a-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2751a-131">例</span><span class="sxs-lookup"><span data-stu-id="2751a-131">Example</span></span>
<span data-ttu-id="2751a-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2751a-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2751a-133">要求</span><span class="sxs-lookup"><span data-stu-id="2751a-133">Request</span></span>
<span data-ttu-id="2751a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2751a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="2751a-135">応答</span><span class="sxs-lookup"><span data-stu-id="2751a-135">Response</span></span>
##### <a name="response"></a><span data-ttu-id="2751a-136">応答</span><span class="sxs-lookup"><span data-stu-id="2751a-136">Response</span></span>
<span data-ttu-id="2751a-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2751a-137">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
