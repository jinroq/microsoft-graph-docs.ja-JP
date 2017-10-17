# <a name="event-dismissreminder"></a><span data-ttu-id="8c44a-101">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="8c44a-101">event: dismissReminder</span></span>

<span data-ttu-id="8c44a-102">トリガーされたアラームを消します。</span><span class="sxs-lookup"><span data-stu-id="8c44a-102">Dismiss a reminder that has been triggered.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c44a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c44a-103">Permissions</span></span>
<span data-ttu-id="8c44a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c44a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c44a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c44a-106">Permission type</span></span>      | <span data-ttu-id="8c44a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c44a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c44a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c44a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8c44a-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c44a-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c44a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c44a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c44a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c44a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c44a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c44a-112">Application</span></span> | <span data-ttu-id="8c44a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c44a-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c44a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c44a-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder
POST /groups/{id}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder
POST /groups/{id}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="8c44a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c44a-115">Request headers</span></span>
| <span data-ttu-id="8c44a-116">名前</span><span class="sxs-lookup"><span data-stu-id="8c44a-116">Name</span></span>       | <span data-ttu-id="8c44a-117">型</span><span class="sxs-lookup"><span data-stu-id="8c44a-117">Type</span></span> | <span data-ttu-id="8c44a-118">説明</span><span class="sxs-lookup"><span data-stu-id="8c44a-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c44a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c44a-119">Authorization</span></span>  | <span data-ttu-id="8c44a-120">string</span><span class="sxs-lookup"><span data-stu-id="8c44a-120">string</span></span>  | <span data-ttu-id="8c44a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c44a-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="8c44a-123">応答</span><span class="sxs-lookup"><span data-stu-id="8c44a-123">Response</span></span>

<span data-ttu-id="8c44a-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8c44a-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c44a-126">例</span><span class="sxs-lookup"><span data-stu-id="8c44a-126">Example</span></span>

<span data-ttu-id="8c44a-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8c44a-127">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8c44a-128">要求</span><span class="sxs-lookup"><span data-stu-id="8c44a-128">Request</span></span>
<span data-ttu-id="8c44a-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c44a-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="8c44a-130">応答</span><span class="sxs-lookup"><span data-stu-id="8c44a-130">Response</span></span>
<span data-ttu-id="8c44a-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8c44a-131">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
