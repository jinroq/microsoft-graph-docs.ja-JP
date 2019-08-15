---
title: アプリケーションを削除する
description: アプリケーションを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 671f1c2774c1e9c75224bd7159d9b0685e44ab13
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408364"
---
# <a name="delete-application"></a><span data-ttu-id="9f736-103">アプリケーションを削除する</span><span class="sxs-lookup"><span data-stu-id="9f736-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f736-104">アプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="9f736-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f736-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f736-105">Permissions</span></span>
<span data-ttu-id="9f736-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f736-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f736-108">Permission type</span></span>      | <span data-ttu-id="9f736-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f736-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f736-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f736-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f736-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f736-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f736-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f736-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f736-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f736-113">Not supported.</span></span>    |
|<span data-ttu-id="9f736-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f736-114">Application</span></span> | <span data-ttu-id="9f736-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f736-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f736-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f736-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f736-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f736-117">Request headers</span></span>
| <span data-ttu-id="9f736-118">名前</span><span class="sxs-lookup"><span data-stu-id="9f736-118">Name</span></span>       | <span data-ttu-id="9f736-119">型</span><span class="sxs-lookup"><span data-stu-id="9f736-119">Type</span></span> | <span data-ttu-id="9f736-120">説明</span><span class="sxs-lookup"><span data-stu-id="9f736-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f736-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f736-121">Authorization</span></span>  | <span data-ttu-id="9f736-122">string</span><span class="sxs-lookup"><span data-stu-id="9f736-122">string</span></span>  | <span data-ttu-id="9f736-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9f736-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f736-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f736-125">Request body</span></span>
<span data-ttu-id="9f736-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9f736-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f736-127">応答</span><span class="sxs-lookup"><span data-stu-id="9f736-127">Response</span></span>

<span data-ttu-id="9f736-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9f736-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f736-130">例</span><span class="sxs-lookup"><span data-stu-id="9f736-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f736-131">要求</span><span class="sxs-lookup"><span data-stu-id="9f736-131">Request</span></span>
<span data-ttu-id="9f736-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f736-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9f736-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9f736-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f736-134">C#</span><span class="sxs-lookup"><span data-stu-id="9f736-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f736-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f736-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f736-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="9f736-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9f736-137">応答</span><span class="sxs-lookup"><span data-stu-id="9f736-137">Response</span></span>
<span data-ttu-id="9f736-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9f736-138">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
