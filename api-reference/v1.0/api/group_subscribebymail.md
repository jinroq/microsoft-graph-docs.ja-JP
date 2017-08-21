# <a name="group-subscribebymail"></a><span data-ttu-id="8d6c5-101">グループ: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="8d6c5-101">group: subscribeByMail</span></span>

<span data-ttu-id="8d6c5-p101">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8d6c5-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d6c5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d6c5-104">Prerequisites</span></span>
<span data-ttu-id="8d6c5-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All* 
*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="8d6c5-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="8d6c5-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d6c5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="8d6c5-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d6c5-107">Request headers</span></span>
| <span data-ttu-id="8d6c5-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d6c5-108">Header</span></span>       | <span data-ttu-id="8d6c5-109">値</span><span class="sxs-lookup"><span data-stu-id="8d6c5-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d6c5-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d6c5-110">Authorization</span></span>  | <span data-ttu-id="8d6c5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d6c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d6c5-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d6c5-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8d6c5-114">応答</span><span class="sxs-lookup"><span data-stu-id="8d6c5-114">Response</span></span>

<span data-ttu-id="8d6c5-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8d6c5-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d6c5-117">例</span><span class="sxs-lookup"><span data-stu-id="8d6c5-117">Example</span></span>
<span data-ttu-id="8d6c5-118">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8d6c5-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d6c5-119">要求</span><span class="sxs-lookup"><span data-stu-id="8d6c5-119">Request</span></span>
<span data-ttu-id="8d6c5-120">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d6c5-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="8d6c5-121">応答</span><span class="sxs-lookup"><span data-stu-id="8d6c5-121">Response</span></span>
<span data-ttu-id="8d6c5-122">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8d6c5-122">Here is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->