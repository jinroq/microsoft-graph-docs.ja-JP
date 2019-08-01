---
title: 写真を削除する
description: 写真を削除します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f4e5a1650e2c75ec16c7625597fccd6111d94b83
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976258"
---
# <a name="delete-photo"></a><span data-ttu-id="8be35-103">写真を削除する</span><span class="sxs-lookup"><span data-stu-id="8be35-103">Delete photo</span></span>

<span data-ttu-id="8be35-104">写真を削除します。</span><span class="sxs-lookup"><span data-stu-id="8be35-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="8be35-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8be35-105">Permissions</span></span>
<span data-ttu-id="8be35-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8be35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8be35-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8be35-108">Permission type</span></span>      | <span data-ttu-id="8be35-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8be35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8be35-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8be35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8be35-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8be35-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8be35-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8be35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8be35-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8be35-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8be35-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8be35-114">Application</span></span> | <span data-ttu-id="8be35-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8be35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8be35-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8be35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="8be35-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8be35-117">Request headers</span></span>
| <span data-ttu-id="8be35-118">名前</span><span class="sxs-lookup"><span data-stu-id="8be35-118">Name</span></span>       | <span data-ttu-id="8be35-119">型</span><span class="sxs-lookup"><span data-stu-id="8be35-119">Type</span></span> | <span data-ttu-id="8be35-120">説明</span><span class="sxs-lookup"><span data-stu-id="8be35-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8be35-121">if-match</span><span class="sxs-lookup"><span data-stu-id="8be35-121">if-match</span></span>  | <span data-ttu-id="8be35-122">string</span><span class="sxs-lookup"><span data-stu-id="8be35-122">string</span></span>  | <span data-ttu-id="8be35-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="8be35-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="8be35-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8be35-124">Authorization</span></span>  | <span data-ttu-id="8be35-125">string</span><span class="sxs-lookup"><span data-stu-id="8be35-125">string</span></span>  | <span data-ttu-id="8be35-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8be35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8be35-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8be35-128">Request body</span></span>
<span data-ttu-id="8be35-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8be35-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8be35-130">応答</span><span class="sxs-lookup"><span data-stu-id="8be35-130">Response</span></span>

<span data-ttu-id="8be35-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8be35-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8be35-133">例</span><span class="sxs-lookup"><span data-stu-id="8be35-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8be35-134">要求</span><span class="sxs-lookup"><span data-stu-id="8be35-134">Request</span></span>
<span data-ttu-id="8be35-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8be35-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8be35-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8be35-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8be35-137">C#</span><span class="sxs-lookup"><span data-stu-id="8be35-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8be35-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8be35-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8be35-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="8be35-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8be35-140">Java</span><span class="sxs-lookup"><span data-stu-id="8be35-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8be35-141">応答</span><span class="sxs-lookup"><span data-stu-id="8be35-141">Response</span></span>
<span data-ttu-id="8be35-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8be35-142">Here is an example of the response.</span></span>
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
