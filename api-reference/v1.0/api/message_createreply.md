# <a name="message-createreply"></a><span data-ttu-id="99237-101">メッセージ: createReply</span><span class="sxs-lookup"><span data-stu-id="99237-101">message: createReply</span></span>

<span data-ttu-id="99237-102">指定した[メッセージ](../resources/message.md)に対する返信の下書きを作成します。</span><span class="sxs-lookup"><span data-stu-id="99237-102">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="99237-103">下書きを[更新](../api/message_update.md)して**本文**に返信のコンテンツを追加したり、その他のメッセージのプロパティを変更したりすることも、下書きをそのまま[送信](../api/message_send.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="99237-103">You can then [update](../api/message_update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="99237-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99237-104">Permissions</span></span>
<span data-ttu-id="99237-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99237-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99237-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99237-107">Permission type</span></span>      | <span data-ttu-id="99237-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99237-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99237-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99237-109">Delegated (work or school account)</span></span> | <span data-ttu-id="99237-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99237-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="99237-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99237-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99237-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99237-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="99237-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99237-113">Application</span></span> | <span data-ttu-id="99237-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99237-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99237-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99237-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="99237-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99237-116">Request headers</span></span>
| <span data-ttu-id="99237-117">名前</span><span class="sxs-lookup"><span data-stu-id="99237-117">Name</span></span>       | <span data-ttu-id="99237-118">型</span><span class="sxs-lookup"><span data-stu-id="99237-118">Type</span></span> | <span data-ttu-id="99237-119">説明</span><span class="sxs-lookup"><span data-stu-id="99237-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99237-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="99237-120">Authorization</span></span>  | <span data-ttu-id="99237-121">string</span><span class="sxs-lookup"><span data-stu-id="99237-121">string</span></span>  | <span data-ttu-id="99237-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99237-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99237-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="99237-124">Request body</span></span>
<span data-ttu-id="99237-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="99237-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99237-126">応答</span><span class="sxs-lookup"><span data-stu-id="99237-126">Response</span></span>

<span data-ttu-id="99237-127">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="99237-127">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99237-128">例</span><span class="sxs-lookup"><span data-stu-id="99237-128">Example</span></span>
<span data-ttu-id="99237-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="99237-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99237-130">要求</span><span class="sxs-lookup"><span data-stu-id="99237-130">Request</span></span>
<span data-ttu-id="99237-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="99237-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```

##### <a name="response"></a><span data-ttu-id="99237-132">応答</span><span class="sxs-lookup"><span data-stu-id="99237-132">Response</span></span>
<span data-ttu-id="99237-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="99237-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
