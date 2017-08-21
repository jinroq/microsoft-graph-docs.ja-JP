# <a name="get-conversationthread"></a><span data-ttu-id="1dcd5-101">Get conversationThread</span><span class="sxs-lookup"><span data-stu-id="1dcd5-101">Get conversationThread</span></span>

<span data-ttu-id="1dcd5-p101">グループに属している特定のスレッドを取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-p101">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="1dcd5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1dcd5-104">Prerequisites</span></span>
<span data-ttu-id="1dcd5-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All、Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="1dcd5-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="1dcd5-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dcd5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1dcd5-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1dcd5-107">Optional query parameters</span></span>
<span data-ttu-id="1dcd5-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1dcd5-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dcd5-109">Request headers</span></span>
| <span data-ttu-id="1dcd5-110">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dcd5-110">Header</span></span>       | <span data-ttu-id="1dcd5-111">値</span><span class="sxs-lookup"><span data-stu-id="1dcd5-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1dcd5-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dcd5-112">Authorization</span></span>  | <span data-ttu-id="1dcd5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1dcd5-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dcd5-115">Request body</span></span>
<span data-ttu-id="1dcd5-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dcd5-117">応答</span><span class="sxs-lookup"><span data-stu-id="1dcd5-117">Response</span></span>

<span data-ttu-id="1dcd5-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-118">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1dcd5-119">例</span><span class="sxs-lookup"><span data-stu-id="1dcd5-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dcd5-120">要求</span><span class="sxs-lookup"><span data-stu-id="1dcd5-120">Request</span></span>
<span data-ttu-id="1dcd5-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="1dcd5-122">応答</span><span class="sxs-lookup"><span data-stu-id="1dcd5-122">Response</span></span>
<span data-ttu-id="1dcd5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1dcd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
