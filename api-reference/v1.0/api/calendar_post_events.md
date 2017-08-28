# <a name="create-event"></a><span data-ttu-id="4aac0-101">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="4aac0-101">Create Event</span></span>

<span data-ttu-id="4aac0-102">この API を使用して、既定または指定の予定表に新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="4aac0-102">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="4aac0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4aac0-103">Permissions</span></span>
<span data-ttu-id="4aac0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4aac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4aac0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4aac0-106">Permission type</span></span>      | <span data-ttu-id="4aac0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4aac0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aac0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4aac0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4aac0-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aac0-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4aac0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4aac0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aac0-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aac0-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4aac0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4aac0-112">Application</span></span> | <span data-ttu-id="4aac0-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aac0-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aac0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4aac0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4aac0-115">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="4aac0-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="4aac0-116">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="4aac0-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="4aac0-117">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="4aac0-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="4aac0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4aac0-118">Request headers</span></span>
| <span data-ttu-id="4aac0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4aac0-119">Header</span></span>       | <span data-ttu-id="4aac0-120">値</span><span class="sxs-lookup"><span data-stu-id="4aac0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4aac0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aac0-121">Authorization</span></span>  | <span data-ttu-id="4aac0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4aac0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4aac0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aac0-124">Content-Type</span></span>  | <span data-ttu-id="4aac0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4aac0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4aac0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4aac0-127">Request body</span></span>
<span data-ttu-id="4aac0-128">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4aac0-128">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4aac0-129">応答</span><span class="sxs-lookup"><span data-stu-id="4aac0-129">Response</span></span>

<span data-ttu-id="4aac0-130">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4aac0-130">If successful, this method returns `201, Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aac0-131">例</span><span class="sxs-lookup"><span data-stu-id="4aac0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aac0-132">要求</span><span class="sxs-lookup"><span data-stu-id="4aac0-132">Request</span></span>
<span data-ttu-id="4aac0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4aac0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="4aac0-134">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4aac0-134">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4aac0-135">応答</span><span class="sxs-lookup"><span data-stu-id="4aac0-135">Response</span></span>
<span data-ttu-id="4aac0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4aac0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
