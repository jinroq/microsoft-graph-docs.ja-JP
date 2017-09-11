# <a name="get-calendar"></a><span data-ttu-id="e11b0-101">Get calendar</span><span class="sxs-lookup"><span data-stu-id="e11b0-101">Get calendar</span></span>

<span data-ttu-id="e11b0-102">予定表オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e11b0-102">Retrieve the properties and relationships of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e11b0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e11b0-103">Permissions</span></span>
<span data-ttu-id="e11b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e11b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e11b0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e11b0-106">Permission type</span></span>      | <span data-ttu-id="e11b0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e11b0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e11b0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e11b0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e11b0-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e11b0-109">Calendars.Read</span></span>    |
|<span data-ttu-id="e11b0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e11b0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e11b0-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e11b0-111">Calendars.Read</span></span>    |
|<span data-ttu-id="e11b0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e11b0-112">Application</span></span> | <span data-ttu-id="e11b0-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e11b0-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e11b0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e11b0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e11b0-115">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="e11b0-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="e11b0-116">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="e11b0-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="e11b0-117">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="e11b0-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e11b0-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e11b0-118">Optional query parameters</span></span>
<span data-ttu-id="e11b0-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e11b0-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e11b0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e11b0-120">Request headers</span></span>
| <span data-ttu-id="e11b0-121">名前</span><span class="sxs-lookup"><span data-stu-id="e11b0-121">Name</span></span>       | <span data-ttu-id="e11b0-122">型</span><span class="sxs-lookup"><span data-stu-id="e11b0-122">Type</span></span> | <span data-ttu-id="e11b0-123">説明</span><span class="sxs-lookup"><span data-stu-id="e11b0-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e11b0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e11b0-124">Authorization</span></span>  | <span data-ttu-id="e11b0-125">string</span><span class="sxs-lookup"><span data-stu-id="e11b0-125">string</span></span>  | <span data-ttu-id="e11b0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e11b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e11b0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e11b0-128">Request body</span></span>
<span data-ttu-id="e11b0-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e11b0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e11b0-130">応答</span><span class="sxs-lookup"><span data-stu-id="e11b0-130">Response</span></span>

<span data-ttu-id="e11b0-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e11b0-131">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e11b0-132">例</span><span class="sxs-lookup"><span data-stu-id="e11b0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e11b0-133">要求</span><span class="sxs-lookup"><span data-stu-id="e11b0-133">Request</span></span>
<span data-ttu-id="e11b0-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e11b0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="e11b0-135">応答</span><span class="sxs-lookup"><span data-stu-id="e11b0-135">Response</span></span>
<span data-ttu-id="e11b0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e11b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
