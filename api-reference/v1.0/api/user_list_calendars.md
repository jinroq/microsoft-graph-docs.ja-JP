# <a name="list-calendars"></a><span data-ttu-id="5ba7b-101">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5ba7b-101">List calendars</span></span>

<span data-ttu-id="5ba7b-102">すべてのユーザーの予定表を取得します (`/calendars` ナビゲーション プロパティ)。また既定の予定表グループまたは特定の予定表グループから予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-102">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="5ba7b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ba7b-103">Permissions</span></span>
<span data-ttu-id="5ba7b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ba7b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ba7b-106">Permission type</span></span>      | <span data-ttu-id="5ba7b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ba7b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ba7b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ba7b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5ba7b-109">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ba7b-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5ba7b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ba7b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ba7b-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ba7b-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5ba7b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ba7b-112">Application</span></span> | <span data-ttu-id="5ba7b-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ba7b-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ba7b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ba7b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5ba7b-115">すべてのユーザーの予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-115">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="5ba7b-116">既定の [calendarGroup](../resources/calendarGroup.md) のユーザーの予定表。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-116">The user's calendars in the default [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="5ba7b-117">特定の [calendarGroup](../resources/calendarGroup.md) のユーザーの予定表。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-117">The user's calendars in a specific [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ba7b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ba7b-118">Optional query parameters</span></span>
<span data-ttu-id="5ba7b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5ba7b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ba7b-120">Request headers</span></span>
| <span data-ttu-id="5ba7b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ba7b-121">Header</span></span>       | <span data-ttu-id="5ba7b-122">値</span><span class="sxs-lookup"><span data-stu-id="5ba7b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ba7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ba7b-123">Authorization</span></span>  | <span data-ttu-id="5ba7b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ba7b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ba7b-126">Content-Type</span></span>   | <span data-ttu-id="5ba7b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5ba7b-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ba7b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ba7b-128">Request body</span></span>
<span data-ttu-id="5ba7b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ba7b-130">応答</span><span class="sxs-lookup"><span data-stu-id="5ba7b-130">Response</span></span>

<span data-ttu-id="5ba7b-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Calendar](../resources/calendar.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-131">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ba7b-132">例</span><span class="sxs-lookup"><span data-stu-id="5ba7b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ba7b-133">要求</span><span class="sxs-lookup"><span data-stu-id="5ba7b-133">Request</span></span>
<span data-ttu-id="5ba7b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="5ba7b-135">応答</span><span class="sxs-lookup"><span data-stu-id="5ba7b-135">Response</span></span>
<span data-ttu-id="5ba7b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ba7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
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
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->