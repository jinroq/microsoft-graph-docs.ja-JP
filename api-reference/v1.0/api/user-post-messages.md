---
title: メッセージを作成する
description: この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 295397e4c85e2096d69e7ba14432cc866b4094a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564044"
---
# <a name="create-message"></a><span data-ttu-id="6c5d0-105">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="6c5d0-105">Create Message</span></span>

<span data-ttu-id="6c5d0-p102">この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="6c5d0-109">同じ **POST** の呼び出しで下書きを作成するときに、[添付ファイル](../resources/attachment.md)を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-109">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c5d0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c5d0-110">Permissions</span></span>
<span data-ttu-id="6c5d0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c5d0-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c5d0-113">Permission type</span></span>      | <span data-ttu-id="6c5d0-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c5d0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c5d0-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c5d0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6c5d0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c5d0-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6c5d0-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c5d0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c5d0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c5d0-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6c5d0-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c5d0-119">Application</span></span> | <span data-ttu-id="6c5d0-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c5d0-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c5d0-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c5d0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="6c5d0-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c5d0-122">Request headers</span></span>
| <span data-ttu-id="6c5d0-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c5d0-123">Header</span></span>       | <span data-ttu-id="6c5d0-124">値</span><span class="sxs-lookup"><span data-stu-id="6c5d0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c5d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c5d0-125">Authorization</span></span>  | <span data-ttu-id="6c5d0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c5d0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c5d0-128">Content-Type</span></span>  | <span data-ttu-id="6c5d0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6c5d0-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c5d0-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c5d0-130">Request body</span></span>
<span data-ttu-id="6c5d0-131">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-131">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="6c5d0-132">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにメッセージに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-132">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="6c5d0-133">応答</span><span class="sxs-lookup"><span data-stu-id="6c5d0-133">Response</span></span>

<span data-ttu-id="6c5d0-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-134">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c5d0-135">例</span><span class="sxs-lookup"><span data-stu-id="6c5d0-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6c5d0-136">要求 1</span><span class="sxs-lookup"><span data-stu-id="6c5d0-136">Request 1</span></span>
<span data-ttu-id="6c5d0-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-137">Here is an example of the request.</span></span>
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
<span data-ttu-id="6c5d0-138">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="6c5d0-139">応答 1</span><span class="sxs-lookup"><span data-stu-id="6c5d0-139">Response 1</span></span>
<span data-ttu-id="6c5d0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="6c5d0-143">要求 2</span><span class="sxs-lookup"><span data-stu-id="6c5d0-143">Request 2</span></span>
<span data-ttu-id="6c5d0-144">次の例では、メッセージの下書きを作成する際に顧客のインターネット メッセージ ヘッダーをいくつか追加します。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-144">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="6c5d0-145">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="6c5d0-146">応答 2</span><span class="sxs-lookup"><span data-stu-id="6c5d0-146">Response 2</span></span>
<span data-ttu-id="6c5d0-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-147">Here is an example of the response.</span></span> <span data-ttu-id="6c5d0-148">注: インターネット メッセージ ヘッダーは、既定で POST レスポンスに返されません。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-148">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="6c5d0-149">簡潔にするために、ここに示す応答オブジェクトも切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6c5d0-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c5d0-150">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6c5d0-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c5d0-151">See also</span></span>

- [<span data-ttu-id="6c5d0-152">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6c5d0-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6c5d0-153">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6c5d0-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
