# <a name="list-members"></a><span data-ttu-id="7f5ef-101">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7f5ef-101">List members</span></span>

<span data-ttu-id="7f5ef-p101">グループの直接メンバーの一覧を取得します。グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f5ef-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f5ef-105">Prerequisites</span></span>
<span data-ttu-id="7f5ef-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.Read.All*、*Directory.AccessAsUser.All*、*User.ReadBasic.All*、または *User.Read.All*</span><span class="sxs-lookup"><span data-stu-id="7f5ef-106">One of the following **scopes** is required to execute this API: *Directory.Read.All*, *Directory.AccessAsUser.All*, *User.ReadBasic.All*, or *User.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="7f5ef-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f5ef-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f5ef-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f5ef-108">Optional query parameters</span></span>
<span data-ttu-id="7f5ef-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f5ef-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f5ef-110">Request headers</span></span>
| <span data-ttu-id="7f5ef-111">名前</span><span class="sxs-lookup"><span data-stu-id="7f5ef-111">Name</span></span>       | <span data-ttu-id="7f5ef-112">型</span><span class="sxs-lookup"><span data-stu-id="7f5ef-112">Type</span></span> | <span data-ttu-id="7f5ef-113">説明</span><span class="sxs-lookup"><span data-stu-id="7f5ef-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f5ef-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f5ef-114">Authorization</span></span>  | <span data-ttu-id="7f5ef-115">string</span><span class="sxs-lookup"><span data-stu-id="7f5ef-115">string</span></span>  | <span data-ttu-id="7f5ef-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f5ef-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f5ef-118">Request body</span></span>
<span data-ttu-id="7f5ef-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f5ef-120">応答</span><span class="sxs-lookup"><span data-stu-id="7f5ef-120">Response</span></span>

<span data-ttu-id="7f5ef-121">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f5ef-122">例</span><span class="sxs-lookup"><span data-stu-id="7f5ef-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f5ef-123">要求</span><span class="sxs-lookup"><span data-stu-id="7f5ef-123">Request</span></span>
<span data-ttu-id="7f5ef-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="7f5ef-125">応答</span><span class="sxs-lookup"><span data-stu-id="7f5ef-125">Response</span></span>
<span data-ttu-id="7f5ef-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f5ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->