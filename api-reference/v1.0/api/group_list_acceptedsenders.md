# <a name="list-acceptedsenders"></a><span data-ttu-id="27efc-101">acceptedSenders のリスト化</span><span class="sxs-lookup"><span data-stu-id="27efc-101">List acceptedSenders</span></span>

<span data-ttu-id="27efc-102">このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="27efc-102">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="27efc-p101">承諾済み送信者リスト内のユーザーは、グループの会話を投稿することができます (要求取得 URL で識別)。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="27efc-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27efc-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="27efc-105">Prerequisites</span></span>
<span data-ttu-id="27efc-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="27efc-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="27efc-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27efc-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27efc-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="27efc-108">Optional query parameters</span></span>
<span data-ttu-id="27efc-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="27efc-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="27efc-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27efc-110">Request headers</span></span>
| <span data-ttu-id="27efc-111">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27efc-111">Header</span></span>       | <span data-ttu-id="27efc-112">値</span><span class="sxs-lookup"><span data-stu-id="27efc-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27efc-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="27efc-113">Authorization</span></span>  | <span data-ttu-id="27efc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="27efc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27efc-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="27efc-116">Request body</span></span>
<span data-ttu-id="27efc-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="27efc-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27efc-118">応答</span><span class="sxs-lookup"><span data-stu-id="27efc-118">Response</span></span>

<span data-ttu-id="27efc-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="27efc-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27efc-120">例</span><span class="sxs-lookup"><span data-stu-id="27efc-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27efc-121">要求</span><span class="sxs-lookup"><span data-stu-id="27efc-121">Request</span></span>
<span data-ttu-id="27efc-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27efc-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```
##### <a name="response"></a><span data-ttu-id="27efc-123">応答</span><span class="sxs-lookup"><span data-stu-id="27efc-123">Response</span></span>
<span data-ttu-id="27efc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27efc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->