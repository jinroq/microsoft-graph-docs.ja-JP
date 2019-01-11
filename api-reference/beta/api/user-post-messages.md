---
title: メッセージを作成する
description: この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。
localization_priority: Normal
ms.openlocfilehash: ff4472b84ed218607ff6cda2b991f6bf2b63cda3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883735"
---
# <a name="create-message"></a><span data-ttu-id="16e07-105">メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="16e07-105">Create Message</span></span>

> <span data-ttu-id="16e07-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16e07-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16e07-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e07-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16e07-p103">この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。</span><span class="sxs-lookup"><span data-stu-id="16e07-p103">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="16e07-111">同じ**POST**呼び出しで下書きを作成中に次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="16e07-111">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="16e07-112">[添付ファイル](../resources/attachment.md)を含める</span><span class="sxs-lookup"><span data-stu-id="16e07-112">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="16e07-113">[説明](../resources/mention.md)を使用して、新しいメッセージに別のユーザーを呼び出す</span><span class="sxs-lookup"><span data-stu-id="16e07-113">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="16e07-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16e07-114">Permissions</span></span>
<span data-ttu-id="16e07-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16e07-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e07-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16e07-117">Permission type</span></span>      | <span data-ttu-id="16e07-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16e07-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16e07-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16e07-119">Delegated (work or school account)</span></span> | <span data-ttu-id="16e07-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16e07-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="16e07-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16e07-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16e07-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16e07-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="16e07-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16e07-123">Application</span></span> | <span data-ttu-id="16e07-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16e07-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="16e07-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16e07-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="16e07-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16e07-126">Request headers</span></span>
| <span data-ttu-id="16e07-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16e07-127">Header</span></span>       | <span data-ttu-id="16e07-128">値</span><span class="sxs-lookup"><span data-stu-id="16e07-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16e07-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="16e07-129">Authorization</span></span>  | <span data-ttu-id="16e07-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16e07-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16e07-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16e07-132">Content-Type</span></span>  | <span data-ttu-id="16e07-133">application/json</span><span class="sxs-lookup"><span data-stu-id="16e07-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16e07-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="16e07-134">Request body</span></span>
<span data-ttu-id="16e07-135">要求の本文に、[メッセージ](../resources/message.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="16e07-135">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="16e07-136">**言及**を使用して新しいメッセージに別のユーザーを呼び出す場合は。</span><span class="sxs-lookup"><span data-stu-id="16e07-136">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="16e07-137">要求の本文で必要な**toRecipients**プロパティ**を示して**プロパティ、および任意の書き込み可能なメッセージ プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="16e07-137">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="16e07-138">**紹介**プロパティにそれぞれ記載されている、**記載されている**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="16e07-138">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="16e07-139">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにメッセージに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="16e07-139">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="16e07-140">応答</span><span class="sxs-lookup"><span data-stu-id="16e07-140">Response</span></span>

<span data-ttu-id="16e07-141">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[メッセージ](../resources/message.md)のオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="16e07-141">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e07-142">例</span><span class="sxs-lookup"><span data-stu-id="16e07-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="16e07-143">要求 1</span><span class="sxs-lookup"><span data-stu-id="16e07-143">Request 1</span></span>
<span data-ttu-id="16e07-144">ここでは、新しいメッセージの下書きを作成する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16e07-144">Here is an example of the request to create a draft of a new message.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
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
<span data-ttu-id="16e07-145">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16e07-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="16e07-146">応答 1</span><span class="sxs-lookup"><span data-stu-id="16e07-146">Response 1</span></span>
<span data-ttu-id="16e07-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16e07-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('ad787b4f-1fda-4523-8e48-ffedb7f4635f')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t\"",
    "id":"AAMkAGRWAAAFSmKXAAA=",
    "createdDateTime":"2017-12-23T07:29:57Z",
    "lastModifiedDateTime":"2017-12-23T07:29:58Z",
    "changeKey":"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t",
    "categories":[

    ],
    "receivedDateTime":"2017-12-23T07:29:58Z",
    "sentDateTime":"2017-12-23T07:29:58Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR130@MWHPR130.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkAGRWAAAAAAEPAAA=",
    "conversationId":"AAQkAGRVYAsRJrRdc_mWNaxU=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkAGRWAAAFSmKXAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"AdeleV@contoso.onmicrosoft.com",
                "address":"AdeleV@contoso.onmicrosoft.com"
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

##### <a name="request-2"></a><span data-ttu-id="16e07-150">要求 2</span><span class="sxs-lookup"><span data-stu-id="16e07-150">Request 2</span></span>
<span data-ttu-id="16e07-151">次の例では、彼女のブースに Randi 就くで下書きのメールを示しています。</span><span class="sxs-lookup"><span data-stu-id="16e07-151">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="16e07-152">メッセージには、Dana Swope の他のユーザーの参照も含まれています。</span><span class="sxs-lookup"><span data-stu-id="16e07-152">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="16e07-153">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16e07-153">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_mentions_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject": "Party planning",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {    
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
}
```


##### <a name="response-2"></a><span data-ttu-id="16e07-154">応答 2</span><span class="sxs-lookup"><span data-stu-id="16e07-154">Response 2</span></span>
<span data-ttu-id="16e07-p108">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16e07-p108">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/Messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAbYj7\"",
  "id":"AQMkADJmMTUAAAW1fsAAAAA==",
  "body":{
    "contentType":"Text",
    "content":""
  },
  "bodyPreview":"",
  "sender":null,
  "from":null,
  "subject": "Party planning",
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      }
    }
  ],
  "mentionsPreview":{
    "isMentioned":false
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAW1fsAAAAA%3D%3D')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')/mentions('4577bba4-b063-4cea-9073-6f7ca815fcec')",
      "id":"4577bba4-b063-4cea-9073-6f7ca815fcec",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-22T02:22:44Z",
      "serverCreatedDateTime":"2016-07-22T02:22:44.201Z",
      "deepLink":null,
      "application":null
    }
  ]
}

```

##### <a name="request-3"></a><span data-ttu-id="16e07-158">要求 3</span><span class="sxs-lookup"><span data-stu-id="16e07-158">Request 3</span></span>
<span data-ttu-id="16e07-159">次の使用例は、メッセージの下書きを作成するときにいくつかの顧客のインターネット メッセージ ヘッダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="16e07-159">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
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
<span data-ttu-id="16e07-160">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16e07-160">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="16e07-161">応答 3</span><span class="sxs-lookup"><span data-stu-id="16e07-161">Response 3</span></span>
<span data-ttu-id="16e07-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="16e07-162">Here is an example of the response.</span></span> <span data-ttu-id="16e07-163">注: インターネット メッセージのヘッダーは、POST 応答に既定では返されません。</span><span class="sxs-lookup"><span data-stu-id="16e07-163">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="16e07-164">ここに示す応答オブジェクトは、簡潔にするためもあります。</span><span class="sxs-lookup"><span data-stu-id="16e07-164">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="16e07-165">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16e07-165">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
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
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
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

## <a name="see-also"></a><span data-ttu-id="16e07-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="16e07-166">See also</span></span>

- [<span data-ttu-id="16e07-167">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="16e07-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="16e07-168">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="16e07-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="16e07-169">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="16e07-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
