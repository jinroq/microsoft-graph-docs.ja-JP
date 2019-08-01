---
title: Delete contactFolder
description: 既定の contactFolder 以外の contactFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: be5f222fc59135ad992b11b2eee6d777a387f9c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003225"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="dfb02-103">Delete contactFolder</span><span class="sxs-lookup"><span data-stu-id="dfb02-103">Delete contactFolder</span></span>

<span data-ttu-id="dfb02-104">既定の contactFolder 以外の contactFolder を削除します。</span><span class="sxs-lookup"><span data-stu-id="dfb02-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfb02-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dfb02-105">Permissions</span></span>
<span data-ttu-id="dfb02-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfb02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfb02-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dfb02-108">Permission type</span></span>      | <span data-ttu-id="dfb02-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dfb02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfb02-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dfb02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfb02-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb02-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dfb02-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dfb02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfb02-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb02-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dfb02-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dfb02-114">Application</span></span> | <span data-ttu-id="dfb02-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb02-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfb02-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dfb02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dfb02-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfb02-117">Request headers</span></span>
| <span data-ttu-id="dfb02-118">名前</span><span class="sxs-lookup"><span data-stu-id="dfb02-118">Name</span></span>       | <span data-ttu-id="dfb02-119">型</span><span class="sxs-lookup"><span data-stu-id="dfb02-119">Type</span></span> | <span data-ttu-id="dfb02-120">説明</span><span class="sxs-lookup"><span data-stu-id="dfb02-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfb02-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfb02-121">Authorization</span></span>  | <span data-ttu-id="dfb02-122">string</span><span class="sxs-lookup"><span data-stu-id="dfb02-122">string</span></span>  | <span data-ttu-id="dfb02-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dfb02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfb02-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dfb02-125">Request body</span></span>
<span data-ttu-id="dfb02-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dfb02-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfb02-127">応答</span><span class="sxs-lookup"><span data-stu-id="dfb02-127">Response</span></span>

<span data-ttu-id="dfb02-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="dfb02-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfb02-130">例</span><span class="sxs-lookup"><span data-stu-id="dfb02-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfb02-131">要求</span><span class="sxs-lookup"><span data-stu-id="dfb02-131">Request</span></span>
<span data-ttu-id="dfb02-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dfb02-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dfb02-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dfb02-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dfb02-134">C#</span><span class="sxs-lookup"><span data-stu-id="dfb02-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfb02-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfb02-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dfb02-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="dfb02-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dfb02-137">Java</span><span class="sxs-lookup"><span data-stu-id="dfb02-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dfb02-138">応答</span><span class="sxs-lookup"><span data-stu-id="dfb02-138">Response</span></span>
<span data-ttu-id="dfb02-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dfb02-139">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
