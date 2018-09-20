# <a name="get-calendar"></a><span data-ttu-id="fae0c-101">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="fae0c-101">Get calendar</span></span>

<span data-ttu-id="fae0c-102">[予定表](../resources/calendar.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="fae0c-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="fae0c-103">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="fae0c-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="fae0c-104">アプリが別のユーザーの予定表を取得できる 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="fae0c-104">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="fae0c-105">このアプリにアプリケーションのアクセス許可がある場合、または、</span><span class="sxs-lookup"><span data-stu-id="fae0c-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="fae0c-106">このアプリに、1 人のユーザーから適切な[アクセス許可](#permissions)が委任され、別のユーザーは、そのユーザーと予定表を共有しているか、またはそのユーザーにアクセスを委任しているかする場合。</span><span class="sxs-lookup"><span data-stu-id="fae0c-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="fae0c-107"> [詳細と例](../../../concepts/outlook-get-shared-events-calendars.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fae0c-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fae0c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fae0c-108">Permissions</span></span>
<span data-ttu-id="fae0c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fae0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fae0c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fae0c-111">Permission type</span></span>      | <span data-ttu-id="fae0c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fae0c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fae0c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fae0c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fae0c-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fae0c-114">Calendars.Read</span></span>    |
|<span data-ttu-id="fae0c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fae0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fae0c-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fae0c-116">Calendars.Read</span></span>    |
|<span data-ttu-id="fae0c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fae0c-117">Application</span></span> | <span data-ttu-id="fae0c-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fae0c-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="fae0c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fae0c-119">HTTP request</span></span>
<span data-ttu-id="fae0c-120"><!-- { "blockType": "ignored" } --> ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="fae0c-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="fae0c-121">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="fae0c-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="fae0c-122">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="fae0c-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fae0c-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fae0c-123">Optional query parameters</span></span>
<span data-ttu-id="fae0c-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fae0c-124">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fae0c-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fae0c-125">Request headers</span></span>
| <span data-ttu-id="fae0c-126">名前</span><span class="sxs-lookup"><span data-stu-id="fae0c-126">Name</span></span>       | <span data-ttu-id="fae0c-127">型</span><span class="sxs-lookup"><span data-stu-id="fae0c-127">Type</span></span> | <span data-ttu-id="fae0c-128">説明</span><span class="sxs-lookup"><span data-stu-id="fae0c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fae0c-129">承認</span><span class="sxs-lookup"><span data-stu-id="fae0c-129">Authorization</span></span>  | <span data-ttu-id="fae0c-130">文字列</span><span class="sxs-lookup"><span data-stu-id="fae0c-130">string</span></span>  | <span data-ttu-id="fae0c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fae0c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fae0c-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="fae0c-133">Request body</span></span>
<span data-ttu-id="fae0c-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fae0c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fae0c-135">応答</span><span class="sxs-lookup"><span data-stu-id="fae0c-135">Response</span></span>

<span data-ttu-id="fae0c-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fae0c-136">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fae0c-137">例</span><span class="sxs-lookup"><span data-stu-id="fae0c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fae0c-138">要求</span><span class="sxs-lookup"><span data-stu-id="fae0c-138">Request</span></span>
<span data-ttu-id="fae0c-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fae0c-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="fae0c-140">応答</span><span class="sxs-lookup"><span data-stu-id="fae0c-140">Response</span></span>
<span data-ttu-id="fae0c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fae0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
