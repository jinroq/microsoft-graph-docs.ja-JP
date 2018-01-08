# <a name="remove-rejectedsender"></a><span data-ttu-id="c354b-101">rejectedSender の削除</span><span class="sxs-lookup"><span data-stu-id="c354b-101">Remove rejectedSender</span></span>
<span data-ttu-id="c354b-102">rejectedSenders リストからユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="c354b-102">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="c354b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c354b-103">Permissions</span></span>
<span data-ttu-id="c354b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c354b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c354b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c354b-106">Permission type</span></span>                        | <span data-ttu-id="c354b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c354b-107">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="c354b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c354b-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="c354b-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c354b-109">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c354b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c354b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c354b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c354b-111">Not supported.</span></span> |
| <span data-ttu-id="c354b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c354b-112">Application</span></span>                            | <span data-ttu-id="c354b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c354b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c354b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c354b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="c354b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c354b-115">Request headers</span></span>

| <span data-ttu-id="c354b-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c354b-116">Header</span></span>         | <span data-ttu-id="c354b-117">値</span><span class="sxs-lookup"><span data-stu-id="c354b-117">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c354b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="c354b-118">Authorization</span></span>  | <span data-ttu-id="c354b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c354b-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="c354b-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="c354b-121">Request body</span></span>
<span data-ttu-id="c354b-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c354b-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c354b-123">応答</span><span class="sxs-lookup"><span data-stu-id="c354b-123">Response</span></span>
<span data-ttu-id="c354b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c354b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c354b-126">例</span><span class="sxs-lookup"><span data-stu-id="c354b-126">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c354b-127">要求</span><span class="sxs-lookup"><span data-stu-id="c354b-127">Request</span></span>
<span data-ttu-id="c354b-128">要求のいくつかの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c354b-128">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{id}

DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="c354b-129">応答</span><span class="sxs-lookup"><span data-stu-id="c354b-129">Response</span></span>
<span data-ttu-id="c354b-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c354b-130">The following is an example of a response.</span></span> 
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->