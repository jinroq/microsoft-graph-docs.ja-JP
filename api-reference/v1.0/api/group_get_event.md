# <a name="get-event"></a><span data-ttu-id="ab896-101">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="ab896-101">Get event</span></span>
<span data-ttu-id="ab896-102">[event](../resources/event.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ab896-102">Get an [event](../resources/event.md) instance:</span></span>

## <a name="permissions"></a><span data-ttu-id="ab896-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab896-103">Permissions</span></span>
<span data-ttu-id="ab896-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab896-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab896-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab896-106">Permission type</span></span>      | <span data-ttu-id="ab896-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab896-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab896-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab896-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ab896-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab896-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab896-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab896-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab896-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab896-111">Not supported.</span></span>    |
|<span data-ttu-id="ab896-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab896-112">Application</span></span> | <span data-ttu-id="ab896-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab896-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab896-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab896-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab896-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ab896-115">Optional query parameters</span></span>
<span data-ttu-id="ab896-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ab896-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab896-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab896-117">Request headers</span></span>
| <span data-ttu-id="ab896-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab896-118">Header</span></span>       | <span data-ttu-id="ab896-119">値</span><span class="sxs-lookup"><span data-stu-id="ab896-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab896-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab896-120">Authorization</span></span>  | <span data-ttu-id="ab896-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab896-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab896-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab896-123">Request body</span></span>
<span data-ttu-id="ab896-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ab896-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab896-125">応答</span><span class="sxs-lookup"><span data-stu-id="ab896-125">Response</span></span>
<span data-ttu-id="ab896-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ab896-126">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab896-127">例</span><span class="sxs-lookup"><span data-stu-id="ab896-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ab896-128">要求</span><span class="sxs-lookup"><span data-stu-id="ab896-128">Request</span></span>
<span data-ttu-id="ab896-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab896-129">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="ab896-130">応答</span><span class="sxs-lookup"><span data-stu-id="ab896-130">Response</span></span>
<span data-ttu-id="ab896-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab896-131">The following is an example of a response.</span></span>
><span data-ttu-id="ab896-132">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ab896-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ab896-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ab896-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
