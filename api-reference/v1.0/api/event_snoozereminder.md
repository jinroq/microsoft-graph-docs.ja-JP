# <a name="event-snoozereminder"></a><span data-ttu-id="85316-101">イベント: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="85316-101">event: snoozeReminder</span></span>

<span data-ttu-id="85316-102">新しい時刻まで、アラームを延期します。</span><span class="sxs-lookup"><span data-stu-id="85316-102">Postpone a reminder until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="85316-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85316-103">Permissions</span></span>
<span data-ttu-id="85316-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="85316-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85316-106">Permission type</span></span>      | <span data-ttu-id="85316-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85316-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85316-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85316-108">Delegated (work or school account)</span></span> | <span data-ttu-id="85316-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85316-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="85316-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85316-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85316-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85316-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="85316-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85316-112">Application</span></span> | <span data-ttu-id="85316-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85316-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="85316-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85316-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder
POST /groups/{id}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder
POST /groups/{id}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="85316-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85316-115">Request headers</span></span>
| <span data-ttu-id="85316-116">名前</span><span class="sxs-lookup"><span data-stu-id="85316-116">Name</span></span>       | <span data-ttu-id="85316-117">型</span><span class="sxs-lookup"><span data-stu-id="85316-117">Type</span></span> | <span data-ttu-id="85316-118">説明</span><span class="sxs-lookup"><span data-stu-id="85316-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85316-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="85316-119">Authorization</span></span>  | <span data-ttu-id="85316-120">string</span><span class="sxs-lookup"><span data-stu-id="85316-120">string</span></span>  | <span data-ttu-id="85316-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85316-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85316-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85316-123">Content-Type</span></span> | <span data-ttu-id="85316-124">string</span><span class="sxs-lookup"><span data-stu-id="85316-124">string</span></span>  | <span data-ttu-id="85316-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="85316-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85316-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="85316-127">Request body</span></span>
<span data-ttu-id="85316-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="85316-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85316-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="85316-129">Parameter</span></span>    | <span data-ttu-id="85316-130">型</span><span class="sxs-lookup"><span data-stu-id="85316-130">Type</span></span>   |<span data-ttu-id="85316-131">説明</span><span class="sxs-lookup"><span data-stu-id="85316-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85316-132">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="85316-132">newReminderTime</span></span>|<span data-ttu-id="85316-133">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="85316-133">DateTimeTimeZone</span></span>|<span data-ttu-id="85316-134">アラームをトリガーする新しい日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="85316-134">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="85316-135">応答</span><span class="sxs-lookup"><span data-stu-id="85316-135">Response</span></span>

<span data-ttu-id="85316-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="85316-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85316-138">例</span><span class="sxs-lookup"><span data-stu-id="85316-138">Example</span></span>
<span data-ttu-id="85316-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="85316-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85316-140">要求</span><span class="sxs-lookup"><span data-stu-id="85316-140">Request</span></span>
<span data-ttu-id="85316-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85316-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="85316-142">応答</span><span class="sxs-lookup"><span data-stu-id="85316-142">Response</span></span>
<span data-ttu-id="85316-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="85316-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
