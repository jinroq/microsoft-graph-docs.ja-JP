# <a name="get-calendargroup"></a><span data-ttu-id="53a21-101">Get calendarGroup</span><span class="sxs-lookup"><span data-stu-id="53a21-101">Get calendarGroup</span></span>

<span data-ttu-id="53a21-102">予定表グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="53a21-102">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53a21-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53a21-103">Permissions</span></span>

<span data-ttu-id="53a21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="53a21-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53a21-106">Permission type</span></span>                        | <span data-ttu-id="53a21-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53a21-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="53a21-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53a21-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="53a21-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="53a21-109">Calendars.Read</span></span>                              |
| <span data-ttu-id="53a21-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53a21-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53a21-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="53a21-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="53a21-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53a21-112">Application</span></span>                            | <span data-ttu-id="53a21-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="53a21-113">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="53a21-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53a21-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="53a21-115">ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="53a21-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53a21-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="53a21-116">Optional query parameters</span></span>

<span data-ttu-id="53a21-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="53a21-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53a21-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53a21-118">Request headers</span></span>

| <span data-ttu-id="53a21-119">名前</span><span class="sxs-lookup"><span data-stu-id="53a21-119">Name</span></span>          | <span data-ttu-id="53a21-120">型</span><span class="sxs-lookup"><span data-stu-id="53a21-120">Type</span></span>   | <span data-ttu-id="53a21-121">説明</span><span class="sxs-lookup"><span data-stu-id="53a21-121">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="53a21-122">承認</span><span class="sxs-lookup"><span data-stu-id="53a21-122">Authorization</span></span> | <span data-ttu-id="53a21-123">string</span><span class="sxs-lookup"><span data-stu-id="53a21-123">string</span></span> | <span data-ttu-id="53a21-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53a21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53a21-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="53a21-126">Request body</span></span>

<span data-ttu-id="53a21-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="53a21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53a21-128">応答</span><span class="sxs-lookup"><span data-stu-id="53a21-128">Response</span></span>

<span data-ttu-id="53a21-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [CalendarGroup](../resources/calendargroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53a21-129">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53a21-130">例</span><span class="sxs-lookup"><span data-stu-id="53a21-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="53a21-131">要求</span><span class="sxs-lookup"><span data-stu-id="53a21-131">Request</span></span>

<span data-ttu-id="53a21-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53a21-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="53a21-133">応答</span><span class="sxs-lookup"><span data-stu-id="53a21-133">Response</span></span>

<span data-ttu-id="53a21-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53a21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
