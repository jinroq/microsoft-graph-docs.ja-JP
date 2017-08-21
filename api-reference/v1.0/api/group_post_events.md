# <a name="create-event"></a><span data-ttu-id="b6674-101">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="b6674-101">Create Event</span></span>

<span data-ttu-id="b6674-102">この API を使用して、新しい[イベント](../resources/event.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="b6674-102">Use this API to create a new [event](../resources/event.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6674-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6674-103">Prerequisites</span></span>
<span data-ttu-id="b6674-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="b6674-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="b6674-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6674-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```
## <a name="request-headers"></a><span data-ttu-id="b6674-106">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6674-106">Request headers</span></span>
| <span data-ttu-id="b6674-107">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6674-107">Header</span></span>       | <span data-ttu-id="b6674-108">値</span><span class="sxs-lookup"><span data-stu-id="b6674-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6674-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6674-109">Authorization</span></span>  | <span data-ttu-id="b6674-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6674-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6674-112">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6674-112">Request body</span></span>
<span data-ttu-id="b6674-113">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6674-113">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6674-114">応答</span><span class="sxs-lookup"><span data-stu-id="b6674-114">Response</span></span>

<span data-ttu-id="b6674-115">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b6674-115">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6674-116">例</span><span class="sxs-lookup"><span data-stu-id="b6674-116">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6674-117">要求</span><span class="sxs-lookup"><span data-stu-id="b6674-117">Request</span></span>
<span data-ttu-id="b6674-118">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6674-118">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="b6674-119">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6674-119">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b6674-120">応答</span><span class="sxs-lookup"><span data-stu-id="b6674-120">Response</span></span>
<span data-ttu-id="b6674-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6674-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
