---
title: 写真を削除する
description: 写真を削除します。
localization_priority: Normal
ms.openlocfilehash: 9ca65416ecce815f99dbf8a0ff84724322f75df2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458867"
---
# <a name="delete-photo"></a><span data-ttu-id="2c50c-103">写真を削除する</span><span class="sxs-lookup"><span data-stu-id="2c50c-103">Delete photo</span></span>

<span data-ttu-id="2c50c-104">写真を削除します。</span><span class="sxs-lookup"><span data-stu-id="2c50c-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c50c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2c50c-105">Permissions</span></span>
<span data-ttu-id="2c50c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c50c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c50c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2c50c-108">Permission type</span></span>      | <span data-ttu-id="2c50c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2c50c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c50c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2c50c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c50c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c50c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c50c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2c50c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c50c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c50c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c50c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2c50c-114">Application</span></span> | <span data-ttu-id="2c50c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c50c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c50c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c50c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="2c50c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2c50c-117">Request headers</span></span>
| <span data-ttu-id="2c50c-118">名前</span><span class="sxs-lookup"><span data-stu-id="2c50c-118">Name</span></span>       | <span data-ttu-id="2c50c-119">型</span><span class="sxs-lookup"><span data-stu-id="2c50c-119">Type</span></span> | <span data-ttu-id="2c50c-120">説明</span><span class="sxs-lookup"><span data-stu-id="2c50c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c50c-121">if-match</span><span class="sxs-lookup"><span data-stu-id="2c50c-121">if-match</span></span>  | <span data-ttu-id="2c50c-122">string</span><span class="sxs-lookup"><span data-stu-id="2c50c-122">string</span></span>  | <span data-ttu-id="2c50c-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="2c50c-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="2c50c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c50c-124">Authorization</span></span>  | <span data-ttu-id="2c50c-125">string</span><span class="sxs-lookup"><span data-stu-id="2c50c-125">string</span></span>  | <span data-ttu-id="2c50c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2c50c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c50c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2c50c-128">Request body</span></span>
<span data-ttu-id="2c50c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2c50c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c50c-130">応答</span><span class="sxs-lookup"><span data-stu-id="2c50c-130">Response</span></span>

<span data-ttu-id="2c50c-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2c50c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c50c-133">例</span><span class="sxs-lookup"><span data-stu-id="2c50c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c50c-134">要求</span><span class="sxs-lookup"><span data-stu-id="2c50c-134">Request</span></span>
<span data-ttu-id="2c50c-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2c50c-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2c50c-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2c50c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c50c-137">C#</span><span class="sxs-lookup"><span data-stu-id="2c50c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c50c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c50c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c50c-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="2c50c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c50c-140">応答</span><span class="sxs-lookup"><span data-stu-id="2c50c-140">Response</span></span>
<span data-ttu-id="2c50c-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2c50c-141">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
