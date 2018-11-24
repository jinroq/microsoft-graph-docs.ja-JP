# <a name="list-events"></a><span data-ttu-id="849fd-101">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="849fd-101">List events</span></span>

<span data-ttu-id="849fd-p101">予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="849fd-p101">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="849fd-104">拡張イベントのインスタンスを取得すると、[予定表ビューを取得する](calendar_list_calendarview.md)または[イベントのインスタンスを取得する](event_list_instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="849fd-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="849fd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="849fd-105">Permissions</span></span>
<span data-ttu-id="849fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="849fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="849fd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="849fd-108">Permission type</span></span>      | <span data-ttu-id="849fd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="849fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="849fd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="849fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="849fd-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="849fd-111">Calendars.Read</span></span>    |
|<span data-ttu-id="849fd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="849fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="849fd-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="849fd-113">Calendars.Read</span></span>    |
|<span data-ttu-id="849fd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="849fd-114">Application</span></span> | <span data-ttu-id="849fd-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="849fd-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="849fd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="849fd-116">HTTP request</span></span>
<span data-ttu-id="849fd-117"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="849fd-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="849fd-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="849fd-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="849fd-119">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="849fd-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="849fd-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="849fd-120">Optional query parameters</span></span>
<span data-ttu-id="849fd-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="849fd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="849fd-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="849fd-122">Request headers</span></span>
| <span data-ttu-id="849fd-123">名前</span><span class="sxs-lookup"><span data-stu-id="849fd-123">Name</span></span>       | <span data-ttu-id="849fd-124">型</span><span class="sxs-lookup"><span data-stu-id="849fd-124">Type</span></span> | <span data-ttu-id="849fd-125">説明</span><span class="sxs-lookup"><span data-stu-id="849fd-125">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="849fd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="849fd-126">Authorization</span></span>  | <span data-ttu-id="849fd-127">string</span><span class="sxs-lookup"><span data-stu-id="849fd-127">string</span></span> | <span data-ttu-id="849fd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="849fd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="849fd-130">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="849fd-130">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="849fd-131">string</span><span class="sxs-lookup"><span data-stu-id="849fd-131">string</span></span> | <span data-ttu-id="849fd-132">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="849fd-132">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="849fd-133">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="849fd-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="849fd-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="849fd-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="849fd-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="849fd-135">Request body</span></span>
<span data-ttu-id="849fd-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="849fd-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="849fd-137">応答</span><span class="sxs-lookup"><span data-stu-id="849fd-137">Response</span></span>

<span data-ttu-id="849fd-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="849fd-138">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="849fd-139">例</span><span class="sxs-lookup"><span data-stu-id="849fd-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="849fd-140">要求</span><span class="sxs-lookup"><span data-stu-id="849fd-140">Request</span></span>
<span data-ttu-id="849fd-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="849fd-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="849fd-142">応答</span><span class="sxs-lookup"><span data-stu-id="849fd-142">Response</span></span>
<span data-ttu-id="849fd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="849fd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
