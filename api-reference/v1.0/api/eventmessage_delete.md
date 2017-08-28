# <a name="delete-eventmessage"></a><span data-ttu-id="907a0-101">eventMessage の削除</span><span class="sxs-lookup"><span data-stu-id="907a0-101">Delete eventMessage</span></span>

<span data-ttu-id="907a0-102">eventMessage を削除します。</span><span class="sxs-lookup"><span data-stu-id="907a0-102">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="907a0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="907a0-103">Permissions</span></span>
<span data-ttu-id="907a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="907a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="907a0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="907a0-106">Permission type</span></span>      | <span data-ttu-id="907a0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="907a0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="907a0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="907a0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="907a0-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="907a0-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="907a0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="907a0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="907a0-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="907a0-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="907a0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="907a0-112">Application</span></span> | <span data-ttu-id="907a0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="907a0-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="907a0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="907a0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="907a0-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="907a0-115">Request headers</span></span>
| <span data-ttu-id="907a0-116">名前</span><span class="sxs-lookup"><span data-stu-id="907a0-116">Name</span></span>       | <span data-ttu-id="907a0-117">型</span><span class="sxs-lookup"><span data-stu-id="907a0-117">Type</span></span> | <span data-ttu-id="907a0-118">説明</span><span class="sxs-lookup"><span data-stu-id="907a0-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="907a0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="907a0-119">Authorization</span></span>  | <span data-ttu-id="907a0-120">string</span><span class="sxs-lookup"><span data-stu-id="907a0-120">string</span></span>  | <span data-ttu-id="907a0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="907a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="907a0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="907a0-123">Request body</span></span>
<span data-ttu-id="907a0-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="907a0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="907a0-125">応答</span><span class="sxs-lookup"><span data-stu-id="907a0-125">Response</span></span>

<span data-ttu-id="907a0-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="907a0-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="907a0-128">例</span><span class="sxs-lookup"><span data-stu-id="907a0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="907a0-129">要求</span><span class="sxs-lookup"><span data-stu-id="907a0-129">Request</span></span>
<span data-ttu-id="907a0-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="907a0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="907a0-131">応答</span><span class="sxs-lookup"><span data-stu-id="907a0-131">Response</span></span>
<span data-ttu-id="907a0-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="907a0-132">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->