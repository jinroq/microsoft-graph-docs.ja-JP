# <a name="create-acceptedsender"></a><span data-ttu-id="750a2-101">AcceptedSender の作成</span><span class="sxs-lookup"><span data-stu-id="750a2-101">Create acceptedSender</span></span>

<span data-ttu-id="750a2-102">AcceptedSender リストに新しいユーザーやグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="750a2-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="750a2-p101">`@odata.id` 内のユーザーやグループを要求の本文で指定します。承諾済み送信者リスト内のユーザーは、グループに会話を投稿できません。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="750a2-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="750a2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="750a2-106">Prerequisites</span></span>
<span data-ttu-id="750a2-107">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="750a2-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="750a2-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="750a2-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="750a2-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="750a2-109">Request headers</span></span>
| <span data-ttu-id="750a2-110">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="750a2-110">Header</span></span>       | <span data-ttu-id="750a2-111">値</span><span class="sxs-lookup"><span data-stu-id="750a2-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="750a2-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="750a2-112">Authorization</span></span>  | <span data-ttu-id="750a2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="750a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="750a2-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="750a2-115">Request body</span></span>
<span data-ttu-id="750a2-116">要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="750a2-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="750a2-117">応答</span><span class="sxs-lookup"><span data-stu-id="750a2-117">Response</span></span>

<span data-ttu-id="750a2-118">このメソッドは `204, No Content` 応答コードを返し、応答の本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="750a2-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="750a2-119">例</span><span class="sxs-lookup"><span data-stu-id="750a2-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="750a2-120">要求</span><span class="sxs-lookup"><span data-stu-id="750a2-120">Request</span></span>
<span data-ttu-id="750a2-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="750a2-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="750a2-122">応答</span><span class="sxs-lookup"><span data-stu-id="750a2-122">Response</span></span>
<span data-ttu-id="750a2-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="750a2-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
