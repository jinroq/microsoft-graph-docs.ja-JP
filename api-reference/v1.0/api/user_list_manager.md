# <a name="list-manager"></a><span data-ttu-id="b0fd5-101">上司を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b0fd5-101">List manager</span></span>

<span data-ttu-id="b0fd5-p101">ユーザーの上司を取得します。ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0fd5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b0fd5-104">Prerequisites</span></span>
<span data-ttu-id="b0fd5-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="b0fd5-105">One of the following **scopes** is required to execute this API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="b0fd5-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0fd5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0fd5-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0fd5-107">Optional query parameters</span></span>
<span data-ttu-id="b0fd5-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0fd5-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0fd5-109">Request headers</span></span>
| <span data-ttu-id="b0fd5-110">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0fd5-110">Header</span></span>       | <span data-ttu-id="b0fd5-111">値</span><span class="sxs-lookup"><span data-stu-id="b0fd5-111">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b0fd5-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0fd5-112">Authorization</span></span>  | <span data-ttu-id="b0fd5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b0fd5-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0fd5-115">Content-Type</span></span>   | <span data-ttu-id="b0fd5-116">application/json</span><span class="sxs-lookup"><span data-stu-id="b0fd5-116">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b0fd5-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0fd5-117">Request body</span></span>
<span data-ttu-id="b0fd5-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0fd5-119">応答</span><span class="sxs-lookup"><span data-stu-id="b0fd5-119">Response</span></span>

<span data-ttu-id="b0fd5-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0fd5-121">例</span><span class="sxs-lookup"><span data-stu-id="b0fd5-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0fd5-122">要求</span><span class="sxs-lookup"><span data-stu-id="b0fd5-122">Request</span></span>
<span data-ttu-id="b0fd5-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="b0fd5-124">応答</span><span class="sxs-lookup"><span data-stu-id="b0fd5-124">Response</span></span>
<span data-ttu-id="b0fd5-125">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b0fd5-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
