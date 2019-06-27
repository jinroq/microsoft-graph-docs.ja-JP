---
title: メッセージを作成する
description: この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f3157977ee66aab36eef55dec50c7ea387936ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269973"
---
# <a name="create-message"></a><span data-ttu-id="0a70e-105">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="0a70e-105">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a70e-p102">この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="0a70e-109">同じ**POST**呼び出しで下書きを作成する際に、次のことを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="0a70e-109">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="0a70e-110">[添付ファイル](../resources/attachment.md)を含める</span><span class="sxs-lookup"><span data-stu-id="0a70e-110">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="0a70e-111">別のユーザーを新しいメッセージで呼び出すには、[メンション](../resources/mention.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="0a70e-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a70e-112">Permissions</span></span>
<span data-ttu-id="0a70e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a70e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a70e-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a70e-115">Permission type</span></span>      | <span data-ttu-id="0a70e-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a70e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a70e-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a70e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0a70e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a70e-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0a70e-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a70e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a70e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a70e-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0a70e-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a70e-121">Application</span></span> | <span data-ttu-id="0a70e-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a70e-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a70e-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a70e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="0a70e-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a70e-124">Request headers</span></span>
| <span data-ttu-id="0a70e-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a70e-125">Header</span></span>       | <span data-ttu-id="0a70e-126">値</span><span class="sxs-lookup"><span data-stu-id="0a70e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a70e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a70e-127">Authorization</span></span>  | <span data-ttu-id="0a70e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a70e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a70e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a70e-130">Content-Type</span></span>  | <span data-ttu-id="0a70e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0a70e-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a70e-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a70e-132">Request body</span></span>
<span data-ttu-id="0a70e-133">要求本文で、[メッセージ](../resources/message.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-133">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="0a70e-134">新しいメッセージで別のユーザーを呼び出すために、**メンション**を使用する場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="0a70e-134">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="0a70e-135">要求本文に、必要な**Torecipients**プロパティ、**メンション**プロパティ、および任意の書き込み可能なメッセージプロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="0a70e-135">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="0a70e-136">**メンション**プロパティの各メンションに対して、**説明**されているプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a70e-136">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="0a70e-137">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにメッセージに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="0a70e-137">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="0a70e-138">応答</span><span class="sxs-lookup"><span data-stu-id="0a70e-138">Response</span></span>

<span data-ttu-id="0a70e-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[message](../resources/message.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-139">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a70e-140">例</span><span class="sxs-lookup"><span data-stu-id="0a70e-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="0a70e-141">要求 1</span><span class="sxs-lookup"><span data-stu-id="0a70e-141">Request 1</span></span>
<span data-ttu-id="0a70e-142">新しいメッセージの下書きを作成する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-142">Here is an example of the request to create a draft of a new message.</span></span>
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
<span data-ttu-id="0a70e-143">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-143">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="0a70e-144">応答 1</span><span class="sxs-lookup"><span data-stu-id="0a70e-144">Response 1</span></span>
<span data-ttu-id="0a70e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a70e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a70e-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0a70e-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a70e-149">C#</span><span class="sxs-lookup"><span data-stu-id="0a70e-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a70e-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a70e-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0a70e-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="0a70e-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="0a70e-152">要求 2</span><span class="sxs-lookup"><span data-stu-id="0a70e-152">Request 2</span></span>
<span data-ttu-id="0a70e-153">次の例では、Randi という下書き電子メールを、Samantha ブースに示します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-153">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="0a70e-154">このメッセージには、別のユーザーの Dana Swope も含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a70e-154">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="0a70e-155">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-155">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
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


##### <a name="response-2"></a><span data-ttu-id="0a70e-156">応答 2</span><span class="sxs-lookup"><span data-stu-id="0a70e-156">Response 2</span></span>
<span data-ttu-id="0a70e-p107">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a70e-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a70e-160">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0a70e-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a70e-161">C#</span><span class="sxs-lookup"><span data-stu-id="0a70e-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a70e-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a70e-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0a70e-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="0a70e-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-3"></a><span data-ttu-id="0a70e-164">要求 3</span><span class="sxs-lookup"><span data-stu-id="0a70e-164">Request 3</span></span>
<span data-ttu-id="0a70e-165">次の例では、メッセージの下書きを作成する際に顧客のインターネット メッセージ ヘッダーをいくつか追加します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-165">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="0a70e-166">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a70e-166">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="0a70e-167">応答 3</span><span class="sxs-lookup"><span data-stu-id="0a70e-167">Response 3</span></span>
<span data-ttu-id="0a70e-168">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0a70e-168">Here is an example of the response.</span></span> <span data-ttu-id="0a70e-169">注: インターネット メッセージ ヘッダーは、既定で POST レスポンスに返されません。</span><span class="sxs-lookup"><span data-stu-id="0a70e-169">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="0a70e-170">簡潔にするために、ここに示す応答オブジェクトも切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0a70e-170">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="0a70e-171">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a70e-171">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a70e-172">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0a70e-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a70e-173">C#</span><span class="sxs-lookup"><span data-stu-id="0a70e-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a70e-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a70e-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0a70e-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="0a70e-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="0a70e-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="0a70e-176">See also</span></span>

- [<span data-ttu-id="0a70e-177">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="0a70e-177">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0a70e-178">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="0a70e-178">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0a70e-179">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="0a70e-179">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
