# <a name="get-message"></a><span data-ttu-id="729db-101">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="729db-101">Get message</span></span>

<span data-ttu-id="729db-102">[メッセージ](../resources/message.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="729db-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="729db-103">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="729db-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="729db-104">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="729db-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="729db-105">別のユーザーのメッセージ フォルダーでメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="729db-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="729db-106">アプリケーションのアクセス許可がある場合、または 1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーのメッセージ フォルダーからメッセージを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="729db-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="729db-107">このセクションでは、委任されたアクセス許可に関連するシナリオについて説明します。</span><span class="sxs-lookup"><span data-stu-id="729db-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="729db-108">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="729db-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="729db-109">別のユーザー Garth は、John とメッセージ フォルダーを共有しています。</span><span class="sxs-lookup"><span data-stu-id="729db-109">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="729db-110">その場合、以下に示すサンプル クエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーでメッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="729db-110">You can get a message in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="729db-111">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対しサポートされているすべての GET メッセージ操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="729db-111">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="729db-112">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="729db-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="729db-113">Garth が John とメッセージ フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="729db-113">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="729db-114">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身のメッセージ フォルダーでメッセージを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="729db-114">In such cases, specifying a user ID or user principal name only works for getting a message in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="729db-115">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="729db-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="729db-116">共有の連絡先フォルダー、予定表、メッセージ フォルダー</span><span class="sxs-lookup"><span data-stu-id="729db-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="729db-117">連絡先、イベント、共有フォルダー内のメッセージ</span><span class="sxs-lookup"><span data-stu-id="729db-117">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="729db-118">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="729db-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="729db-119">この機能は、連絡先、イベント、メッセージ、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="729db-119">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="729db-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="729db-120">Permissions</span></span>
<span data-ttu-id="729db-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="729db-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="729db-123">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="729db-123">Permission type</span></span>      | <span data-ttu-id="729db-124">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="729db-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="729db-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="729db-125">Delegated (work or school account)</span></span> | <span data-ttu-id="729db-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="729db-126">Mail.Read</span></span>    |
|<span data-ttu-id="729db-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="729db-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="729db-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="729db-128">Mail.Read</span></span>    |
|<span data-ttu-id="729db-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="729db-129">Application</span></span> | <span data-ttu-id="729db-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="729db-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="729db-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="729db-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="729db-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="729db-132">Optional query parameters</span></span>
<span data-ttu-id="729db-133">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="729db-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="729db-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="729db-134">Request headers</span></span>
| <span data-ttu-id="729db-135">名前</span><span class="sxs-lookup"><span data-stu-id="729db-135">Name</span></span>       | <span data-ttu-id="729db-136">型</span><span class="sxs-lookup"><span data-stu-id="729db-136">Type</span></span> | <span data-ttu-id="729db-137">説明</span><span class="sxs-lookup"><span data-stu-id="729db-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="729db-138">承認</span><span class="sxs-lookup"><span data-stu-id="729db-138">Authorization</span></span>  | <span data-ttu-id="729db-139">文字列</span><span class="sxs-lookup"><span data-stu-id="729db-139">string</span></span>  | <span data-ttu-id="729db-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="729db-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="729db-142">優先: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="729db-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="729db-143">文字列</span><span class="sxs-lookup"><span data-stu-id="729db-143">string</span></span> | <span data-ttu-id="729db-144">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="729db-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="729db-145">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="729db-145">Values can be "text" or "html".</span></span> <span data-ttu-id="729db-146">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="729db-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="729db-147">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="729db-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="729db-148">省略可能。</span><span class="sxs-lookup"><span data-stu-id="729db-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="729db-149">要求本文</span><span class="sxs-lookup"><span data-stu-id="729db-149">Request body</span></span>
<span data-ttu-id="729db-150">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="729db-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="729db-151">応答</span><span class="sxs-lookup"><span data-stu-id="729db-151">Response</span></span>

<span data-ttu-id="729db-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="729db-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="729db-153">例</span><span class="sxs-lookup"><span data-stu-id="729db-153">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="729db-154">要求 1</span><span class="sxs-lookup"><span data-stu-id="729db-154">Request 1</span></span>
<span data-ttu-id="729db-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="729db-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="729db-156">応答 1</span><span class="sxs-lookup"><span data-stu-id="729db-156">Response 1</span></span>
<span data-ttu-id="729db-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="729db-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="729db-160">要求 2</span><span class="sxs-lookup"><span data-stu-id="729db-160">Request 2</span></span>
<span data-ttu-id="729db-161">次の例では、メッセージのインターネット メッセージ ヘッダーを取得する `$select` クエリ パラメーターを実行します。</span><span class="sxs-lookup"><span data-stu-id="729db-161">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="729db-162">応答 2</span><span class="sxs-lookup"><span data-stu-id="729db-162">Response 2</span></span>
<span data-ttu-id="729db-163">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="729db-163">Here is an example of the response.</span></span> <span data-ttu-id="729db-164">注: 簡潔にするために、応答オブジェクトの一連のメッセージ ヘッダーが切り捨てられています。</span><span class="sxs-lookup"><span data-stu-id="729db-164">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="729db-165">実際の呼び出しではすべてのヘッダーが返されます。</span><span class="sxs-lookup"><span data-stu-id="729db-165">All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="729db-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="729db-166">See also</span></span>

- [<span data-ttu-id="729db-167">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="729db-167">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="729db-168">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="729db-168">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
