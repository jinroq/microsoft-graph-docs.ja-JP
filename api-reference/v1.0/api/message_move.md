# <a name="message-move"></a><span data-ttu-id="35438-101">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="35438-101">message: move</span></span>

<span data-ttu-id="35438-102">メッセージをフォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="35438-102">Move a message to a folder.</span></span> <span data-ttu-id="35438-103">これは、宛先フォルダーにメッセージの新しいコピーを作成し、元のメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="35438-103">This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="35438-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35438-104">Permissions</span></span>

<span data-ttu-id="35438-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="35438-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35438-107">Permission type</span></span> | <span data-ttu-id="35438-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35438-108">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="35438-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35438-109">Delegated (work or school account)</span></span> | <span data-ttu-id="35438-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35438-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35438-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35438-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35438-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35438-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35438-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35438-113">Application</span></span> | <span data-ttu-id="35438-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35438-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35438-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35438-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="35438-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35438-116">Request headers</span></span>

| <span data-ttu-id="35438-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35438-117">Header</span></span> | <span data-ttu-id="35438-118">値</span><span class="sxs-lookup"><span data-stu-id="35438-118">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="35438-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="35438-119">Authorization</span></span> | <span data-ttu-id="35438-120">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="35438-120"></span></span> <span data-ttu-id="35438-121">必須。</span><span class="sxs-lookup"><span data-stu-id="35438-121">Required.</span></span> |
| <span data-ttu-id="35438-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35438-122">Content-Type</span></span> | <span data-ttu-id="35438-123">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="35438-123"></span></span> <span data-ttu-id="35438-124">必須。</span><span class="sxs-lookup"><span data-stu-id="35438-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35438-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="35438-125">Request body</span></span>

<span data-ttu-id="35438-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="35438-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35438-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="35438-127">Parameter</span></span>   | <span data-ttu-id="35438-128">型</span><span class="sxs-lookup"><span data-stu-id="35438-128">Type</span></span> |<span data-ttu-id="35438-129">説明</span><span class="sxs-lookup"><span data-stu-id="35438-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35438-130">destinationId</span><span class="sxs-lookup"><span data-stu-id="35438-130">destinationId</span></span>|<span data-ttu-id="35438-131">文字列</span><span class="sxs-lookup"><span data-stu-id="35438-131">String</span></span>|<span data-ttu-id="35438-132">宛先フォルダーの ID または既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="35438-132">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="35438-133">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35438-133">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="35438-134">応答</span><span class="sxs-lookup"><span data-stu-id="35438-134">Response</span></span>

<span data-ttu-id="35438-135">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文内の [message](../resources/message.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="35438-135">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35438-136">例</span><span class="sxs-lookup"><span data-stu-id="35438-136">Example</span></span>

<span data-ttu-id="35438-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="35438-137">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="35438-138">要求</span><span class="sxs-lookup"><span data-stu-id="35438-138">Request</span></span>

<span data-ttu-id="35438-139"> 次の要求は、その要求の既知のフォルダ名 `deleteditems` で識別される、削除済みアイテム  フォルダに指定したメッセージを移動します。</span><span class="sxs-lookup"><span data-stu-id="35438-139">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="35438-140">応答</span><span class="sxs-lookup"><span data-stu-id="35438-140">Response</span></span>

<span data-ttu-id="35438-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="35438-141">Here is an example of the response.</span></span>

> <span data-ttu-id="35438-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="35438-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
