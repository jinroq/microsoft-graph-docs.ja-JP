# <a name="add-attachment"></a><span data-ttu-id="5a639-101">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="5a639-101">Add attachment</span></span>

<span data-ttu-id="5a639-p101">[添付ファイル](../resources/attachment.md)を投稿に追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="5a639-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a639-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5a639-104">Prerequisites</span></span>
<span data-ttu-id="5a639-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a639-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="5a639-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a639-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5a639-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a639-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5a639-108">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5a639-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="5a639-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a639-109">Request headers</span></span>
| <span data-ttu-id="5a639-110">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a639-110">Header</span></span>       | <span data-ttu-id="5a639-111">値</span><span class="sxs-lookup"><span data-stu-id="5a639-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a639-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a639-112">Authorization</span></span>  | <span data-ttu-id="5a639-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a639-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a639-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a639-115">Request body</span></span>
<span data-ttu-id="5a639-116">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a639-116">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5a639-117">応答</span><span class="sxs-lookup"><span data-stu-id="5a639-117">Response</span></span>

<span data-ttu-id="5a639-118">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5a639-118">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="5a639-119">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="5a639-119">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5a639-120">要求</span><span class="sxs-lookup"><span data-stu-id="5a639-120">Request</span></span>
<span data-ttu-id="5a639-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a639-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="5a639-122">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a639-122">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="5a639-123">応答</span><span class="sxs-lookup"><span data-stu-id="5a639-123">Response</span></span>
<span data-ttu-id="5a639-p103">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5a639-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="5a639-127">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="5a639-127">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5a639-128">要求</span><span class="sxs-lookup"><span data-stu-id="5a639-128">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="5a639-129">応答</span><span class="sxs-lookup"><span data-stu-id="5a639-129">Response</span></span>
<span data-ttu-id="5a639-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5a639-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
