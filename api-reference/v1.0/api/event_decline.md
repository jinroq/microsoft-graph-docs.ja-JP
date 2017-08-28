# <a name="event-decline"></a><span data-ttu-id="8f97a-101">イベント: 辞退</span><span class="sxs-lookup"><span data-stu-id="8f97a-101">event: decline</span></span>

<span data-ttu-id="8f97a-102">指定したイベントへの招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="8f97a-102">Decline invitation to the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f97a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f97a-103">Permissions</span></span>
<span data-ttu-id="8f97a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f97a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8f97a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f97a-106">Permission type</span></span>      | <span data-ttu-id="8f97a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f97a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f97a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f97a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8f97a-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f97a-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8f97a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f97a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f97a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f97a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8f97a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f97a-112">Application</span></span> | <span data-ttu-id="8f97a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f97a-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f97a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f97a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline
POST /groups/{id}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline
POST /groups/{id}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```
## <a name="request-headers"></a><span data-ttu-id="8f97a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f97a-115">Request headers</span></span>
| <span data-ttu-id="8f97a-116">名前</span><span class="sxs-lookup"><span data-stu-id="8f97a-116">Name</span></span>       | <span data-ttu-id="8f97a-117">型</span><span class="sxs-lookup"><span data-stu-id="8f97a-117">Type</span></span> | <span data-ttu-id="8f97a-118">説明</span><span class="sxs-lookup"><span data-stu-id="8f97a-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8f97a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f97a-119">Authorization</span></span>  | <span data-ttu-id="8f97a-120">string</span><span class="sxs-lookup"><span data-stu-id="8f97a-120">string</span></span>  | <span data-ttu-id="8f97a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8f97a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f97a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f97a-123">Content-Type</span></span> | <span data-ttu-id="8f97a-124">string</span><span class="sxs-lookup"><span data-stu-id="8f97a-124">string</span></span>  | <span data-ttu-id="8f97a-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="8f97a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f97a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f97a-127">Request body</span></span>
<span data-ttu-id="8f97a-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8f97a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f97a-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f97a-129">Parameter</span></span>    | <span data-ttu-id="8f97a-130">型</span><span class="sxs-lookup"><span data-stu-id="8f97a-130">Type</span></span>   |<span data-ttu-id="8f97a-131">説明</span><span class="sxs-lookup"><span data-stu-id="8f97a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f97a-132">comment</span><span class="sxs-lookup"><span data-stu-id="8f97a-132">comment</span></span>|<span data-ttu-id="8f97a-133">String</span><span class="sxs-lookup"><span data-stu-id="8f97a-133">String</span></span>|<span data-ttu-id="8f97a-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="8f97a-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="8f97a-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="8f97a-136">sendResponse</span></span>|<span data-ttu-id="8f97a-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="8f97a-137">Boolean</span></span>|<span data-ttu-id="8f97a-p105">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="8f97a-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="8f97a-141">応答</span><span class="sxs-lookup"><span data-stu-id="8f97a-141">Response</span></span>

<span data-ttu-id="8f97a-p106">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8f97a-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f97a-144">例</span><span class="sxs-lookup"><span data-stu-id="8f97a-144">Example</span></span>
<span data-ttu-id="8f97a-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8f97a-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f97a-146">要求</span><span class="sxs-lookup"><span data-stu-id="8f97a-146">Request</span></span>
<span data-ttu-id="8f97a-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f97a-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8f97a-148">応答</span><span class="sxs-lookup"><span data-stu-id="8f97a-148">Response</span></span>
##### <a name="response"></a><span data-ttu-id="8f97a-149">応答</span><span class="sxs-lookup"><span data-stu-id="8f97a-149">Response</span></span>
<span data-ttu-id="8f97a-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8f97a-150">Here is an example of the response.</span></span>
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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
