# <a name="delete-conversation-thread"></a><span data-ttu-id="4a20f-101">会話スレッドを削除する</span><span class="sxs-lookup"><span data-stu-id="4a20f-101">Delete conversation thread</span></span>
<span data-ttu-id="4a20f-102">[thread](../resources/conversationthread.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4a20f-102">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a20f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a20f-103">Permissions</span></span>
<span data-ttu-id="4a20f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a20f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a20f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a20f-106">Permission type</span></span>      | <span data-ttu-id="4a20f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a20f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a20f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a20f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a20f-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a20f-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a20f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a20f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a20f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a20f-111">Not supported.</span></span>    |
|<span data-ttu-id="4a20f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a20f-112">Application</span></span> | <span data-ttu-id="4a20f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a20f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a20f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a20f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a20f-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a20f-115">Request headers</span></span>
| <span data-ttu-id="4a20f-116">名前</span><span class="sxs-lookup"><span data-stu-id="4a20f-116">Name</span></span>       | <span data-ttu-id="4a20f-117">型</span><span class="sxs-lookup"><span data-stu-id="4a20f-117">Type</span></span> | <span data-ttu-id="4a20f-118">説明</span><span class="sxs-lookup"><span data-stu-id="4a20f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a20f-119">承認</span><span class="sxs-lookup"><span data-stu-id="4a20f-119">Authorization</span></span>  | <span data-ttu-id="4a20f-120">文字列</span><span class="sxs-lookup"><span data-stu-id="4a20f-120">string</span></span>  | <span data-ttu-id="4a20f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a20f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a20f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a20f-123">Request body</span></span>
<span data-ttu-id="4a20f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4a20f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a20f-125">応答</span><span class="sxs-lookup"><span data-stu-id="4a20f-125">Response</span></span>
<span data-ttu-id="4a20f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4a20f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a20f-128">例</span><span class="sxs-lookup"><span data-stu-id="4a20f-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4a20f-129">要求</span><span class="sxs-lookup"><span data-stu-id="4a20f-129">Request</span></span>
<span data-ttu-id="4a20f-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a20f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="4a20f-131">応答</span><span class="sxs-lookup"><span data-stu-id="4a20f-131">Response</span></span>
<span data-ttu-id="4a20f-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a20f-132">The following is an example of the response.</span></span> 
><span data-ttu-id="4a20f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a20f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->