# <a name="list-attachments"></a><span data-ttu-id="a2777-101">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a2777-101">List attachments</span></span>

<span data-ttu-id="a2777-102">投稿に添付された [Attachment](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2777-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2777-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2777-103">Prerequisites</span></span>
<span data-ttu-id="a2777-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2777-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="a2777-105">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2777-105">Group.Read.All</span></span>
* <span data-ttu-id="a2777-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2777-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a2777-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2777-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a2777-108">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="a2777-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2777-109">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2777-109">Optional query parameters</span></span>
<span data-ttu-id="a2777-110">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a2777-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2777-111">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2777-111">Request headers</span></span>
| <span data-ttu-id="a2777-112">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2777-112">Header</span></span>       | <span data-ttu-id="a2777-113">値</span><span class="sxs-lookup"><span data-stu-id="a2777-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2777-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2777-114">Authorization</span></span>  | <span data-ttu-id="a2777-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2777-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2777-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2777-117">Request body</span></span>
<span data-ttu-id="a2777-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2777-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2777-119">応答</span><span class="sxs-lookup"><span data-stu-id="a2777-119">Response</span></span>

<span data-ttu-id="a2777-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a2777-120">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2777-121">例</span><span class="sxs-lookup"><span data-stu-id="a2777-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2777-122">要求</span><span class="sxs-lookup"><span data-stu-id="a2777-122">Request</span></span>
<span data-ttu-id="a2777-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2777-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="a2777-124">応答</span><span class="sxs-lookup"><span data-stu-id="a2777-124">Response</span></span>
<span data-ttu-id="a2777-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2777-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
