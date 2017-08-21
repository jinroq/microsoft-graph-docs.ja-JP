# <a name="create-calendar"></a><span data-ttu-id="f9cda-101">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="f9cda-101">Create Calendar</span></span>

<span data-ttu-id="f9cda-102">この API を使用して、新しい予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="f9cda-102">Use this API to create a new calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9cda-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9cda-103">Prerequisites</span></span>
<span data-ttu-id="f9cda-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="f9cda-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="f9cda-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9cda-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="f9cda-106">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9cda-106">Request headers</span></span>
| <span data-ttu-id="f9cda-107">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9cda-107">Header</span></span>       | <span data-ttu-id="f9cda-108">値</span><span class="sxs-lookup"><span data-stu-id="f9cda-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9cda-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9cda-109">Authorization</span></span>  | <span data-ttu-id="f9cda-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f9cda-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9cda-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9cda-112">Content-Type</span></span>  | <span data-ttu-id="f9cda-113">application/json</span><span class="sxs-lookup"><span data-stu-id="f9cda-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9cda-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9cda-114">Request body</span></span>
<span data-ttu-id="f9cda-115">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9cda-115">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f9cda-116">応答</span><span class="sxs-lookup"><span data-stu-id="f9cda-116">Response</span></span>

<span data-ttu-id="f9cda-117">成功した場合、このメソッドは応答本文で `201, Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9cda-117">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9cda-118">例</span><span class="sxs-lookup"><span data-stu-id="f9cda-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9cda-119">要求</span><span class="sxs-lookup"><span data-stu-id="f9cda-119">Request</span></span>
<span data-ttu-id="f9cda-120">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9cda-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="f9cda-121">要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9cda-121">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f9cda-122">応答</span><span class="sxs-lookup"><span data-stu-id="f9cda-122">Response</span></span>
<span data-ttu-id="f9cda-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9cda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
    }
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
