# <a name="update-page"></a><span data-ttu-id="3784c-101">ページを更新する</span><span class="sxs-lookup"><span data-stu-id="3784c-101">Update page</span></span>

<span data-ttu-id="3784c-102">OneNote ページの内容を更新します。</span><span class="sxs-lookup"><span data-stu-id="3784c-102">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="3784c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3784c-103">Permissions</span></span>
<span data-ttu-id="3784c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3784c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3784c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3784c-106">Permission type</span></span>      | <span data-ttu-id="3784c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3784c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3784c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3784c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3784c-109">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3784c-109">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3784c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3784c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3784c-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3784c-111">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3784c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3784c-112">Application</span></span> | <span data-ttu-id="3784c-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3784c-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3784c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3784c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="3784c-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3784c-115">Request headers</span></span>
| <span data-ttu-id="3784c-116">名前</span><span class="sxs-lookup"><span data-stu-id="3784c-116">Name</span></span>       | <span data-ttu-id="3784c-117">型</span><span class="sxs-lookup"><span data-stu-id="3784c-117">Type</span></span> | <span data-ttu-id="3784c-118">説明</span><span class="sxs-lookup"><span data-stu-id="3784c-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3784c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3784c-119">Authorization</span></span>  | <span data-ttu-id="3784c-120">string</span><span class="sxs-lookup"><span data-stu-id="3784c-120">string</span></span>  | <span data-ttu-id="3784c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3784c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3784c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3784c-123">Content-Type</span></span> | <span data-ttu-id="3784c-124">string</span><span class="sxs-lookup"><span data-stu-id="3784c-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3784c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3784c-125">Request body</span></span>
<span data-ttu-id="3784c-p103">要求本文で、ページの変更内容を表す [patchContentCommand](../resources/patchcontentcommand.md) オブジェクトの配列を指定します。詳細と例については、「<a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote ページ コンテンツを更新する</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3784c-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="3784c-128">応答</span><span class="sxs-lookup"><span data-stu-id="3784c-128">Response</span></span>

<span data-ttu-id="3784c-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="3784c-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="3784c-131">例</span><span class="sxs-lookup"><span data-stu-id="3784c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3784c-132">要求</span><span class="sxs-lookup"><span data-stu-id="3784c-132">Request</span></span>
<span data-ttu-id="3784c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3784c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="3784c-134">応答</span><span class="sxs-lookup"><span data-stu-id="3784c-134">Response</span></span>
<span data-ttu-id="3784c-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3784c-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
