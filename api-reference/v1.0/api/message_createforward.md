# <a name="message-createforward"></a><span data-ttu-id="bd421-101">メッセージ: createForward</span><span class="sxs-lookup"><span data-stu-id="bd421-101">message: createForward</span></span>

<span data-ttu-id="bd421-p101">転送メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。</span><span class="sxs-lookup"><span data-stu-id="bd421-p101">Create a draft of the Forward message. You can then [update](../api/message_update.md) or [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd421-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bd421-104">Permissions</span></span>
<span data-ttu-id="bd421-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd421-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd421-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd421-107">Permission type</span></span>      | <span data-ttu-id="bd421-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd421-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd421-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd421-109">Delegated (work or school account)</span></span> | <span data-ttu-id="bd421-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd421-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bd421-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd421-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd421-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd421-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bd421-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd421-113">Application</span></span> | <span data-ttu-id="bd421-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd421-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd421-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd421-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="bd421-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd421-116">Request headers</span></span>
| <span data-ttu-id="bd421-117">名前</span><span class="sxs-lookup"><span data-stu-id="bd421-117">Name</span></span>       | <span data-ttu-id="bd421-118">型</span><span class="sxs-lookup"><span data-stu-id="bd421-118">Type</span></span> | <span data-ttu-id="bd421-119">説明</span><span class="sxs-lookup"><span data-stu-id="bd421-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bd421-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd421-120">Authorization</span></span>  | <span data-ttu-id="bd421-121">string</span><span class="sxs-lookup"><span data-stu-id="bd421-121">string</span></span>  | <span data-ttu-id="bd421-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bd421-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd421-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd421-124">Content-Type</span></span> | <span data-ttu-id="bd421-125">string</span><span class="sxs-lookup"><span data-stu-id="bd421-125">string</span></span>  | <span data-ttu-id="bd421-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="bd421-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd421-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd421-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bd421-129">応答</span><span class="sxs-lookup"><span data-stu-id="bd421-129">Response</span></span>

<span data-ttu-id="bd421-130">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bd421-130">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd421-131">例</span><span class="sxs-lookup"><span data-stu-id="bd421-131">Example</span></span>
<span data-ttu-id="bd421-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bd421-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bd421-133">要求</span><span class="sxs-lookup"><span data-stu-id="bd421-133">Request</span></span>
<span data-ttu-id="bd421-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd421-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
Content-type: application/json
Content-length: 248

{
  "comment": "Comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "address-value"
      }
    },
    {
      "emailAddress": {
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="bd421-135">応答</span><span class="sxs-lookup"><span data-stu-id="bd421-135">Response</span></span>
<span data-ttu-id="bd421-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd421-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
