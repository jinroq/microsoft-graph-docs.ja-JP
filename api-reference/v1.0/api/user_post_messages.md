# <a name="create-message"></a><span data-ttu-id="09257-101">メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="09257-101">Create Message</span></span>

<span data-ttu-id="09257-p101">この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。</span><span class="sxs-lookup"><span data-stu-id="09257-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="09257-105">同じ **POST** の呼び出しで下書きを作成するときに、[添付ファイル](../resources/attachment.md)を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="09257-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09257-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09257-106">Permissions</span></span>
<span data-ttu-id="09257-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09257-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="09257-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09257-109">Permission type</span></span>      | <span data-ttu-id="09257-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="09257-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09257-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09257-111">Delegated (work or school account)</span></span> | <span data-ttu-id="09257-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09257-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="09257-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09257-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09257-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09257-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="09257-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09257-115">Application</span></span> | <span data-ttu-id="09257-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09257-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="09257-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09257-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="09257-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09257-118">Request headers</span></span>
| <span data-ttu-id="09257-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09257-119">Header</span></span>       | <span data-ttu-id="09257-120">値</span><span class="sxs-lookup"><span data-stu-id="09257-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09257-121">承認</span><span class="sxs-lookup"><span data-stu-id="09257-121">Authorization</span></span>  | <span data-ttu-id="09257-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09257-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09257-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09257-124">Content-Type</span></span>  | <span data-ttu-id="09257-125">アプリケーション/json</span><span class="sxs-lookup"><span data-stu-id="09257-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09257-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="09257-126">Request body</span></span>
<span data-ttu-id="09257-127">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09257-127">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="09257-128">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにメッセージに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="09257-128">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="09257-129">応答</span><span class="sxs-lookup"><span data-stu-id="09257-129">Response</span></span>

<span data-ttu-id="09257-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09257-130">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09257-131">例</span><span class="sxs-lookup"><span data-stu-id="09257-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="09257-132">要求 1</span><span class="sxs-lookup"><span data-stu-id="09257-132">Request 1</span></span>
<span data-ttu-id="09257-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09257-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
<span data-ttu-id="09257-134">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09257-134">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="09257-135">応答 1</span><span class="sxs-lookup"><span data-stu-id="09257-135">Response 1</span></span>
<span data-ttu-id="09257-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09257-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="09257-139">要求 2</span><span class="sxs-lookup"><span data-stu-id="09257-139">Request 2</span></span>
<span data-ttu-id="09257-140">次の例では、メッセージの下書きを作成するときに、顧客のインターネット メッセージ ヘッダーを 2 つ追加します。</span><span class="sxs-lookup"><span data-stu-id="09257-140">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```
<span data-ttu-id="09257-141">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09257-141">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="09257-142">応答 2</span><span class="sxs-lookup"><span data-stu-id="09257-142">Response 2</span></span>
<span data-ttu-id="09257-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="09257-143">Here is an example of the response.</span></span> <span data-ttu-id="09257-144">注: 既定では、インターネット メッセージのヘッダーは、POST 応答では返されません。</span><span class="sxs-lookup"><span data-stu-id="09257-144">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="09257-145">注: 簡潔にするために、ここに示す応答オブジェクトも切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="09257-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="09257-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="09257-146">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
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

## <a name="see-also"></a><span data-ttu-id="09257-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="09257-147">See also</span></span>

- [<span data-ttu-id="09257-148">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="09257-148">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="09257-149">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="09257-149">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
