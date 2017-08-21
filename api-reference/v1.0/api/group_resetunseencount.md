# <a name="group-resetunseencount"></a><span data-ttu-id="fb6c1-101">グループ: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="fb6c1-101">group: resetUnseenCount</span></span>

<span data-ttu-id="fb6c1-p101">現在のユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount をリセットします。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb6c1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb6c1-104">Prerequisites</span></span>
<span data-ttu-id="fb6c1-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="fb6c1-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span> 
## <a name="http-request"></a><span data-ttu-id="fb6c1-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb6c1-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="fb6c1-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb6c1-107">Request headers</span></span>
| <span data-ttu-id="fb6c1-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb6c1-108">Header</span></span>       | <span data-ttu-id="fb6c1-109">値</span><span class="sxs-lookup"><span data-stu-id="fb6c1-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb6c1-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb6c1-110">Authorization</span></span>  | <span data-ttu-id="fb6c1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb6c1-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb6c1-113">Request body</span></span>
<span data-ttu-id="fb6c1-114">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb6c1-115">応答</span><span class="sxs-lookup"><span data-stu-id="fb6c1-115">Response</span></span>

<span data-ttu-id="fb6c1-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb6c1-118">例</span><span class="sxs-lookup"><span data-stu-id="fb6c1-118">Example</span></span>
<span data-ttu-id="fb6c1-119">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fb6c1-120">要求</span><span class="sxs-lookup"><span data-stu-id="fb6c1-120">Request</span></span>
<span data-ttu-id="fb6c1-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="fb6c1-122">応答</span><span class="sxs-lookup"><span data-stu-id="fb6c1-122">Response</span></span>
<span data-ttu-id="fb6c1-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fb6c1-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
