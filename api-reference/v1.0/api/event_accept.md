# <a name="event-accept"></a><span data-ttu-id="1dd11-101">イベント: accept</span><span class="sxs-lookup"><span data-stu-id="1dd11-101">event: accept</span></span>

<span data-ttu-id="1dd11-102">ユーザーの[予定表](../resources/event.md)の指定[イベント](../resources/calendar.md)を承認します。</span><span class="sxs-lookup"><span data-stu-id="1dd11-102">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd11-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1dd11-103">Permissions</span></span>
<span data-ttu-id="1dd11-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dd11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1dd11-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dd11-106">Permission type</span></span>      | <span data-ttu-id="1dd11-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dd11-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd11-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dd11-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1dd11-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dd11-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1dd11-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dd11-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd11-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dd11-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1dd11-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dd11-112">Application</span></span> | <span data-ttu-id="1dd11-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dd11-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd11-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dd11-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="1dd11-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dd11-115">Request headers</span></span>
| <span data-ttu-id="1dd11-116">名前</span><span class="sxs-lookup"><span data-stu-id="1dd11-116">Name</span></span>       | <span data-ttu-id="1dd11-117">型</span><span class="sxs-lookup"><span data-stu-id="1dd11-117">Type</span></span> | <span data-ttu-id="1dd11-118">説明</span><span class="sxs-lookup"><span data-stu-id="1dd11-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1dd11-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dd11-119">Authorization</span></span>  | <span data-ttu-id="1dd11-120">文字列</span><span class="sxs-lookup"><span data-stu-id="1dd11-120">string</span></span>  | <span data-ttu-id="1dd11-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1dd11-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dd11-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1dd11-123">Content-Type</span></span> | <span data-ttu-id="1dd11-124">文字列</span><span class="sxs-lookup"><span data-stu-id="1dd11-124">string</span></span>  | <span data-ttu-id="1dd11-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="1dd11-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dd11-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dd11-127">Request body</span></span>
<span data-ttu-id="1dd11-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1dd11-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1dd11-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1dd11-129">Parameter</span></span>    | <span data-ttu-id="1dd11-130">型</span><span class="sxs-lookup"><span data-stu-id="1dd11-130">Type</span></span>   |<span data-ttu-id="1dd11-131">説明</span><span class="sxs-lookup"><span data-stu-id="1dd11-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd11-132">comment</span><span class="sxs-lookup"><span data-stu-id="1dd11-132">comment</span></span>|<span data-ttu-id="1dd11-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1dd11-133">String</span></span>|<span data-ttu-id="1dd11-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="1dd11-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="1dd11-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="1dd11-136">sendResponse</span></span>|<span data-ttu-id="1dd11-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="1dd11-137">Boolean</span></span>|<span data-ttu-id="1dd11-p105">`true` 応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="1dd11-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="1dd11-141">応答</span><span class="sxs-lookup"><span data-stu-id="1dd11-141">Response</span></span>

<span data-ttu-id="1dd11-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1dd11-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd11-144">例</span><span class="sxs-lookup"><span data-stu-id="1dd11-144">Example</span></span>
<span data-ttu-id="1dd11-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1dd11-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1dd11-146">要求</span><span class="sxs-lookup"><span data-stu-id="1dd11-146">Request</span></span>
<span data-ttu-id="1dd11-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dd11-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1dd11-148">応答</span><span class="sxs-lookup"><span data-stu-id="1dd11-148">Response</span></span>
<span data-ttu-id="1dd11-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1dd11-149">Here is an example of the response.</span></span>
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
