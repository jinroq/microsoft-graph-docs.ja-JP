# <a name="event-tentativelyaccept"></a><span data-ttu-id="145a7-101">イベント: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="145a7-101">event: tentativelyAccept</span></span>

<span data-ttu-id="145a7-102">指定したイベントを仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="145a7-102">Tentatively accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="145a7-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="145a7-103">Prerequisites</span></span>
<span data-ttu-id="145a7-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="145a7-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="145a7-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="145a7-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept
POST /groups/{id}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept
POST /groups/{id}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="145a7-106">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="145a7-106">Request headers</span></span>
| <span data-ttu-id="145a7-107">名前</span><span class="sxs-lookup"><span data-stu-id="145a7-107">Name</span></span>       | <span data-ttu-id="145a7-108">型</span><span class="sxs-lookup"><span data-stu-id="145a7-108">Type</span></span> | <span data-ttu-id="145a7-109">説明</span><span class="sxs-lookup"><span data-stu-id="145a7-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="145a7-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="145a7-110">Authorization</span></span>  | <span data-ttu-id="145a7-111">string</span><span class="sxs-lookup"><span data-stu-id="145a7-111">string</span></span>  | <span data-ttu-id="145a7-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="145a7-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="145a7-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="145a7-114">Content-Type</span></span> | <span data-ttu-id="145a7-115">string</span><span class="sxs-lookup"><span data-stu-id="145a7-115">string</span></span>  | <span data-ttu-id="145a7-p102">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="145a7-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="145a7-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="145a7-118">Request body</span></span>
<span data-ttu-id="145a7-119">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="145a7-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="145a7-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="145a7-120">Parameter</span></span>    | <span data-ttu-id="145a7-121">型</span><span class="sxs-lookup"><span data-stu-id="145a7-121">Type</span></span>   |<span data-ttu-id="145a7-122">説明</span><span class="sxs-lookup"><span data-stu-id="145a7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="145a7-123">comment</span><span class="sxs-lookup"><span data-stu-id="145a7-123">comment</span></span>|<span data-ttu-id="145a7-124">String</span><span class="sxs-lookup"><span data-stu-id="145a7-124">String</span></span>|<span data-ttu-id="145a7-p103">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="145a7-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="145a7-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="145a7-127">sendResponse</span></span>|<span data-ttu-id="145a7-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="145a7-128">Boolean</span></span>|<span data-ttu-id="145a7-p104">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="145a7-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="145a7-132">応答</span><span class="sxs-lookup"><span data-stu-id="145a7-132">Response</span></span>

<span data-ttu-id="145a7-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="145a7-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="145a7-135">例</span><span class="sxs-lookup"><span data-stu-id="145a7-135">Example</span></span>
<span data-ttu-id="145a7-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="145a7-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="145a7-137">要求</span><span class="sxs-lookup"><span data-stu-id="145a7-137">Request</span></span>
<span data-ttu-id="145a7-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="145a7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="145a7-139">応答</span><span class="sxs-lookup"><span data-stu-id="145a7-139">Response</span></span>
##### <a name="response"></a><span data-ttu-id="145a7-140">応答</span><span class="sxs-lookup"><span data-stu-id="145a7-140">Response</span></span>
<span data-ttu-id="145a7-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="145a7-141">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
