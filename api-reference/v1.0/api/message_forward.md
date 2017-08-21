# <a name="message-forward"></a><span data-ttu-id="62866-101">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="62866-101">message: forward</span></span>

<span data-ttu-id="62866-p101">メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="62866-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62866-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="62866-104">Prerequisites</span></span>
<span data-ttu-id="62866-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="62866-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="62866-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62866-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="62866-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62866-107">Request headers</span></span>
| <span data-ttu-id="62866-108">名前</span><span class="sxs-lookup"><span data-stu-id="62866-108">Name</span></span>       | <span data-ttu-id="62866-109">型</span><span class="sxs-lookup"><span data-stu-id="62866-109">Type</span></span> | <span data-ttu-id="62866-110">説明</span><span class="sxs-lookup"><span data-stu-id="62866-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62866-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="62866-111">Authorization</span></span>  | <span data-ttu-id="62866-112">string</span><span class="sxs-lookup"><span data-stu-id="62866-112">string</span></span>  | <span data-ttu-id="62866-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="62866-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62866-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62866-115">Content-Type</span></span> | <span data-ttu-id="62866-116">string</span><span class="sxs-lookup"><span data-stu-id="62866-116">string</span></span>  | <span data-ttu-id="62866-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="62866-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62866-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="62866-119">Request body</span></span>
<span data-ttu-id="62866-120">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="62866-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62866-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="62866-121">Parameter</span></span>    | <span data-ttu-id="62866-122">型</span><span class="sxs-lookup"><span data-stu-id="62866-122">Type</span></span>   |<span data-ttu-id="62866-123">説明</span><span class="sxs-lookup"><span data-stu-id="62866-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62866-124">comment</span><span class="sxs-lookup"><span data-stu-id="62866-124">comment</span></span>|<span data-ttu-id="62866-125">String</span><span class="sxs-lookup"><span data-stu-id="62866-125">String</span></span>|<span data-ttu-id="62866-p104">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="62866-p104">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="62866-128">toRecipients</span><span class="sxs-lookup"><span data-stu-id="62866-128">toRecipients</span></span>|<span data-ttu-id="62866-129">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="62866-129">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="62866-130">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="62866-130">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="62866-131">応答</span><span class="sxs-lookup"><span data-stu-id="62866-131">Response</span></span>

<span data-ttu-id="62866-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="62866-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62866-134">例</span><span class="sxs-lookup"><span data-stu-id="62866-134">Example</span></span>
<span data-ttu-id="62866-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="62866-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="62866-136">要求</span><span class="sxs-lookup"><span data-stu-id="62866-136">Request</span></span>
<span data-ttu-id="62866-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62866-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="62866-138">応答</span><span class="sxs-lookup"><span data-stu-id="62866-138">Response</span></span>
##### <a name="response"></a><span data-ttu-id="62866-139">応答</span><span class="sxs-lookup"><span data-stu-id="62866-139">Response</span></span>
<span data-ttu-id="62866-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="62866-140">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
