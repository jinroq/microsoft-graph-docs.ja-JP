# <a name="delete-calendar"></a><span data-ttu-id="0b4ac-101">Delete calendar</span><span class="sxs-lookup"><span data-stu-id="0b4ac-101">Delete calendar</span></span>

<span data-ttu-id="0b4ac-102">既定の予定表以外の予定を削除します。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-102">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b4ac-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b4ac-103">Permissions</span></span>
<span data-ttu-id="0b4ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0b4ac-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b4ac-106">Permission type</span></span>      | <span data-ttu-id="0b4ac-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b4ac-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b4ac-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b4ac-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0b4ac-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b4ac-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0b4ac-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b4ac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b4ac-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b4ac-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0b4ac-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b4ac-112">Application</span></span> | <span data-ttu-id="0b4ac-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b4ac-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b4ac-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b4ac-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0b4ac-115">既定 [calendarGroup](../resources/calendargroup.md) 内の既定の予定表以外のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-115">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="0b4ac-116">指定 [calendarGroup](../resources/calendargroup.md) 内の既定の予定表以外の [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-116">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0b4ac-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b4ac-117">Request headers</span></span>
| <span data-ttu-id="0b4ac-118">名前</span><span class="sxs-lookup"><span data-stu-id="0b4ac-118">Name</span></span>           |  <span data-ttu-id="0b4ac-119">型</span><span class="sxs-lookup"><span data-stu-id="0b4ac-119">Type</span></span>    | <span data-ttu-id="0b4ac-120">説明</span><span class="sxs-lookup"><span data-stu-id="0b4ac-120">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="0b4ac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b4ac-121">Authorization</span></span>  |  <span data-ttu-id="0b4ac-122">string</span><span class="sxs-lookup"><span data-stu-id="0b4ac-122">string</span></span>  | <span data-ttu-id="0b4ac-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b4ac-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b4ac-125">Request body</span></span>
<span data-ttu-id="0b4ac-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b4ac-127">応答</span><span class="sxs-lookup"><span data-stu-id="0b4ac-127">Response</span></span>

<span data-ttu-id="0b4ac-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b4ac-130">例</span><span class="sxs-lookup"><span data-stu-id="0b4ac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b4ac-131">要求</span><span class="sxs-lookup"><span data-stu-id="0b4ac-131">Request</span></span>
<span data-ttu-id="0b4ac-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="0b4ac-133">応答</span><span class="sxs-lookup"><span data-stu-id="0b4ac-133">Response</span></span>
<span data-ttu-id="0b4ac-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0b4ac-134">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
