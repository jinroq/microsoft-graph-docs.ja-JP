# <a name="get-calendar"></a><span data-ttu-id="65064-101">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="65064-101">Get calendar</span></span>

<span data-ttu-id="65064-102">[予定表](../resources/calendar.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="65064-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="65064-103">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="65064-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="65064-104">アプリケーションが別のユーザーの予定表を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="65064-104">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="65064-105">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="65064-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="65064-106">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーとカレンダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="65064-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="65064-107">[詳細と例](../../../concepts/outlook-get-shared-events-calendars.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65064-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65064-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65064-108">Permissions</span></span>
<span data-ttu-id="65064-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65064-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65064-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65064-111">Permission type</span></span>      | <span data-ttu-id="65064-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65064-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65064-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65064-113">Delegated (work or school account)</span></span> | <span data-ttu-id="65064-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="65064-114">Calendars.Read</span></span>    |
|<span data-ttu-id="65064-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65064-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65064-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="65064-116">Calendars.Read</span></span>    |
|<span data-ttu-id="65064-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65064-117">Application</span></span> | <span data-ttu-id="65064-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="65064-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="65064-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65064-119">HTTP request</span></span>
<span data-ttu-id="65064-120"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="65064-120"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="65064-121">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="65064-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="65064-122">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="65064-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65064-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="65064-123">Optional query parameters</span></span>
<span data-ttu-id="65064-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="65064-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="65064-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65064-125">Request headers</span></span>
| <span data-ttu-id="65064-126">名前</span><span class="sxs-lookup"><span data-stu-id="65064-126">Name</span></span>       | <span data-ttu-id="65064-127">型</span><span class="sxs-lookup"><span data-stu-id="65064-127">Type</span></span> | <span data-ttu-id="65064-128">説明</span><span class="sxs-lookup"><span data-stu-id="65064-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65064-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="65064-129">Authorization</span></span>  | <span data-ttu-id="65064-130">string</span><span class="sxs-lookup"><span data-stu-id="65064-130">string</span></span>  | <span data-ttu-id="65064-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65064-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65064-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="65064-133">Request body</span></span>
<span data-ttu-id="65064-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65064-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65064-135">応答</span><span class="sxs-lookup"><span data-stu-id="65064-135">Response</span></span>

<span data-ttu-id="65064-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65064-136">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65064-137">例</span><span class="sxs-lookup"><span data-stu-id="65064-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65064-138">要求</span><span class="sxs-lookup"><span data-stu-id="65064-138">Request</span></span>
<span data-ttu-id="65064-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65064-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="65064-140">応答</span><span class="sxs-lookup"><span data-stu-id="65064-140">Response</span></span>
<span data-ttu-id="65064-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65064-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
