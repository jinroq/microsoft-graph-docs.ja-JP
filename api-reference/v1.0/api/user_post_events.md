# <a name="create-event"></a><span data-ttu-id="46010-101">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="46010-101">Create Event</span></span>

<span data-ttu-id="46010-102">ユーザーの既定の予定表または指定した予定表で[イベント](../resources/event.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="46010-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="46010-103">**start** と **end** プロパティの型が [dateTimeTimeZone](../resources/datetimetimezone.md) であるため、これらの値の一部としてイベントの開始時刻と終了時刻のそれぞれにタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="46010-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="46010-104">イベントが作成されると、サーバーはすべての出席者に招待状を送信します。</span><span class="sxs-lookup"><span data-stu-id="46010-104">When the event is created, the server send invitations to all attendees.</span></span>


## <a name="permissions"></a><span data-ttu-id="46010-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46010-105">Permissions</span></span>
<span data-ttu-id="46010-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="46010-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46010-108">Permission type</span></span>      | <span data-ttu-id="46010-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46010-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46010-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46010-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46010-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46010-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="46010-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46010-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46010-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46010-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="46010-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46010-114">Application</span></span> | <span data-ttu-id="46010-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46010-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="46010-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46010-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="46010-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46010-117">Request headers</span></span>
| <span data-ttu-id="46010-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46010-118">Header</span></span>       | <span data-ttu-id="46010-119">値</span><span class="sxs-lookup"><span data-stu-id="46010-119">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="46010-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="46010-120">Authorization</span></span>  | <span data-ttu-id="46010-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="46010-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="46010-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46010-123">Content-Type</span></span>  | <span data-ttu-id="46010-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="46010-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46010-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="46010-126">Request body</span></span>
<span data-ttu-id="46010-127">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="46010-127">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="46010-128">**イベント** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにイベントに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="46010-128">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="46010-129">応答</span><span class="sxs-lookup"><span data-stu-id="46010-129">Response</span></span>

<span data-ttu-id="46010-130">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46010-130">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46010-131">例</span><span class="sxs-lookup"><span data-stu-id="46010-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46010-132">要求</span><span class="sxs-lookup"><span data-stu-id="46010-132">Request</span></span>
<span data-ttu-id="46010-p104">以下は、要求の例です。`Prefer: outlook.timezone` 要求ヘッダーを使用して、応答の**開始**時刻と**終了**時刻でそのタイム ゾーンを使用するように指定します。</span><span class="sxs-lookup"><span data-stu-id="46010-p104">Here is an example of the request. It uses the `Prefer: outlook.timezone` request header to specify the **start** and **end** times in the response should use that time zone.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"fannyd@contoso.onmicrosoft.com",
        "name": "Fanny Downs"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="46010-135">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="46010-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="46010-136">応答</span><span class="sxs-lookup"><span data-stu-id="46010-136">Response</span></span>
<span data-ttu-id="46010-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46010-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Fanny Downs",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```
## <a name="see-also"></a><span data-ttu-id="46010-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="46010-140">See also</span></span>

- [<span data-ttu-id="46010-141">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="46010-141">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="46010-142">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="46010-142">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
