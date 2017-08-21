# <a name="list-posts"></a><span data-ttu-id="de200-101">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="de200-101">List posts</span></span>

<span data-ttu-id="de200-p101">指定したスレッドの投稿を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="de200-p101">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de200-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="de200-104">Prerequisites</span></span>
<span data-ttu-id="de200-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All、Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="de200-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="de200-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de200-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="de200-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="de200-107">Optional query parameters</span></span>
<span data-ttu-id="de200-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="de200-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="de200-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de200-109">Request headers</span></span>
| <span data-ttu-id="de200-110">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de200-110">Header</span></span>       | <span data-ttu-id="de200-111">値</span><span class="sxs-lookup"><span data-stu-id="de200-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de200-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="de200-112">Authorization</span></span>  | <span data-ttu-id="de200-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de200-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de200-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="de200-115">Request body</span></span>
<span data-ttu-id="de200-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="de200-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de200-117">応答</span><span class="sxs-lookup"><span data-stu-id="de200-117">Response</span></span>

<span data-ttu-id="de200-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Post](../resources/post.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="de200-118">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de200-119">例</span><span class="sxs-lookup"><span data-stu-id="de200-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de200-120">要求</span><span class="sxs-lookup"><span data-stu-id="de200-120">Request</span></span>
<span data-ttu-id="de200-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de200-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="de200-122">応答</span><span class="sxs-lookup"><span data-stu-id="de200-122">Response</span></span>
<span data-ttu-id="de200-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de200-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
