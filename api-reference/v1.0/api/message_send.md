# <a name="message-send"></a><span data-ttu-id="ac9f4-101">メッセージ: send</span><span class="sxs-lookup"><span data-stu-id="ac9f4-101">message: send</span></span>

<span data-ttu-id="ac9f4-p101">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac9f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac9f4-105">Permissions</span></span>
<span data-ttu-id="ac9f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac9f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac9f4-108">Permission type</span></span>      | <span data-ttu-id="ac9f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac9f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac9f4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac9f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac9f4-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ac9f4-111">Mail.Send</span></span>    |
|<span data-ttu-id="ac9f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac9f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac9f4-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ac9f4-113">Mail.Send</span></span>    |
|<span data-ttu-id="ac9f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac9f4-114">Application</span></span> | <span data-ttu-id="ac9f4-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ac9f4-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac9f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac9f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="ac9f4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac9f4-117">Request headers</span></span>
| <span data-ttu-id="ac9f4-118">名前</span><span class="sxs-lookup"><span data-stu-id="ac9f4-118">Name</span></span>       | <span data-ttu-id="ac9f4-119">型</span><span class="sxs-lookup"><span data-stu-id="ac9f4-119">Type</span></span> | <span data-ttu-id="ac9f4-120">説明</span><span class="sxs-lookup"><span data-stu-id="ac9f4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac9f4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac9f4-121">Authorization</span></span>  | <span data-ttu-id="ac9f4-122">string</span><span class="sxs-lookup"><span data-stu-id="ac9f4-122">string</span></span>  | <span data-ttu-id="ac9f4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac9f4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac9f4-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ac9f4-126">応答</span><span class="sxs-lookup"><span data-stu-id="ac9f4-126">Response</span></span>

<span data-ttu-id="ac9f4-p104">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac9f4-129">例</span><span class="sxs-lookup"><span data-stu-id="ac9f4-129">Example</span></span>
<span data-ttu-id="ac9f4-130">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ac9f4-131">要求</span><span class="sxs-lookup"><span data-stu-id="ac9f4-131">Request</span></span>
<span data-ttu-id="ac9f4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="ac9f4-133">応答</span><span class="sxs-lookup"><span data-stu-id="ac9f4-133">Response</span></span>

<span data-ttu-id="ac9f4-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ac9f4-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
