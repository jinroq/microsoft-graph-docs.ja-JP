---
title: OrgContact の削除
description: OrgContact を削除します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 612a56c7fdf35ddb8e6b6eefc6b89c3830c700aa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414330"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="d7bd6-103">OrgContact の削除</span><span class="sxs-lookup"><span data-stu-id="d7bd6-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7bd6-104">OrgContact を削除します。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7bd6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7bd6-105">Permissions</span></span>
<span data-ttu-id="d7bd6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7bd6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7bd6-108">Permission type</span></span>      | <span data-ttu-id="d7bd6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7bd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7bd6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7bd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7bd6-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7bd6-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7bd6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7bd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7bd6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-113">Not supported.</span></span>    |
|<span data-ttu-id="d7bd6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7bd6-114">Application</span></span> | <span data-ttu-id="d7bd6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7bd6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7bd6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d7bd6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7bd6-117">Request headers</span></span>
| <span data-ttu-id="d7bd6-118">名前</span><span class="sxs-lookup"><span data-stu-id="d7bd6-118">Name</span></span>       | <span data-ttu-id="d7bd6-119">型</span><span class="sxs-lookup"><span data-stu-id="d7bd6-119">Type</span></span> | <span data-ttu-id="d7bd6-120">説明</span><span class="sxs-lookup"><span data-stu-id="d7bd6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7bd6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7bd6-121">Authorization</span></span>  | <span data-ttu-id="d7bd6-122">string</span><span class="sxs-lookup"><span data-stu-id="d7bd6-122">string</span></span>  | <span data-ttu-id="d7bd6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7bd6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7bd6-125">Request body</span></span>
<span data-ttu-id="d7bd6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7bd6-127">応答</span><span class="sxs-lookup"><span data-stu-id="d7bd6-127">Response</span></span>

<span data-ttu-id="d7bd6-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7bd6-130">例</span><span class="sxs-lookup"><span data-stu-id="d7bd6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7bd6-131">要求</span><span class="sxs-lookup"><span data-stu-id="d7bd6-131">Request</span></span>
<span data-ttu-id="d7bd6-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7bd6-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d7bd6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7bd6-134">C#</span><span class="sxs-lookup"><span data-stu-id="d7bd6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7bd6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7bd6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7bd6-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="d7bd6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7bd6-137">応答</span><span class="sxs-lookup"><span data-stu-id="d7bd6-137">Response</span></span>
<span data-ttu-id="d7bd6-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d7bd6-138">Here is an example of the response.</span></span> 
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
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
