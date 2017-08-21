# <a name="group-addfavorite"></a><span data-ttu-id="a737d-101">グループ: addFavorite</span><span class="sxs-lookup"><span data-stu-id="a737d-101">group: addFavorite</span></span>
<span data-ttu-id="a737d-p101">現在のユーザーのお気に入りのグループ一覧にグループを追加します。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="a737d-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a737d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a737d-104">Prerequisites</span></span>
<span data-ttu-id="a737d-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="a737d-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="a737d-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a737d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```
## <a name="request-headers"></a><span data-ttu-id="a737d-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a737d-107">Request headers</span></span>
| <span data-ttu-id="a737d-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a737d-108">Header</span></span>       | <span data-ttu-id="a737d-109">値</span><span class="sxs-lookup"><span data-stu-id="a737d-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a737d-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="a737d-110">Authorization</span></span>  | <span data-ttu-id="a737d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a737d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a737d-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="a737d-113">Request body</span></span>
<span data-ttu-id="a737d-114">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a737d-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a737d-115">応答</span><span class="sxs-lookup"><span data-stu-id="a737d-115">Response</span></span>

<span data-ttu-id="a737d-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a737d-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a737d-118">例</span><span class="sxs-lookup"><span data-stu-id="a737d-118">Example</span></span>
<span data-ttu-id="a737d-119">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a737d-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a737d-120">要求</span><span class="sxs-lookup"><span data-stu-id="a737d-120">Request</span></span>
<span data-ttu-id="a737d-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a737d-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

##### <a name="response"></a><span data-ttu-id="a737d-122">応答</span><span class="sxs-lookup"><span data-stu-id="a737d-122">Response</span></span>
<span data-ttu-id="a737d-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a737d-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->