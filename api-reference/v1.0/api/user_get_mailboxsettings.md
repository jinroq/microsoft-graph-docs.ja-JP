# <a name="get-user-mailbox-settings"></a><span data-ttu-id="bee07-101">ユーザーのメールボックスの設定を取得する</span><span class="sxs-lookup"><span data-stu-id="bee07-101">Get user mailbox settings</span></span>

<span data-ttu-id="bee07-p101">ユーザーの [mailboxSettings](../resources/mailboxsettings.md) を取得します。これには、自動応答 (ユーザーが電子メールを受信したときに自動的にユーザーに通知)、ロケール (言語と国/地域)、およびタイム ゾーンの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bee07-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="bee07-104">すべてのメールボックス設定を表示することも、特定の設定を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="bee07-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="bee07-105">タイム ゾーンは、ユーザーが自分のメールボックスに設定できる優先設定のうちの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="bee07-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="bee07-106">有効なタイム ゾーンの形式には、Windows タイム ゾーン形式および [Internet Assigned Numbers Authority (IANA) タイム ゾーン]((http://www.iana.org/time-zones)) (Olson タイム ゾーンとも呼ばれる) 形式があります。</span><span class="sxs-lookup"><span data-stu-id="bee07-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span> <span data-ttu-id="bee07-107">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="bee07-107">The Windows format is the default.</span></span> 

<span data-ttu-id="bee07-108">ユーザーの優先タイム ゾーンを取得するとき、そのタイム ゾーンは設定された形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="bee07-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="bee07-109">タイム ゾーンを特定の形式 (Windows または IANA) にする場合は、最初に[メールボックス設定としてその形式の優先タイム ゾーンを更新](user_update_mailboxsettings.md)します。</span><span class="sxs-lookup"><span data-stu-id="bee07-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="bee07-110">その後は、その形式でタイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="bee07-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="bee07-111">または、アプリ内で形式変換を個別に管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="bee07-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="bee07-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bee07-112">Permissions</span></span>
<span data-ttu-id="bee07-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bee07-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bee07-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bee07-115">Permission type</span></span>      | <span data-ttu-id="bee07-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bee07-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bee07-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bee07-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bee07-118">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bee07-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bee07-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bee07-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bee07-120">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bee07-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="bee07-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bee07-121">Application</span></span> | <span data-ttu-id="bee07-122">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bee07-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bee07-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bee07-123">HTTP request</span></span>
<span data-ttu-id="bee07-124">自動応答設定を含むメールボックスのすべての設定を取得するには:</span><span class="sxs-lookup"><span data-stu-id="bee07-124">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="bee07-125">特定の設定 (たとえば、自動応答の設定、ロケール、またはタイム ゾーンのみ) を取得するには:</span><span class="sxs-lookup"><span data-stu-id="bee07-125">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bee07-126">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bee07-126">Optional query parameters</span></span>
<span data-ttu-id="bee07-127">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター]((http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters))をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bee07-127">This method supports the [OData Query Parameters]((http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bee07-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bee07-128">Request headers</span></span>
| <span data-ttu-id="bee07-129">名前</span><span class="sxs-lookup"><span data-stu-id="bee07-129">Name</span></span>       | <span data-ttu-id="bee07-130">型</span><span class="sxs-lookup"><span data-stu-id="bee07-130">Type</span></span> | <span data-ttu-id="bee07-131">説明</span><span class="sxs-lookup"><span data-stu-id="bee07-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bee07-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="bee07-132">Authorization</span></span>  | <span data-ttu-id="bee07-133">string</span><span class="sxs-lookup"><span data-stu-id="bee07-133">string</span></span>  | <span data-ttu-id="bee07-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bee07-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bee07-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="bee07-136">Request body</span></span>
<span data-ttu-id="bee07-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bee07-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bee07-138">応答</span><span class="sxs-lookup"><span data-stu-id="bee07-138">Response</span></span>

<span data-ttu-id="bee07-139">成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="bee07-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="bee07-140">[mailboxSettings](../resources/mailboxsettings.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bee07-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="bee07-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bee07-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="bee07-142">[localeInfo](../resources/localeinfo.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bee07-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="bee07-143">string (**timeZone** の場合)</span><span class="sxs-lookup"><span data-stu-id="bee07-143">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="bee07-144">例</span><span class="sxs-lookup"><span data-stu-id="bee07-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="bee07-145">要求 1</span><span class="sxs-lookup"><span data-stu-id="bee07-145">Request 1</span></span>
<span data-ttu-id="bee07-146">最初の例では、サインインしているユーザーのメールボックスのメールボックス設定をすべて取得します。取得する設定には、自動応答の設定、タイム ゾーン、言語設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bee07-146">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="bee07-147">応答 1</span><span class="sxs-lookup"><span data-stu-id="bee07-147">Response 1</span></span>
<span data-ttu-id="bee07-p106">応答には、メールボックス設定のすべてが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bee07-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="bee07-151">要求 2</span><span class="sxs-lookup"><span data-stu-id="bee07-151">Request 2</span></span>
<span data-ttu-id="bee07-152">2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="bee07-152">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="bee07-153">応答 2</span><span class="sxs-lookup"><span data-stu-id="bee07-153">Response 2</span></span>
<span data-ttu-id="bee07-p107">この応答には自動とうとう設定のみが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bee07-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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