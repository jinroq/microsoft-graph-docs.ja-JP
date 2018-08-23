# <a name="message-send"></a><span data-ttu-id="0107d-101">メッセージ: send</span><span class="sxs-lookup"><span data-stu-id="0107d-101">message: send</span></span>

<span data-ttu-id="0107d-p101">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="0107d-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="0107d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0107d-105">Permissions</span></span>

<span data-ttu-id="0107d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0107d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0107d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0107d-108">Permission type</span></span>      | <span data-ttu-id="0107d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0107d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0107d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0107d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0107d-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0107d-111">Mail.Send</span></span>    |
|<span data-ttu-id="0107d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0107d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0107d-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0107d-113">Mail.Send</span></span>    |
|<span data-ttu-id="0107d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0107d-114">Application</span></span> | <span data-ttu-id="0107d-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0107d-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0107d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0107d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="0107d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0107d-117">Request headers</span></span>

| <span data-ttu-id="0107d-118">名前</span><span class="sxs-lookup"><span data-stu-id="0107d-118">Name</span></span>       | <span data-ttu-id="0107d-119">型</span><span class="sxs-lookup"><span data-stu-id="0107d-119">Type</span></span> | <span data-ttu-id="0107d-120">説明</span><span class="sxs-lookup"><span data-stu-id="0107d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0107d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0107d-121">Authorization</span></span>  | <span data-ttu-id="0107d-122">文字列</span><span class="sxs-lookup"><span data-stu-id="0107d-122">string</span></span>  | <span data-ttu-id="0107d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0107d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0107d-125">Content-Length</span><span class="sxs-lookup"><span data-stu-id="0107d-125">Content-Length</span></span> | <span data-ttu-id="0107d-126">数値</span><span class="sxs-lookup"><span data-stu-id="0107d-126">number</span></span> | <span data-ttu-id="0107d-127">0。必須。</span><span class="sxs-lookup"><span data-stu-id="0107d-127">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0107d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0107d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0107d-129">応答</span><span class="sxs-lookup"><span data-stu-id="0107d-129">Response</span></span>

<span data-ttu-id="0107d-p104">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0107d-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0107d-132">例</span><span class="sxs-lookup"><span data-stu-id="0107d-132">Example</span></span>

<span data-ttu-id="0107d-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0107d-133">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0107d-134">要求</span><span class="sxs-lookup"><span data-stu-id="0107d-134">Request</span></span>

<span data-ttu-id="0107d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0107d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="0107d-136">応答</span><span class="sxs-lookup"><span data-stu-id="0107d-136">Response</span></span>

<span data-ttu-id="0107d-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0107d-137">Here is an example of the response.</span></span>
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
