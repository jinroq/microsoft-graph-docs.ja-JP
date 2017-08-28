# <a name="get-eventmessage"></a><span data-ttu-id="ebdc3-101">eventMessage の取得</span><span class="sxs-lookup"><span data-stu-id="ebdc3-101">Get eventMessage</span></span>

<span data-ttu-id="ebdc3-102">[eventMessage](../resources/eventmessage.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="ebdc3-103">現在、この操作によって返されるイベント メッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebdc3-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ebdc3-104">Permissions</span></span>
<span data-ttu-id="ebdc3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebdc3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebdc3-107">Permission type</span></span>      | <span data-ttu-id="ebdc3-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebdc3-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebdc3-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebdc3-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ebdc3-110">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebdc3-110">Mail.Read</span></span>    |
|<span data-ttu-id="ebdc3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebdc3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebdc3-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebdc3-112">Mail.Read</span></span>    |
|<span data-ttu-id="ebdc3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebdc3-113">Application</span></span> | <span data-ttu-id="ebdc3-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebdc3-114">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebdc3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebdc3-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebdc3-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ebdc3-116">Optional query parameters</span></span>
<span data-ttu-id="ebdc3-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ebdc3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebdc3-118">Request headers</span></span>
| <span data-ttu-id="ebdc3-119">名前</span><span class="sxs-lookup"><span data-stu-id="ebdc3-119">Name</span></span>       | <span data-ttu-id="ebdc3-120">型</span><span class="sxs-lookup"><span data-stu-id="ebdc3-120">Type</span></span> | <span data-ttu-id="ebdc3-121">説明</span><span class="sxs-lookup"><span data-stu-id="ebdc3-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ebdc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebdc3-122">Authorization</span></span>  | <span data-ttu-id="ebdc3-123">string</span><span class="sxs-lookup"><span data-stu-id="ebdc3-123">string</span></span>  | <span data-ttu-id="ebdc3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebdc3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebdc3-126">Request body</span></span>
<span data-ttu-id="ebdc3-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebdc3-128">応答</span><span class="sxs-lookup"><span data-stu-id="ebdc3-128">Response</span></span>

<span data-ttu-id="ebdc3-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-129">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebdc3-130">例</span><span class="sxs-lookup"><span data-stu-id="ebdc3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebdc3-131">要求</span><span class="sxs-lookup"><span data-stu-id="ebdc3-131">Request</span></span>
<span data-ttu-id="ebdc3-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="ebdc3-133">応答</span><span class="sxs-lookup"><span data-stu-id="ebdc3-133">Response</span></span>
<span data-ttu-id="ebdc3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebdc3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
