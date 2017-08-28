# <a name="delete-event"></a><span data-ttu-id="0ad45-101">イベントの削除</span><span class="sxs-lookup"><span data-stu-id="0ad45-101">Delete event</span></span>

<span data-ttu-id="0ad45-102">イベントを削除します。</span><span class="sxs-lookup"><span data-stu-id="0ad45-102">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ad45-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0ad45-103">Permissions</span></span>
<span data-ttu-id="0ad45-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ad45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ad45-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ad45-106">Permission type</span></span>      | <span data-ttu-id="0ad45-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ad45-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ad45-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ad45-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0ad45-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ad45-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ad45-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ad45-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ad45-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ad45-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ad45-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ad45-112">Application</span></span> | <span data-ttu-id="0ad45-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ad45-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ad45-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ad45-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0ad45-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ad45-115">Request headers</span></span>
| <span data-ttu-id="0ad45-116">名前</span><span class="sxs-lookup"><span data-stu-id="0ad45-116">Name</span></span>       | <span data-ttu-id="0ad45-117">型</span><span class="sxs-lookup"><span data-stu-id="0ad45-117">Type</span></span> | <span data-ttu-id="0ad45-118">説明</span><span class="sxs-lookup"><span data-stu-id="0ad45-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ad45-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ad45-119">Authorization</span></span>  | <span data-ttu-id="0ad45-120">string</span><span class="sxs-lookup"><span data-stu-id="0ad45-120">string</span></span>  | <span data-ttu-id="0ad45-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0ad45-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ad45-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ad45-123">Request body</span></span>
<span data-ttu-id="0ad45-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0ad45-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ad45-125">応答</span><span class="sxs-lookup"><span data-stu-id="0ad45-125">Response</span></span>

<span data-ttu-id="0ad45-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0ad45-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ad45-128">例</span><span class="sxs-lookup"><span data-stu-id="0ad45-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ad45-129">要求</span><span class="sxs-lookup"><span data-stu-id="0ad45-129">Request</span></span>
<span data-ttu-id="0ad45-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ad45-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="0ad45-131">応答</span><span class="sxs-lookup"><span data-stu-id="0ad45-131">Response</span></span>
<span data-ttu-id="0ad45-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0ad45-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
