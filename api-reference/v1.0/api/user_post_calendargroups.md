# <a name="create-calendargroup"></a><span data-ttu-id="d2b4a-101">CalendarGroup を作成する　</span><span class="sxs-lookup"><span data-stu-id="d2b4a-101">Create CalendarGroup</span></span>

<span data-ttu-id="d2b4a-102">この API を使用して、新しい CalendarGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-102">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2b4a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2b4a-103">Permissions</span></span>
<span data-ttu-id="d2b4a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2b4a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2b4a-106">Permission type</span></span>      | <span data-ttu-id="d2b4a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2b4a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2b4a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2b4a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d2b4a-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2b4a-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d2b4a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2b4a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2b4a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2b4a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d2b4a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2b4a-112">Application</span></span> | <span data-ttu-id="d2b4a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2b4a-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2b4a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2b4a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="d2b4a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2b4a-115">Request headers</span></span>
| <span data-ttu-id="d2b4a-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2b4a-116">Header</span></span>       | <span data-ttu-id="d2b4a-117">値</span><span class="sxs-lookup"><span data-stu-id="d2b4a-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2b4a-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2b4a-118">Authorization</span></span>  | <span data-ttu-id="d2b4a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2b4a-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2b4a-121">Content-Type</span></span>  | <span data-ttu-id="d2b4a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2b4a-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2b4a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2b4a-123">Request body</span></span>
<span data-ttu-id="d2b4a-124">要求本文で、[CalendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-124">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d2b4a-125">応答</span><span class="sxs-lookup"><span data-stu-id="d2b4a-125">Response</span></span>

<span data-ttu-id="d2b4a-126">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-126">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b4a-127">例</span><span class="sxs-lookup"><span data-stu-id="d2b4a-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2b4a-128">要求</span><span class="sxs-lookup"><span data-stu-id="d2b4a-128">Request</span></span>
<span data-ttu-id="d2b4a-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="d2b4a-130">要求本文で、[calendarGroup](../resources/calendargroup.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-130">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d2b4a-131">応答</span><span class="sxs-lookup"><span data-stu-id="d2b4a-131">Response</span></span>
<span data-ttu-id="d2b4a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2b4a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
