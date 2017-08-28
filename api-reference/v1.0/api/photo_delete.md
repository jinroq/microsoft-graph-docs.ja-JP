# <a name="delete-photo"></a><span data-ttu-id="860a8-101">写真を削除する</span><span class="sxs-lookup"><span data-stu-id="860a8-101">Delete photo</span></span>

<span data-ttu-id="860a8-102">写真を削除します。</span><span class="sxs-lookup"><span data-stu-id="860a8-102">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="860a8-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="860a8-103">Permissions</span></span>
<span data-ttu-id="860a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="860a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="860a8-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="860a8-106">Permission type</span></span>      | <span data-ttu-id="860a8-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="860a8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="860a8-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="860a8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="860a8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860a8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="860a8-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="860a8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="860a8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860a8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="860a8-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="860a8-112">Application</span></span> | <span data-ttu-id="860a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="860a8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="860a8-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="860a8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="860a8-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="860a8-115">Request headers</span></span>
| <span data-ttu-id="860a8-116">名前</span><span class="sxs-lookup"><span data-stu-id="860a8-116">Name</span></span>       | <span data-ttu-id="860a8-117">型</span><span class="sxs-lookup"><span data-stu-id="860a8-117">Type</span></span> | <span data-ttu-id="860a8-118">説明</span><span class="sxs-lookup"><span data-stu-id="860a8-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="860a8-119">if-match</span><span class="sxs-lookup"><span data-stu-id="860a8-119">if-match</span></span>  | <span data-ttu-id="860a8-120">string</span><span class="sxs-lookup"><span data-stu-id="860a8-120">string</span></span>  | <span data-ttu-id="860a8-121">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="860a8-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="860a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="860a8-122">Authorization</span></span>  | <span data-ttu-id="860a8-123">string</span><span class="sxs-lookup"><span data-stu-id="860a8-123">string</span></span>  | <span data-ttu-id="860a8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="860a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="860a8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="860a8-126">Request body</span></span>
<span data-ttu-id="860a8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="860a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="860a8-128">応答</span><span class="sxs-lookup"><span data-stu-id="860a8-128">Response</span></span>

<span data-ttu-id="860a8-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="860a8-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="860a8-131">例</span><span class="sxs-lookup"><span data-stu-id="860a8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="860a8-132">要求</span><span class="sxs-lookup"><span data-stu-id="860a8-132">Request</span></span>
<span data-ttu-id="860a8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="860a8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="860a8-134">応答</span><span class="sxs-lookup"><span data-stu-id="860a8-134">Response</span></span>
<span data-ttu-id="860a8-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="860a8-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
