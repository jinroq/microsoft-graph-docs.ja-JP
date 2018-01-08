# <a name="group-resetunseencount"></a><span data-ttu-id="d8a6a-101">グループ: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="d8a6a-101">group: resetUnseenCount</span></span>

<span data-ttu-id="d8a6a-p101">現在のユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount をリセットします。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8a6a-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d8a6a-104">Permissions</span></span>
<span data-ttu-id="d8a6a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d8a6a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8a6a-107">Permission type</span></span>      | <span data-ttu-id="d8a6a-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8a6a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8a6a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8a6a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d8a6a-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8a6a-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8a6a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8a6a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8a6a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-112">Not supported.</span></span>    |
|<span data-ttu-id="d8a6a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8a6a-113">Application</span></span> | <span data-ttu-id="d8a6a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8a6a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8a6a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="d8a6a-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8a6a-116">Request headers</span></span>
| <span data-ttu-id="d8a6a-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8a6a-117">Header</span></span>       | <span data-ttu-id="d8a6a-118">値</span><span class="sxs-lookup"><span data-stu-id="d8a6a-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8a6a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8a6a-119">Authorization</span></span>  | <span data-ttu-id="d8a6a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8a6a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8a6a-122">Request body</span></span>
<span data-ttu-id="d8a6a-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8a6a-124">応答</span><span class="sxs-lookup"><span data-stu-id="d8a6a-124">Response</span></span>

<span data-ttu-id="d8a6a-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8a6a-127">例</span><span class="sxs-lookup"><span data-stu-id="d8a6a-127">Example</span></span>
<span data-ttu-id="d8a6a-128">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-128">Here is an example of how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="d8a6a-129">要求</span><span class="sxs-lookup"><span data-stu-id="d8a6a-129">Request</span></span>
<span data-ttu-id="d8a6a-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="d8a6a-131">応答</span><span class="sxs-lookup"><span data-stu-id="d8a6a-131">Response</span></span>
<span data-ttu-id="d8a6a-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8a6a-132">The following is an example of a response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
