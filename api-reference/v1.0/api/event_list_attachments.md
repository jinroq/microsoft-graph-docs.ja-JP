# <a name="list-attachments"></a><span data-ttu-id="59db5-101">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="59db5-101">List attachments</span></span>

<span data-ttu-id="59db5-102">イベントに添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="59db5-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="59db5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59db5-103">Permissions</span></span>
<span data-ttu-id="59db5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59db5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59db5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59db5-106">Permission type</span></span>      | <span data-ttu-id="59db5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59db5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59db5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59db5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="59db5-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59db5-109">Calendars.Read</span></span>    |
|<span data-ttu-id="59db5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59db5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59db5-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59db5-111">Calendars.Read</span></span>    |
|<span data-ttu-id="59db5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59db5-112">Application</span></span> | <span data-ttu-id="59db5-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59db5-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="59db5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59db5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="59db5-115">ユーザーまたはグループの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="59db5-115">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments
GET /groups/{id}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
```
<span data-ttu-id="59db5-116">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="59db5-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="59db5-117">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="59db5-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59db5-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="59db5-118">Optional query parameters</span></span>
<span data-ttu-id="59db5-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59db5-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59db5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59db5-120">Request headers</span></span>
| <span data-ttu-id="59db5-121">名前</span><span class="sxs-lookup"><span data-stu-id="59db5-121">Name</span></span>       | <span data-ttu-id="59db5-122">型</span><span class="sxs-lookup"><span data-stu-id="59db5-122">Type</span></span> | <span data-ttu-id="59db5-123">説明</span><span class="sxs-lookup"><span data-stu-id="59db5-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59db5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="59db5-124">Authorization</span></span>  | <span data-ttu-id="59db5-125">string</span><span class="sxs-lookup"><span data-stu-id="59db5-125">string</span></span>  | <span data-ttu-id="59db5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59db5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59db5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="59db5-128">Request body</span></span>
<span data-ttu-id="59db5-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="59db5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59db5-130">応答</span><span class="sxs-lookup"><span data-stu-id="59db5-130">Response</span></span>

<span data-ttu-id="59db5-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="59db5-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59db5-132">例</span><span class="sxs-lookup"><span data-stu-id="59db5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59db5-133">要求</span><span class="sxs-lookup"><span data-stu-id="59db5-133">Request</span></span>
<span data-ttu-id="59db5-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59db5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="59db5-135">応答</span><span class="sxs-lookup"><span data-stu-id="59db5-135">Response</span></span>
<span data-ttu-id="59db5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="59db5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->