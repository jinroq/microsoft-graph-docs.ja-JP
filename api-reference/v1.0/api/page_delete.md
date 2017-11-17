# <a name="delete-page"></a><span data-ttu-id="b714f-101">ページを削除する</span><span class="sxs-lookup"><span data-stu-id="b714f-101">Delete page</span></span>

<span data-ttu-id="b714f-102">OneNote のページを削除します。</span><span class="sxs-lookup"><span data-stu-id="b714f-102">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="b714f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b714f-103">Permissions</span></span>
<span data-ttu-id="b714f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b714f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b714f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b714f-106">Permission type</span></span>      | <span data-ttu-id="b714f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b714f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b714f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b714f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b714f-109">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b714f-109">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b714f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b714f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b714f-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b714f-111">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b714f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b714f-112">Application</span></span> | <span data-ttu-id="b714f-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b714f-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b714f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b714f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b714f-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b714f-115">Request headers</span></span>
| <span data-ttu-id="b714f-116">名前</span><span class="sxs-lookup"><span data-stu-id="b714f-116">Name</span></span>       | <span data-ttu-id="b714f-117">型</span><span class="sxs-lookup"><span data-stu-id="b714f-117">Type</span></span> | <span data-ttu-id="b714f-118">説明</span><span class="sxs-lookup"><span data-stu-id="b714f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b714f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b714f-119">Authorization</span></span>  | <span data-ttu-id="b714f-120">string</span><span class="sxs-lookup"><span data-stu-id="b714f-120">string</span></span>  | <span data-ttu-id="b714f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b714f-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b714f-123">応答</span><span class="sxs-lookup"><span data-stu-id="b714f-123">Response</span></span>

<span data-ttu-id="b714f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b714f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b714f-126">例</span><span class="sxs-lookup"><span data-stu-id="b714f-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b714f-127">要求</span><span class="sxs-lookup"><span data-stu-id="b714f-127">Request</span></span>
<span data-ttu-id="b714f-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b714f-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="b714f-129">応答</span><span class="sxs-lookup"><span data-stu-id="b714f-129">Response</span></span>
<span data-ttu-id="b714f-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b714f-130">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->