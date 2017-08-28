# <a name="create-calendar"></a><span data-ttu-id="cb6eb-101">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="cb6eb-101">Create Calendar</span></span>

<span data-ttu-id="cb6eb-102">この API を使って、予定表グループに新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-102">Use this API to create a new Calendar in a calendar group.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb6eb-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb6eb-103">Permissions</span></span>
<span data-ttu-id="cb6eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb6eb-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb6eb-106">Permission type</span></span>      | <span data-ttu-id="cb6eb-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb6eb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb6eb-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb6eb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cb6eb-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb6eb-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cb6eb-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb6eb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb6eb-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb6eb-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cb6eb-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb6eb-112">Application</span></span> | <span data-ttu-id="cb6eb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb6eb-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb6eb-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb6eb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cb6eb-115">ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```
<span data-ttu-id="cb6eb-116">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="cb6eb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb6eb-117">Request headers</span></span>
| <span data-ttu-id="cb6eb-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb6eb-118">Header</span></span>       | <span data-ttu-id="cb6eb-119">値</span><span class="sxs-lookup"><span data-stu-id="cb6eb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb6eb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb6eb-120">Authorization</span></span>  | <span data-ttu-id="cb6eb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb6eb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb6eb-123">Content-Type</span></span>  | <span data-ttu-id="cb6eb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cb6eb-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb6eb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb6eb-126">Request body</span></span>
<span data-ttu-id="cb6eb-127">要求本文で、[予定表](../resources/calendar.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-127">In the request body, supply a JSON representation of [Calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cb6eb-128">応答</span><span class="sxs-lookup"><span data-stu-id="cb6eb-128">Response</span></span>

<span data-ttu-id="cb6eb-129">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-129">If successful, this method returns `201, Created` response code and [Calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb6eb-130">例</span><span class="sxs-lookup"><span data-stu-id="cb6eb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb6eb-131">要求</span><span class="sxs-lookup"><span data-stu-id="cb6eb-131">Request</span></span>
<span data-ttu-id="cb6eb-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```
<span data-ttu-id="cb6eb-133">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-133">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cb6eb-134">応答</span><span class="sxs-lookup"><span data-stu-id="cb6eb-134">Response</span></span>
<span data-ttu-id="cb6eb-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb6eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
