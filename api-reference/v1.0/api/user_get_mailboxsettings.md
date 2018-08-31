# <a name="get-user-mailbox-settings"></a><span data-ttu-id="66c7c-101">ユーザーのメールボックスの設定を取得する</span><span class="sxs-lookup"><span data-stu-id="66c7c-101">Get user mailbox settings</span></span>

<span data-ttu-id="66c7c-p101">ユーザーの [mailboxSettings](../resources/mailboxsettings.md) を取得します。これには、自動応答 (ユーザーが電子メールを受信したときに自動的にユーザーに通知)、ロケール (言語と国/地域)、タイム ゾーン、就業時間の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone, and working hours.</span></span>

<span data-ttu-id="66c7c-104">すべてのメールボックス設定を表示することも、特定の設定を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="66c7c-105">タイム ゾーンは、ユーザーが自分のメールボックスに設定できる優先設定のうちの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="66c7c-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="66c7c-106">有効なタイム ゾーンの形式には、Windows タイム ゾーン形式および [Internet Assigned Numbers Authority (IANA) タイム ゾーン](http://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式があります。</span><span class="sxs-lookup"><span data-stu-id="66c7c-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="66c7c-107">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="66c7c-107">The Windows format is the default.</span></span> 

<span data-ttu-id="66c7c-108">ユーザーの優先タイム ゾーンを取得するとき、そのタイム ゾーンは設定された形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="66c7c-109">タイム ゾーンを特定の形式 (Windows または IANA) にする場合は、最初に[メールボックス設定としてその形式の優先タイム ゾーンを更新](user_update_mailboxsettings.md)します。</span><span class="sxs-lookup"><span data-stu-id="66c7c-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="66c7c-110">その後は、その形式でタイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="66c7c-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="66c7c-111">または、アプリ内で形式変換を個別に管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="66c7c-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66c7c-112">Permissions</span></span>
<span data-ttu-id="66c7c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66c7c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66c7c-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66c7c-115">Permission type</span></span>      | <span data-ttu-id="66c7c-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66c7c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66c7c-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66c7c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="66c7c-118">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66c7c-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="66c7c-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66c7c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66c7c-120">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66c7c-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="66c7c-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66c7c-121">Application</span></span> | <span data-ttu-id="66c7c-122">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66c7c-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="66c7c-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66c7c-123">HTTP request</span></span>
<span data-ttu-id="66c7c-124">ユーザーのすべてのメールボックス設定を取得する場合: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="66c7c-124">To get all mailbox settings for a user:<!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="66c7c-125">特定の設定 (たとえば、自動応答の設定、ロケール、タイム ゾーン、または就業時間のみ) を取得する場合: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="66c7c-125">To get specific settings - for example, only the automatic replies settings, locale, time zone, or working hours:<!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66c7c-126">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66c7c-126">Optional query parameters</span></span>
<span data-ttu-id="66c7c-127">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66c7c-127">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66c7c-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66c7c-128">Request headers</span></span>
| <span data-ttu-id="66c7c-129">名前</span><span class="sxs-lookup"><span data-stu-id="66c7c-129">Name</span></span>       | <span data-ttu-id="66c7c-130">型</span><span class="sxs-lookup"><span data-stu-id="66c7c-130">Type</span></span> | <span data-ttu-id="66c7c-131">説明</span><span class="sxs-lookup"><span data-stu-id="66c7c-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66c7c-132">承認</span><span class="sxs-lookup"><span data-stu-id="66c7c-132">Authorization</span></span>  | <span data-ttu-id="66c7c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="66c7c-133">string</span></span>  | <span data-ttu-id="66c7c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66c7c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66c7c-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="66c7c-136">Request body</span></span>
<span data-ttu-id="66c7c-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="66c7c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66c7c-138">応答</span><span class="sxs-lookup"><span data-stu-id="66c7c-138">Response</span></span>

<span data-ttu-id="66c7c-139">成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="66c7c-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="66c7c-140">[mailboxSettings](../resources/mailboxsettings.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="66c7c-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="66c7c-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="66c7c-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="66c7c-142">[localeInfo](../resources/localeinfo.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="66c7c-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="66c7c-143">string (**timeZone** の場合)</span><span class="sxs-lookup"><span data-stu-id="66c7c-143">string (for **timeZone**)</span></span>
- [<span data-ttu-id="66c7c-144">workingHours</span><span class="sxs-lookup"><span data-stu-id="66c7c-144">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="66c7c-145">例</span><span class="sxs-lookup"><span data-stu-id="66c7c-145">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="66c7c-146">要求 1</span><span class="sxs-lookup"><span data-stu-id="66c7c-146">Request 1</span></span>
<span data-ttu-id="66c7c-147">最初の例では、サインインしているユーザーのメールボックスのすべてのメールボックス設定を取得します。取得される設定には、自動応答、ロケール (言語と国/地域)、タイム ゾーン、就業時間の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-147">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="66c7c-148">応答 1</span><span class="sxs-lookup"><span data-stu-id="66c7c-148">Response 1</span></span>
<span data-ttu-id="66c7c-p106">応答には、メールボックス設定のすべてが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.000",
        "endTime":"17:00:00.000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="66c7c-152">要求 2</span><span class="sxs-lookup"><span data-stu-id="66c7c-152">Request 2</span></span>
<span data-ttu-id="66c7c-153">2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="66c7c-153">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="66c7c-154">応答 2</span><span class="sxs-lookup"><span data-stu-id="66c7c-154">Response 2</span></span>
<span data-ttu-id="66c7c-p107">この応答には自動とうとう設定のみが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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


##### <a name="request-3"></a><span data-ttu-id="66c7c-158">要求 3</span><span class="sxs-lookup"><span data-stu-id="66c7c-158">Request 3</span></span>
<span data-ttu-id="66c7c-159">3 番目の例では、サインインしているユーザーのメールボックスの自動応答の設定を具体的に指定して取得します。</span><span class="sxs-lookup"><span data-stu-id="66c7c-159">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="66c7c-160">応答 3</span><span class="sxs-lookup"><span data-stu-id="66c7c-160">Response 3</span></span>
<span data-ttu-id="66c7c-161">この応答には、自動応答の設定のみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-161">The response includes only the working hours settings.</span></span> <span data-ttu-id="66c7c-162">ユーザーの就業時間には、[カスタム タイム ゾーン](../resources/customtimezone.md)が適用されていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="66c7c-162">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="66c7c-163">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="66c7c-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="66c7c-164">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="66c7c-164">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
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