# <a name="get-post"></a><span data-ttu-id="e5534-101">投稿を取得する</span><span class="sxs-lookup"><span data-stu-id="e5534-101">Get post</span></span>

<span data-ttu-id="e5534-p101">指定したスレッド内の投稿のプロパティと関係を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5534-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="e5534-104">**投稿**リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**投稿**インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="e5534-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5534-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5534-105">Prerequisites</span></span>
<span data-ttu-id="e5534-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5534-106">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="e5534-107">*Group.Read.All*、*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e5534-107">*Group.Read.All*, *Group.Readwrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e5534-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5534-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5534-109">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e5534-109">Optional query parameters</span></span>
<span data-ttu-id="e5534-110">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e5534-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e5534-111">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5534-111">Request headers</span></span>
| <span data-ttu-id="e5534-112">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5534-112">Header</span></span>       | <span data-ttu-id="e5534-113">値</span><span class="sxs-lookup"><span data-stu-id="e5534-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5534-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5534-114">Authorization</span></span>  | <span data-ttu-id="e5534-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e5534-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5534-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5534-117">Request body</span></span>
<span data-ttu-id="e5534-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e5534-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5534-119">応答</span><span class="sxs-lookup"><span data-stu-id="e5534-119">Response</span></span>

<span data-ttu-id="e5534-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[投稿](../resources/post.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5534-120">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5534-121">例</span><span class="sxs-lookup"><span data-stu-id="e5534-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5534-122">要求</span><span class="sxs-lookup"><span data-stu-id="e5534-122">Request</span></span>
<span data-ttu-id="e5534-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5534-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="e5534-124">応答</span><span class="sxs-lookup"><span data-stu-id="e5534-124">Response</span></span>
<span data-ttu-id="e5534-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5534-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

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
  }
}
```

## <a name="see-also"></a><span data-ttu-id="e5534-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5534-128">See also</span></span>

- [<span data-ttu-id="e5534-129">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="e5534-129">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e5534-130">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="e5534-130">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
