# <a name="list-events"></a><span data-ttu-id="cd073-101">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd073-101">List events</span></span>
<span data-ttu-id="cd073-102">[イベント](../resources/event.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cd073-102">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd073-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cd073-103">Permissions</span></span>
<span data-ttu-id="cd073-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd073-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd073-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd073-106">Permission type</span></span>      | <span data-ttu-id="cd073-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd073-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd073-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd073-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cd073-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd073-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd073-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd073-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd073-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd073-111">Not supported.</span></span>    |
|<span data-ttu-id="cd073-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd073-112">Application</span></span> | <span data-ttu-id="cd073-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd073-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd073-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd073-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd073-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cd073-115">Optional query parameters</span></span>
<span data-ttu-id="cd073-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cd073-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd073-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd073-117">Request headers</span></span>
| <span data-ttu-id="cd073-118">名前</span><span class="sxs-lookup"><span data-stu-id="cd073-118">Name</span></span>       | <span data-ttu-id="cd073-119">型</span><span class="sxs-lookup"><span data-stu-id="cd073-119">Type</span></span> | <span data-ttu-id="cd073-120">説明</span><span class="sxs-lookup"><span data-stu-id="cd073-120">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="cd073-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd073-121">Authorization</span></span>  | <span data-ttu-id="cd073-122">string</span><span class="sxs-lookup"><span data-stu-id="cd073-122">string</span></span> | <span data-ttu-id="cd073-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cd073-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd073-125">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cd073-125">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="cd073-126">string</span><span class="sxs-lookup"><span data-stu-id="cd073-126">string</span></span> | <span data-ttu-id="cd073-127">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="cd073-127">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="cd073-128">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="cd073-128">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="cd073-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cd073-129">Optional.</span></span> |
| <span data-ttu-id="cd073-130">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="cd073-130">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="cd073-131">string</span><span class="sxs-lookup"><span data-stu-id="cd073-131">string</span></span> | <span data-ttu-id="cd073-132">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="cd073-132">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="cd073-133">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="cd073-133">Values can be "text" or "html".</span></span> <span data-ttu-id="cd073-134">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="cd073-134">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="cd073-135">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="cd073-135">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="cd073-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cd073-136">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd073-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd073-137">Request body</span></span>
<span data-ttu-id="cd073-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cd073-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd073-139">応答</span><span class="sxs-lookup"><span data-stu-id="cd073-139">Response</span></span>
<span data-ttu-id="cd073-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cd073-140">If successful, this method returns a `200 OK` response code and a collection of [Event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd073-141">例</span><span class="sxs-lookup"><span data-stu-id="cd073-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cd073-142">要求</span><span class="sxs-lookup"><span data-stu-id="cd073-142">Request</span></span>
<span data-ttu-id="cd073-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd073-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="cd073-144">応答</span><span class="sxs-lookup"><span data-stu-id="cd073-144">Response</span></span>
<span data-ttu-id="cd073-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd073-145">The following is an example of the response.</span></span>
><span data-ttu-id="cd073-146">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cd073-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cd073-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cd073-147">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
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
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
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
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
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
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
          }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
