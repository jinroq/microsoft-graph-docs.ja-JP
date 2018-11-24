# <a name="get-message"></a><span data-ttu-id="01896-101">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="01896-101">Get message</span></span>

<span data-ttu-id="01896-102">[メッセージ](../resources/message.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="01896-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="01896-103">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="01896-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="01896-104">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーにメッセージを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="01896-104">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="01896-105">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="01896-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="01896-106">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="01896-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="01896-107">[詳細と例](../../../concepts/outlook-share-messages-folders.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01896-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

<span data-ttu-id="01896-108">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="01896-108">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="01896-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="01896-109">Permissions</span></span>
<span data-ttu-id="01896-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01896-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01896-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="01896-112">Permission type</span></span>      | <span data-ttu-id="01896-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="01896-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01896-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="01896-114">Delegated (work or school account)</span></span> | <span data-ttu-id="01896-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01896-115">Mail.Read</span></span>    |
|<span data-ttu-id="01896-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="01896-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01896-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01896-117">Mail.Read</span></span>    |
|<span data-ttu-id="01896-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="01896-118">Application</span></span> | <span data-ttu-id="01896-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01896-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="01896-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="01896-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01896-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="01896-121">Optional query parameters</span></span>
<span data-ttu-id="01896-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="01896-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01896-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01896-123">Request headers</span></span>
| <span data-ttu-id="01896-124">名前</span><span class="sxs-lookup"><span data-stu-id="01896-124">Name</span></span>       | <span data-ttu-id="01896-125">型</span><span class="sxs-lookup"><span data-stu-id="01896-125">Type</span></span> | <span data-ttu-id="01896-126">説明</span><span class="sxs-lookup"><span data-stu-id="01896-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01896-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="01896-127">Authorization</span></span>  | <span data-ttu-id="01896-128">string</span><span class="sxs-lookup"><span data-stu-id="01896-128">string</span></span>  | <span data-ttu-id="01896-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="01896-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01896-131">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="01896-131">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="01896-132">文字列</span><span class="sxs-lookup"><span data-stu-id="01896-132">string</span></span> | <span data-ttu-id="01896-133">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="01896-133">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="01896-134">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="01896-134">Values can be "text" or "html".</span></span> <span data-ttu-id="01896-135">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="01896-135">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="01896-136">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="01896-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="01896-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="01896-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01896-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="01896-138">Request body</span></span>
<span data-ttu-id="01896-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="01896-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01896-140">応答</span><span class="sxs-lookup"><span data-stu-id="01896-140">Response</span></span>

<span data-ttu-id="01896-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="01896-141">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01896-142">例</span><span class="sxs-lookup"><span data-stu-id="01896-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="01896-143">要求 1</span><span class="sxs-lookup"><span data-stu-id="01896-143">Request 1</span></span>
<span data-ttu-id="01896-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="01896-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="01896-145">応答 1</span><span class="sxs-lookup"><span data-stu-id="01896-145">Response 1</span></span>
<span data-ttu-id="01896-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="01896-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="01896-149">要求 2</span><span class="sxs-lookup"><span data-stu-id="01896-149">Request 2</span></span>
<span data-ttu-id="01896-150">次の例では、`$select`メッセージのインターネット メッセージ ヘッダーを取得するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="01896-150">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="01896-151">応答 2</span><span class="sxs-lookup"><span data-stu-id="01896-151">Response 2</span></span>
<span data-ttu-id="01896-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="01896-152">Here is an example of the response.</span></span> <span data-ttu-id="01896-153">注: 簡潔にするための一連の応答オブジェクトでメッセージ ヘッダーが切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="01896-153">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="01896-154">すべてのヘッダーは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="01896-154">All of the headers will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="01896-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="01896-155">See also</span></span>

- [<span data-ttu-id="01896-156">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="01896-156">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="01896-157">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="01896-157">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
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
