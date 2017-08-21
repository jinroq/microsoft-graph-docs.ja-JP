# <a name="message-replyall"></a><span data-ttu-id="09e3c-101">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="09e3c-101">message: replyAll</span></span>

<span data-ttu-id="09e3c-p101">メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="09e3c-p101">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09e3c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="09e3c-104">Prerequisites</span></span>
<span data-ttu-id="09e3c-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="09e3c-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="09e3c-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09e3c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="09e3c-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09e3c-107">Request headers</span></span>
| <span data-ttu-id="09e3c-108">名前</span><span class="sxs-lookup"><span data-stu-id="09e3c-108">Name</span></span>       | <span data-ttu-id="09e3c-109">型</span><span class="sxs-lookup"><span data-stu-id="09e3c-109">Type</span></span> | <span data-ttu-id="09e3c-110">説明</span><span class="sxs-lookup"><span data-stu-id="09e3c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09e3c-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e3c-111">Authorization</span></span>  | <span data-ttu-id="09e3c-112">string</span><span class="sxs-lookup"><span data-stu-id="09e3c-112">string</span></span>  | <span data-ttu-id="09e3c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09e3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09e3c-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09e3c-115">Content-Type</span></span> | <span data-ttu-id="09e3c-116">string</span><span class="sxs-lookup"><span data-stu-id="09e3c-116">string</span></span>  | <span data-ttu-id="09e3c-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="09e3c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09e3c-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="09e3c-119">Request body</span></span>
<span data-ttu-id="09e3c-120">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="09e3c-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09e3c-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="09e3c-121">Parameter</span></span>    | <span data-ttu-id="09e3c-122">型</span><span class="sxs-lookup"><span data-stu-id="09e3c-122">Type</span></span>   |<span data-ttu-id="09e3c-123">説明</span><span class="sxs-lookup"><span data-stu-id="09e3c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09e3c-124">comment</span><span class="sxs-lookup"><span data-stu-id="09e3c-124">comment</span></span>|<span data-ttu-id="09e3c-125">String</span><span class="sxs-lookup"><span data-stu-id="09e3c-125">String</span></span>|<span data-ttu-id="09e3c-p104">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="09e3c-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="09e3c-128">応答</span><span class="sxs-lookup"><span data-stu-id="09e3c-128">Response</span></span>

<span data-ttu-id="09e3c-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="09e3c-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e3c-131">例</span><span class="sxs-lookup"><span data-stu-id="09e3c-131">Example</span></span>
<span data-ttu-id="09e3c-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="09e3c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09e3c-133">要求</span><span class="sxs-lookup"><span data-stu-id="09e3c-133">Request</span></span>
<span data-ttu-id="09e3c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09e3c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="09e3c-135">応答</span><span class="sxs-lookup"><span data-stu-id="09e3c-135">Response</span></span>
<span data-ttu-id="09e3c-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="09e3c-136">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
