---
title: メッセージを取得する
description: メッセージ オブジェクトのプロパティと関係を取得します。
author: angelgolfer-ms
ms.openlocfilehash: 03ff42bc22d79caf1d432170d3a3ead50af4cea0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332404"
---
# <a name="get-message"></a><span data-ttu-id="0f417-103">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0f417-103">Get message</span></span>

<span data-ttu-id="0f417-104">[メッセージ](../resources/message.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="0f417-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="0f417-105">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="0f417-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="0f417-106">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーにメッセージを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="0f417-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="0f417-107">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="0f417-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0f417-108">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="0f417-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0f417-109">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f417-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="0f417-110">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="0f417-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="0f417-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f417-111">Permissions</span></span>
<span data-ttu-id="0f417-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f417-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f417-114">Permission type</span></span>      | <span data-ttu-id="0f417-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f417-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f417-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f417-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0f417-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0f417-117">Mail.Read</span></span>    |
|<span data-ttu-id="0f417-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f417-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f417-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0f417-119">Mail.Read</span></span>    |
|<span data-ttu-id="0f417-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f417-120">Application</span></span> | <span data-ttu-id="0f417-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0f417-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f417-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f417-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0f417-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0f417-123">Optional query parameters</span></span>
<span data-ttu-id="0f417-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0f417-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0f417-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f417-125">Request headers</span></span>
| <span data-ttu-id="0f417-126">名前</span><span class="sxs-lookup"><span data-stu-id="0f417-126">Name</span></span>       | <span data-ttu-id="0f417-127">種類</span><span class="sxs-lookup"><span data-stu-id="0f417-127">Type</span></span> | <span data-ttu-id="0f417-128">説明</span><span class="sxs-lookup"><span data-stu-id="0f417-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f417-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f417-129">Authorization</span></span>  | <span data-ttu-id="0f417-130">string</span><span class="sxs-lookup"><span data-stu-id="0f417-130">string</span></span>  | <span data-ttu-id="0f417-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0f417-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0f417-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0f417-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0f417-134">string</span><span class="sxs-lookup"><span data-stu-id="0f417-134">string</span></span> | <span data-ttu-id="0f417-135">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="0f417-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="0f417-136">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="0f417-136">Values can be "text" or "html".</span></span> <span data-ttu-id="0f417-137">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="0f417-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="0f417-138">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="0f417-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="0f417-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0f417-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f417-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f417-140">Request body</span></span>
<span data-ttu-id="0f417-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0f417-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f417-142">応答</span><span class="sxs-lookup"><span data-stu-id="0f417-142">Response</span></span>

<span data-ttu-id="0f417-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f417-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f417-144">例</span><span class="sxs-lookup"><span data-stu-id="0f417-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="0f417-145">要求 1</span><span class="sxs-lookup"><span data-stu-id="0f417-145">Request 1</span></span>
<span data-ttu-id="0f417-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f417-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="0f417-147">応答 1</span><span class="sxs-lookup"><span data-stu-id="0f417-147">Response 1</span></span>
<span data-ttu-id="0f417-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f417-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
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

##### <a name="request-2"></a><span data-ttu-id="0f417-151">要求 2</span><span class="sxs-lookup"><span data-stu-id="0f417-151">Request 2</span></span>
<span data-ttu-id="0f417-152">次の例では、`$select`メッセージのインターネット メッセージ ヘッダーを取得するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="0f417-152">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="0f417-153">応答 2</span><span class="sxs-lookup"><span data-stu-id="0f417-153">Response 2</span></span>
<span data-ttu-id="0f417-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0f417-154">Here is an example of the response.</span></span> <span data-ttu-id="0f417-155">注: 簡潔にするための一連の応答オブジェクトでメッセージ ヘッダーが切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="0f417-155">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="0f417-156">すべてのヘッダーは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f417-156">All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
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


## <a name="see-also"></a><span data-ttu-id="0f417-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f417-157">See also</span></span>

- [<span data-ttu-id="0f417-158">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="0f417-158">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0f417-159">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="0f417-159">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
