# <a name="list-rejectedsenders"></a><span data-ttu-id="ea4e5-101">rejectedSenders の一覧表示</span><span class="sxs-lookup"><span data-stu-id="ea4e5-101">List rejectedSenders</span></span>

<span data-ttu-id="ea4e5-102">このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="ea4e5-p101">拒否送信者リスト内のユーザーは、グループの会話に投稿できません (取得要求 URL で識別)。拒否送信者と承認送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea4e5-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="ea4e5-105">Prerequisites</span></span>
<span data-ttu-id="ea4e5-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ea4e5-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="ea4e5-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea4e5-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea4e5-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea4e5-108">Optional query parameters</span></span>
<span data-ttu-id="ea4e5-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea4e5-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea4e5-110">Request headers</span></span>
| <span data-ttu-id="ea4e5-111">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea4e5-111">Header</span></span>       | <span data-ttu-id="ea4e5-112">値</span><span class="sxs-lookup"><span data-stu-id="ea4e5-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea4e5-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea4e5-113">Authorization</span></span>  | <span data-ttu-id="ea4e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea4e5-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea4e5-116">Request body</span></span>
<span data-ttu-id="ea4e5-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea4e5-118">応答</span><span class="sxs-lookup"><span data-stu-id="ea4e5-118">Response</span></span>

<span data-ttu-id="ea4e5-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea4e5-120">例</span><span class="sxs-lookup"><span data-stu-id="ea4e5-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea4e5-121">要求</span><span class="sxs-lookup"><span data-stu-id="ea4e5-121">Request</span></span>
<span data-ttu-id="ea4e5-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
##### <a name="response"></a><span data-ttu-id="ea4e5-123">応答</span><span class="sxs-lookup"><span data-stu-id="ea4e5-123">Response</span></span>
<span data-ttu-id="ea4e5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea4e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->