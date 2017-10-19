# <a name="get-calendar"></a><span data-ttu-id="b02c4-101">Get calendar</span><span class="sxs-lookup"><span data-stu-id="b02c4-101">Get calendar</span></span>

<span data-ttu-id="b02c4-102">予定表オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b02c4-102">Retrieve the properties and relationships of calendar object.</span></span>


### <a name="get-another-users-calendar"></a><span data-ttu-id="b02c4-103">別のユーザーの予定表の取得</span><span class="sxs-lookup"><span data-stu-id="b02c4-103">Get another user's drive</span></span>

<span data-ttu-id="b02c4-104">アプリケーションのアクセス許可がある場合や、1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合には、別のユーザーの予定表を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get a calendar of another user's.</span></span> <span data-ttu-id="b02c4-105">このセクションでは、委任されたアクセス許可に関連するシナリオに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="b02c4-106">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="b02c4-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="b02c4-107">別のユーザー Garth は、John と予定表を共有しています。</span><span class="sxs-lookup"><span data-stu-id="b02c4-107">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="b02c4-108">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有の予定表を取得できます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-108">You can get that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="b02c4-109">この機能は、以下の [HTTP 要求](#http-request)セクションで記載されているように、個々のユーザーに対しサポートされているすべての連絡先の予定表の取得操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-109">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="b02c4-110">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="b02c4-111">Garth が John と予定表を共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-111">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="b02c4-112">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身の予定表を取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="b02c4-112">In such cases, specifying a user ID or user principal name only works for getting a calendar of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar
```

<span data-ttu-id="b02c4-113">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="b02c4-114">共有の連絡先フォルダー</span><span class="sxs-lookup"><span data-stu-id="b02c4-114">Shared contact folders</span></span>
- <span data-ttu-id="b02c4-115">共有の予定表</span><span class="sxs-lookup"><span data-stu-id="b02c4-115">Shared calendars</span></span>
- <span data-ttu-id="b02c4-116">共有フォルダー内の連絡先およびイベント</span><span class="sxs-lookup"><span data-stu-id="b02c4-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="b02c4-117">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="b02c4-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="b02c4-118">この機能は、連絡先、イベント、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="b02c4-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="b02c4-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b02c4-119">Permissions</span></span>
<span data-ttu-id="b02c4-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b02c4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b02c4-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b02c4-122">Permission type</span></span>      | <span data-ttu-id="b02c4-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b02c4-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b02c4-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b02c4-124">Delegated (work or school account)</span></span> | <span data-ttu-id="b02c4-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b02c4-125">Calendars.Read</span></span>    |
|<span data-ttu-id="b02c4-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b02c4-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b02c4-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b02c4-127">Calendars.Read</span></span>    |
|<span data-ttu-id="b02c4-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b02c4-128">Application</span></span> | <span data-ttu-id="b02c4-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b02c4-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b02c4-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b02c4-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b02c4-131">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b02c4-131">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="b02c4-132">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b02c4-132">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="b02c4-133">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b02c4-133">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b02c4-134">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b02c4-134">Optional query parameters</span></span>
<span data-ttu-id="b02c4-135">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b02c4-135">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b02c4-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b02c4-136">Request headers</span></span>
| <span data-ttu-id="b02c4-137">名前</span><span class="sxs-lookup"><span data-stu-id="b02c4-137">Name</span></span>       | <span data-ttu-id="b02c4-138">型</span><span class="sxs-lookup"><span data-stu-id="b02c4-138">Type</span></span> | <span data-ttu-id="b02c4-139">説明</span><span class="sxs-lookup"><span data-stu-id="b02c4-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b02c4-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="b02c4-140">Authorization</span></span>  | <span data-ttu-id="b02c4-141">string</span><span class="sxs-lookup"><span data-stu-id="b02c4-141">string</span></span>  | <span data-ttu-id="b02c4-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b02c4-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b02c4-144">要求本文</span><span class="sxs-lookup"><span data-stu-id="b02c4-144">Request body</span></span>
<span data-ttu-id="b02c4-145">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b02c4-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b02c4-146">応答</span><span class="sxs-lookup"><span data-stu-id="b02c4-146">Response</span></span>

<span data-ttu-id="b02c4-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b02c4-147">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b02c4-148">例</span><span class="sxs-lookup"><span data-stu-id="b02c4-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b02c4-149">要求</span><span class="sxs-lookup"><span data-stu-id="b02c4-149">Request</span></span>
<span data-ttu-id="b02c4-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b02c4-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="b02c4-151">応答</span><span class="sxs-lookup"><span data-stu-id="b02c4-151">Response</span></span>
<span data-ttu-id="b02c4-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b02c4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
