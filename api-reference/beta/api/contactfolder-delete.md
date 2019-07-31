---
title: Delete contactFolder
description: 既定の contactFolder 以外の contactFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b2b34b1b5d7299fc7e002e26dc9545151dc1108
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943324"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="ad2e1-103">Delete contactFolder</span><span class="sxs-lookup"><span data-stu-id="ad2e1-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad2e1-104">既定の contactFolder 以外の contactFolder を削除します。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad2e1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad2e1-105">Permissions</span></span>
<span data-ttu-id="ad2e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad2e1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad2e1-108">Permission type</span></span>      | <span data-ttu-id="ad2e1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad2e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad2e1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad2e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad2e1-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad2e1-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ad2e1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad2e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad2e1-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad2e1-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ad2e1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad2e1-114">Application</span></span> | <span data-ttu-id="ad2e1-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad2e1-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad2e1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad2e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ad2e1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad2e1-117">Request headers</span></span>
| <span data-ttu-id="ad2e1-118">名前</span><span class="sxs-lookup"><span data-stu-id="ad2e1-118">Name</span></span>       | <span data-ttu-id="ad2e1-119">型</span><span class="sxs-lookup"><span data-stu-id="ad2e1-119">Type</span></span> | <span data-ttu-id="ad2e1-120">説明</span><span class="sxs-lookup"><span data-stu-id="ad2e1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad2e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad2e1-121">Authorization</span></span>  | <span data-ttu-id="ad2e1-122">string</span><span class="sxs-lookup"><span data-stu-id="ad2e1-122">string</span></span>  | <span data-ttu-id="ad2e1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad2e1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad2e1-125">Request body</span></span>
<span data-ttu-id="ad2e1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad2e1-127">応答</span><span class="sxs-lookup"><span data-stu-id="ad2e1-127">Response</span></span>

<span data-ttu-id="ad2e1-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad2e1-130">例</span><span class="sxs-lookup"><span data-stu-id="ad2e1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad2e1-131">要求</span><span class="sxs-lookup"><span data-stu-id="ad2e1-131">Request</span></span>
<span data-ttu-id="ad2e1-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad2e1-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ad2e1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad2e1-134">C#</span><span class="sxs-lookup"><span data-stu-id="ad2e1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad2e1-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad2e1-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad2e1-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="ad2e1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ad2e1-137">Java</span><span class="sxs-lookup"><span data-stu-id="ad2e1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad2e1-138">応答</span><span class="sxs-lookup"><span data-stu-id="ad2e1-138">Response</span></span>
<span data-ttu-id="ad2e1-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ad2e1-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
