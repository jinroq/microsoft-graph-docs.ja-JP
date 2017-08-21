# <a name="get-message"></a><span data-ttu-id="7dfa3-101">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="7dfa3-101">Get message</span></span>

<span data-ttu-id="7dfa3-102">[メッセージ](../resources/message.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="7dfa3-103">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="7dfa3-104">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dfa3-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="7dfa3-105">Prerequisites</span></span>
<span data-ttu-id="7dfa3-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="7dfa3-106">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>  
## <a name="http-request"></a><span data-ttu-id="7dfa3-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dfa3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7dfa3-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7dfa3-108">Optional query parameters</span></span>
<span data-ttu-id="7dfa3-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7dfa3-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dfa3-110">Request headers</span></span>
| <span data-ttu-id="7dfa3-111">名前</span><span class="sxs-lookup"><span data-stu-id="7dfa3-111">Name</span></span>       | <span data-ttu-id="7dfa3-112">型</span><span class="sxs-lookup"><span data-stu-id="7dfa3-112">Type</span></span> | <span data-ttu-id="7dfa3-113">説明</span><span class="sxs-lookup"><span data-stu-id="7dfa3-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7dfa3-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dfa3-114">Authorization</span></span>  | <span data-ttu-id="7dfa3-115">string</span><span class="sxs-lookup"><span data-stu-id="7dfa3-115">string</span></span>  | <span data-ttu-id="7dfa3-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dfa3-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dfa3-118">Request body</span></span>
<span data-ttu-id="7dfa3-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dfa3-120">応答</span><span class="sxs-lookup"><span data-stu-id="7dfa3-120">Response</span></span>

<span data-ttu-id="7dfa3-121">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-121">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7dfa3-122">例</span><span class="sxs-lookup"><span data-stu-id="7dfa3-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7dfa3-123">要求</span><span class="sxs-lookup"><span data-stu-id="7dfa3-123">Request</span></span>
<span data-ttu-id="7dfa3-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="7dfa3-125">応答</span><span class="sxs-lookup"><span data-stu-id="7dfa3-125">Response</span></span>
<span data-ttu-id="7dfa3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7dfa3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
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
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="7dfa3-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="7dfa3-129">See also</span></span>

- [<span data-ttu-id="7dfa3-130">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="7dfa3-130">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="7dfa3-131">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="7dfa3-131">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
