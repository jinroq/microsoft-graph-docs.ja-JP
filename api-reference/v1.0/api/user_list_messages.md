# <a name="list-messages"></a><span data-ttu-id="2a3f6-101">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2a3f6-101">List messages</span></span>

<span data-ttu-id="2a3f6-102">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="2a3f6-103">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a3f6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2a3f6-104">Prerequisites</span></span>
<span data-ttu-id="2a3f6-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Read、Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2a3f6-105">One of the following **scopes** is required to execute this API: *Mail.Read; Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2a3f6-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a3f6-106">HTTP request</span></span>

<span data-ttu-id="2a3f6-107">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="2a3f6-107">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="2a3f6-108">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="2a3f6-108">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a3f6-109">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a3f6-109">Optional query parameters</span></span>
<span data-ttu-id="2a3f6-110">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2a3f6-111">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a3f6-111">Request headers</span></span>
| <span data-ttu-id="2a3f6-112">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a3f6-112">Header</span></span>       | <span data-ttu-id="2a3f6-113">値</span><span class="sxs-lookup"><span data-stu-id="2a3f6-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a3f6-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a3f6-114">Authorization</span></span>  | <span data-ttu-id="2a3f6-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-p101">Bearer {token}. Required.</span></span>  |
 

## <a name="request-body"></a><span data-ttu-id="2a3f6-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a3f6-117">Request body</span></span>
<span data-ttu-id="2a3f6-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a3f6-119">応答</span><span class="sxs-lookup"><span data-stu-id="2a3f6-119">Response</span></span>

<span data-ttu-id="2a3f6-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-120">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="2a3f6-121">この要求の既定のページ サイズは、メッセージ 10 個です。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-121">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="2a3f6-122">例</span><span class="sxs-lookup"><span data-stu-id="2a3f6-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a3f6-123">要求</span><span class="sxs-lookup"><span data-stu-id="2a3f6-123">Request</span></span>
<span data-ttu-id="2a3f6-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="2a3f6-125">応答</span><span class="sxs-lookup"><span data-stu-id="2a3f6-125">Response</span></span>
<span data-ttu-id="2a3f6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a3f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
