# <a name="event-accept"></a><span data-ttu-id="fde94-101">イベント: 承諾</span><span class="sxs-lookup"><span data-stu-id="fde94-101">event: accept</span></span>

<span data-ttu-id="fde94-102">指定したイベントを承諾します。</span><span class="sxs-lookup"><span data-stu-id="fde94-102">Accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fde94-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="fde94-103">Prerequisites</span></span>
<span data-ttu-id="fde94-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="fde94-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="fde94-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fde94-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept
POST /groups/{id}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept
POST /groups/{id}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="fde94-106">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fde94-106">Request headers</span></span>
| <span data-ttu-id="fde94-107">名前</span><span class="sxs-lookup"><span data-stu-id="fde94-107">Name</span></span>       | <span data-ttu-id="fde94-108">型</span><span class="sxs-lookup"><span data-stu-id="fde94-108">Type</span></span> | <span data-ttu-id="fde94-109">説明</span><span class="sxs-lookup"><span data-stu-id="fde94-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fde94-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="fde94-110">Authorization</span></span>  | <span data-ttu-id="fde94-111">string</span><span class="sxs-lookup"><span data-stu-id="fde94-111">string</span></span>  | <span data-ttu-id="fde94-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fde94-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fde94-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fde94-114">Content-Type</span></span> | <span data-ttu-id="fde94-115">string</span><span class="sxs-lookup"><span data-stu-id="fde94-115">string</span></span>  | <span data-ttu-id="fde94-p102">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="fde94-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fde94-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="fde94-118">Request body</span></span>
<span data-ttu-id="fde94-119">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fde94-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fde94-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fde94-120">Parameter</span></span>    | <span data-ttu-id="fde94-121">型</span><span class="sxs-lookup"><span data-stu-id="fde94-121">Type</span></span>   |<span data-ttu-id="fde94-122">説明</span><span class="sxs-lookup"><span data-stu-id="fde94-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fde94-123">comment</span><span class="sxs-lookup"><span data-stu-id="fde94-123">comment</span></span>|<span data-ttu-id="fde94-124">String</span><span class="sxs-lookup"><span data-stu-id="fde94-124">String</span></span>|<span data-ttu-id="fde94-p103">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="fde94-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="fde94-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="fde94-127">sendResponse</span></span>|<span data-ttu-id="fde94-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="fde94-128">Boolean</span></span>|<span data-ttu-id="fde94-p104">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="fde94-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="fde94-132">応答</span><span class="sxs-lookup"><span data-stu-id="fde94-132">Response</span></span>

<span data-ttu-id="fde94-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fde94-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fde94-135">例</span><span class="sxs-lookup"><span data-stu-id="fde94-135">Example</span></span>
<span data-ttu-id="fde94-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fde94-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fde94-137">要求</span><span class="sxs-lookup"><span data-stu-id="fde94-137">Request</span></span>
<span data-ttu-id="fde94-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fde94-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="fde94-139">応答</span><span class="sxs-lookup"><span data-stu-id="fde94-139">Response</span></span>
<span data-ttu-id="fde94-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fde94-140">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
