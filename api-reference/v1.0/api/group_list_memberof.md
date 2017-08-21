# <a name="list-memberof"></a><span data-ttu-id="73f17-101">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="73f17-101">List memberOf</span></span>

<span data-ttu-id="73f17-102">グループが直接メンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="73f17-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="73f17-p101">この操作は推移的ではありません。ユーザーの Office 365 のグループ取得と異なり、これは Office 365 のグループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="73f17-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="73f17-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="73f17-105">Prerequisites</span></span>
<span data-ttu-id="73f17-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="73f17-106">One of the following **scopes** is required to execute this API: *Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="73f17-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73f17-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73f17-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73f17-108">Optional query parameters</span></span>
<span data-ttu-id="73f17-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73f17-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="73f17-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73f17-110">Request headers</span></span>
| <span data-ttu-id="73f17-111">名前</span><span class="sxs-lookup"><span data-stu-id="73f17-111">Name</span></span>       | <span data-ttu-id="73f17-112">型</span><span class="sxs-lookup"><span data-stu-id="73f17-112">Type</span></span> | <span data-ttu-id="73f17-113">説明</span><span class="sxs-lookup"><span data-stu-id="73f17-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73f17-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="73f17-114">Authorization</span></span>  | <span data-ttu-id="73f17-115">string</span><span class="sxs-lookup"><span data-stu-id="73f17-115">string</span></span>  | <span data-ttu-id="73f17-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73f17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73f17-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="73f17-118">Request body</span></span>
<span data-ttu-id="73f17-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73f17-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73f17-120">応答</span><span class="sxs-lookup"><span data-stu-id="73f17-120">Response</span></span>

<span data-ttu-id="73f17-121">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="73f17-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73f17-122">例</span><span class="sxs-lookup"><span data-stu-id="73f17-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73f17-123">要求</span><span class="sxs-lookup"><span data-stu-id="73f17-123">Request</span></span>
<span data-ttu-id="73f17-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73f17-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="73f17-125">応答</span><span class="sxs-lookup"><span data-stu-id="73f17-125">Response</span></span>
<span data-ttu-id="73f17-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73f17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->