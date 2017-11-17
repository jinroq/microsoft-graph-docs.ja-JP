# <a name="get-user-mailbox-settings"></a><span data-ttu-id="13fdd-101">ユーザーのメールボックスの設定を取得する</span><span class="sxs-lookup"><span data-stu-id="13fdd-101">Get user mailbox settings</span></span>

<span data-ttu-id="13fdd-p101">ユーザーの [mailboxSettings](../resources/mailboxsettings.md) を取得します。これには、自動応答 (ユーザーが電子メールを受信したときに自動的にユーザーに通知)、ロケール (言語と国/地域)、およびタイム ゾーンの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="13fdd-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="13fdd-104">すべてのメールボックス設定を表示することも、特定の設定を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="13fdd-104">You can view all mailbox settings, or, get specific settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="13fdd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13fdd-105">Permissions</span></span>
<span data-ttu-id="13fdd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13fdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13fdd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13fdd-108">Permission type</span></span>      | <span data-ttu-id="13fdd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13fdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13fdd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13fdd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13fdd-111">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13fdd-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="13fdd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13fdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13fdd-113">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13fdd-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="13fdd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13fdd-114">Application</span></span> | <span data-ttu-id="13fdd-115">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13fdd-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13fdd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13fdd-116">HTTP request</span></span>
<span data-ttu-id="13fdd-117">自動応答設定を含むメールボックスのすべての設定を取得するには:</span><span class="sxs-lookup"><span data-stu-id="13fdd-117">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="13fdd-118">特定の設定 (たとえば、自動応答の設定、ロケール、またはタイム ゾーンのみ) を取得するには:</span><span class="sxs-lookup"><span data-stu-id="13fdd-118">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13fdd-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="13fdd-119">Optional query parameters</span></span>
<span data-ttu-id="13fdd-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="13fdd-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="13fdd-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13fdd-121">Request headers</span></span>
| <span data-ttu-id="13fdd-122">名前</span><span class="sxs-lookup"><span data-stu-id="13fdd-122">Name</span></span>       | <span data-ttu-id="13fdd-123">型</span><span class="sxs-lookup"><span data-stu-id="13fdd-123">Type</span></span> | <span data-ttu-id="13fdd-124">説明</span><span class="sxs-lookup"><span data-stu-id="13fdd-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13fdd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="13fdd-125">Authorization</span></span>  | <span data-ttu-id="13fdd-126">string</span><span class="sxs-lookup"><span data-stu-id="13fdd-126">string</span></span>  | <span data-ttu-id="13fdd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13fdd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13fdd-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="13fdd-129">Request body</span></span>
<span data-ttu-id="13fdd-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13fdd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13fdd-131">応答</span><span class="sxs-lookup"><span data-stu-id="13fdd-131">Response</span></span>

<span data-ttu-id="13fdd-132">成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="13fdd-132">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="13fdd-133">[mailboxSettings](../resources/mailboxsettings.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="13fdd-133">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="13fdd-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="13fdd-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="13fdd-135">[localeInfo](../resources/localeinfo.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="13fdd-135">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="13fdd-136">string (**timeZone** の場合)</span><span class="sxs-lookup"><span data-stu-id="13fdd-136">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="13fdd-137">例</span><span class="sxs-lookup"><span data-stu-id="13fdd-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="13fdd-138">要求 1</span><span class="sxs-lookup"><span data-stu-id="13fdd-138">Request 1</span></span>
<span data-ttu-id="13fdd-139">最初の例では、サインインしているユーザーのメールボックスのメールボックス設定をすべて取得します。取得する設定には、自動応答の設定、タイム ゾーン、言語設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="13fdd-139">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="13fdd-140">応答 1</span><span class="sxs-lookup"><span data-stu-id="13fdd-140">Response 1</span></span>
<span data-ttu-id="13fdd-p104">応答には、メールボックス設定のすべてが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13fdd-p104">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="13fdd-144">要求 2</span><span class="sxs-lookup"><span data-stu-id="13fdd-144">Request 2</span></span>
<span data-ttu-id="13fdd-145">2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="13fdd-145">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="13fdd-146">応答 2</span><span class="sxs-lookup"><span data-stu-id="13fdd-146">Response 2</span></span>
<span data-ttu-id="13fdd-p105">この応答には自動とうとう設定のみが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13fdd-p105">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->