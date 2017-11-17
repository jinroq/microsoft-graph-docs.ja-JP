# <a name="list-calendarview"></a><span data-ttu-id="754e2-101">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="754e2-101">List calendarView</span></span>

<span data-ttu-id="754e2-102">グループの既定の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="754e2-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="permissions"></a><span data-ttu-id="754e2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="754e2-103">Permissions</span></span>
<span data-ttu-id="754e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="754e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="754e2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="754e2-106">Permission type</span></span>      | <span data-ttu-id="754e2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="754e2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="754e2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="754e2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="754e2-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="754e2-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="754e2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="754e2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="754e2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="754e2-111">Not supported.</span></span>    |
|<span data-ttu-id="754e2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="754e2-112">Application</span></span> | <span data-ttu-id="754e2-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="754e2-113">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="754e2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="754e2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="754e2-115">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="754e2-115">Query parameters</span></span>

<span data-ttu-id="754e2-116">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="754e2-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="754e2-117">パラメーター</span><span class="sxs-lookup"><span data-stu-id="754e2-117">Parameter</span></span>    | <span data-ttu-id="754e2-118">型</span><span class="sxs-lookup"><span data-stu-id="754e2-118">Type</span></span>   |<span data-ttu-id="754e2-119">説明</span><span class="sxs-lookup"><span data-stu-id="754e2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="754e2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="754e2-120">startDateTime</span></span>|<span data-ttu-id="754e2-121">String</span><span class="sxs-lookup"><span data-stu-id="754e2-121">String</span></span>|<span data-ttu-id="754e2-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="754e2-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="754e2-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="754e2-124">endDateTime</span></span>|<span data-ttu-id="754e2-125">String</span><span class="sxs-lookup"><span data-stu-id="754e2-125">String</span></span>|<span data-ttu-id="754e2-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="754e2-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="754e2-128">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="754e2-128">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="754e2-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="754e2-129">Request headers</span></span>
| <span data-ttu-id="754e2-130">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="754e2-130">Header</span></span>       | <span data-ttu-id="754e2-131">値</span><span class="sxs-lookup"><span data-stu-id="754e2-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="754e2-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="754e2-132">Authorization</span></span>  | <span data-ttu-id="754e2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="754e2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="754e2-135">Prefer</span><span class="sxs-lookup"><span data-stu-id="754e2-135">Prefer</span></span> | <span data-ttu-id="754e2-136">string</span><span class="sxs-lookup"><span data-stu-id="754e2-136">string</span></span> | <span data-ttu-id="754e2-p105">outlook.timezone="Eastern 標準時"です。省略可能。これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。指定されていない場合、応答は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="754e2-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="754e2-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="754e2-141">Request body</span></span>
<span data-ttu-id="754e2-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="754e2-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="754e2-143">応答</span><span class="sxs-lookup"><span data-stu-id="754e2-143">Response</span></span>

<span data-ttu-id="754e2-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="754e2-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="754e2-145">例</span><span class="sxs-lookup"><span data-stu-id="754e2-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="754e2-146">要求</span><span class="sxs-lookup"><span data-stu-id="754e2-146">Request</span></span>
<span data-ttu-id="754e2-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="754e2-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="754e2-148">応答</span><span class="sxs-lookup"><span data-stu-id="754e2-148">Response</span></span>
<span data-ttu-id="754e2-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="754e2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
