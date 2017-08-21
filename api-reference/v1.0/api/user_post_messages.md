# <a name="create-message"></a><span data-ttu-id="6fa8d-101">メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="6fa8d-101">Create Message</span></span>

<span data-ttu-id="6fa8d-p101">この API を使用して、新しいメッセージの下書きを作成します。下書きを任意のフォルダーに作成し、必要に応じて送信前に更新できます。[下書き] フォルダーに保存するには、/messages ショートカットを使用します。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="6fa8d-105">同じ **POST** の呼び出しで下書きを作成するときに、[添付ファイル](../resources/attachment.md)を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fa8d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6fa8d-106">Prerequisites</span></span>
<span data-ttu-id="6fa8d-107">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="6fa8d-107">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="6fa8d-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fa8d-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="6fa8d-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fa8d-109">Request headers</span></span>
| <span data-ttu-id="6fa8d-110">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fa8d-110">Header</span></span>       | <span data-ttu-id="6fa8d-111">値</span><span class="sxs-lookup"><span data-stu-id="6fa8d-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fa8d-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa8d-112">Authorization</span></span>  | <span data-ttu-id="6fa8d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6fa8d-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fa8d-115">Content-Type</span></span>  | <span data-ttu-id="6fa8d-116">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa8d-116">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fa8d-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fa8d-117">Request body</span></span>
<span data-ttu-id="6fa8d-118">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-118">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="6fa8d-119">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにメッセージに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-119">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="6fa8d-120">応答</span><span class="sxs-lookup"><span data-stu-id="6fa8d-120">Response</span></span>

<span data-ttu-id="6fa8d-121">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-121">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa8d-122">例</span><span class="sxs-lookup"><span data-stu-id="6fa8d-122">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6fa8d-123">要求 1</span><span class="sxs-lookup"><span data-stu-id="6fa8d-123">Request 1</span></span>
<span data-ttu-id="6fa8d-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json
Content-length: 248

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
```
<span data-ttu-id="6fa8d-125">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-125">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="6fa8d-126">応答 1</span><span class="sxs-lookup"><span data-stu-id="6fa8d-126">Response 1</span></span>
<span data-ttu-id="6fa8d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6fa8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 248

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
```

## <a name="see-also"></a><span data-ttu-id="6fa8d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6fa8d-130">See also</span></span>

- [<span data-ttu-id="6fa8d-131">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6fa8d-131">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="6fa8d-132">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6fa8d-132">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
