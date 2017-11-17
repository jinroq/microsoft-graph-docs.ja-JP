# <a name="list-attachments"></a><span data-ttu-id="c0297-101">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c0297-101">List attachments</span></span>

<span data-ttu-id="c0297-102">投稿に添付された[添付ファイル](../resources/attachment.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c0297-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0297-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0297-103">Permissions</span></span>
<span data-ttu-id="c0297-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c0297-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0297-106">Permission type</span></span>      | <span data-ttu-id="c0297-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0297-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0297-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0297-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c0297-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0297-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c0297-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0297-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0297-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0297-111">Not supported.</span></span>    |
|<span data-ttu-id="c0297-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0297-112">Application</span></span> | <span data-ttu-id="c0297-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0297-113">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0297-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0297-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c0297-115">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c0297-115">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0297-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0297-116">Optional query parameters</span></span>
<span data-ttu-id="c0297-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c0297-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0297-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0297-118">Request headers</span></span>
| <span data-ttu-id="c0297-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0297-119">Header</span></span>       | <span data-ttu-id="c0297-120">値</span><span class="sxs-lookup"><span data-stu-id="c0297-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0297-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0297-121">Authorization</span></span>  | <span data-ttu-id="c0297-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0297-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0297-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0297-124">Request body</span></span>
<span data-ttu-id="c0297-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c0297-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0297-126">応答</span><span class="sxs-lookup"><span data-stu-id="c0297-126">Response</span></span>

<span data-ttu-id="c0297-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c0297-127">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0297-128">例</span><span class="sxs-lookup"><span data-stu-id="c0297-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0297-129">要求</span><span class="sxs-lookup"><span data-stu-id="c0297-129">Request</span></span>
<span data-ttu-id="c0297-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0297-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="c0297-131">応答</span><span class="sxs-lookup"><span data-stu-id="c0297-131">Response</span></span>
<span data-ttu-id="c0297-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0297-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
