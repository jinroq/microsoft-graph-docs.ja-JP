# <a name="event-decline"></a><span data-ttu-id="8a65d-101">イベント: 辞退</span><span class="sxs-lookup"><span data-stu-id="8a65d-101">event: decline</span></span>

<span data-ttu-id="8a65d-102">ユーザーの [予定表](../resources/event.md) で指定した[イベント](../resources/calendar.md)への招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="8a65d-102">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a65d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a65d-103">Permissions</span></span>

<span data-ttu-id="8a65d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a65d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a65d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a65d-106">Permission type</span></span>      | <span data-ttu-id="8a65d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a65d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a65d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a65d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8a65d-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a65d-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8a65d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a65d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a65d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a65d-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8a65d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a65d-112">Application</span></span> | <span data-ttu-id="8a65d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a65d-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a65d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a65d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="8a65d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a65d-115">Request headers</span></span>

| <span data-ttu-id="8a65d-116">名前</span><span class="sxs-lookup"><span data-stu-id="8a65d-116">Name</span></span>       | <span data-ttu-id="8a65d-117">型</span><span class="sxs-lookup"><span data-stu-id="8a65d-117">Type</span></span> | <span data-ttu-id="8a65d-118">説明</span><span class="sxs-lookup"><span data-stu-id="8a65d-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a65d-119">承認</span><span class="sxs-lookup"><span data-stu-id="8a65d-119">Authorization</span></span>  | <span data-ttu-id="8a65d-120">文字列</span><span class="sxs-lookup"><span data-stu-id="8a65d-120">string</span></span>  | <span data-ttu-id="8a65d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a65d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a65d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a65d-123">Content-Type</span></span> | <span data-ttu-id="8a65d-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8a65d-124">string</span></span>  | <span data-ttu-id="8a65d-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="8a65d-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a65d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a65d-127">Request body</span></span>

<span data-ttu-id="8a65d-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a65d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a65d-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a65d-129">Parameter</span></span>    | <span data-ttu-id="8a65d-130">型</span><span class="sxs-lookup"><span data-stu-id="8a65d-130">Type</span></span>   |<span data-ttu-id="8a65d-131">説明</span><span class="sxs-lookup"><span data-stu-id="8a65d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a65d-132">コメント</span><span class="sxs-lookup"><span data-stu-id="8a65d-132">comment</span></span>|<span data-ttu-id="8a65d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8a65d-133">String</span></span>|<span data-ttu-id="8a65d-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="8a65d-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="8a65d-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="8a65d-136">sendResponse</span></span>|<span data-ttu-id="8a65d-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="8a65d-137">Boolean</span></span>|<span data-ttu-id="8a65d-p105">`true` 応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="8a65d-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="8a65d-141">応答</span><span class="sxs-lookup"><span data-stu-id="8a65d-141">Response</span></span>

<span data-ttu-id="8a65d-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8a65d-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a65d-144">例</span><span class="sxs-lookup"><span data-stu-id="8a65d-144">Example</span></span>

<span data-ttu-id="8a65d-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8a65d-145">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8a65d-146">要求</span><span class="sxs-lookup"><span data-stu-id="8a65d-146">Request</span></span>

<span data-ttu-id="8a65d-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a65d-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

<br/>

### <a name="response"></a><span data-ttu-id="8a65d-148">応答</span><span class="sxs-lookup"><span data-stu-id="8a65d-148">Response</span></span>

<span data-ttu-id="8a65d-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8a65d-149">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
