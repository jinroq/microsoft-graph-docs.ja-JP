---
title: アプリケーションを削除する
description: アプリケーションを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfc3fd437d81bcc9cdd8490f9597b409f87969a0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945579"
---
# <a name="delete-application"></a><span data-ttu-id="c51e0-103">アプリケーションを削除する</span><span class="sxs-lookup"><span data-stu-id="c51e0-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c51e0-104">アプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="c51e0-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c51e0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c51e0-105">Permissions</span></span>
<span data-ttu-id="c51e0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c51e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51e0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c51e0-108">Permission type</span></span>      | <span data-ttu-id="c51e0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c51e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c51e0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c51e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c51e0-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c51e0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c51e0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c51e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c51e0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c51e0-113">Not supported.</span></span>    |
|<span data-ttu-id="c51e0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c51e0-114">Application</span></span> | <span data-ttu-id="c51e0-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51e0-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c51e0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c51e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c51e0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c51e0-117">Request headers</span></span>
| <span data-ttu-id="c51e0-118">名前</span><span class="sxs-lookup"><span data-stu-id="c51e0-118">Name</span></span>       | <span data-ttu-id="c51e0-119">型</span><span class="sxs-lookup"><span data-stu-id="c51e0-119">Type</span></span> | <span data-ttu-id="c51e0-120">説明</span><span class="sxs-lookup"><span data-stu-id="c51e0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c51e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51e0-121">Authorization</span></span>  | <span data-ttu-id="c51e0-122">string</span><span class="sxs-lookup"><span data-stu-id="c51e0-122">string</span></span>  | <span data-ttu-id="c51e0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c51e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c51e0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c51e0-125">Request body</span></span>
<span data-ttu-id="c51e0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c51e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c51e0-127">応答</span><span class="sxs-lookup"><span data-stu-id="c51e0-127">Response</span></span>

<span data-ttu-id="c51e0-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c51e0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c51e0-130">例</span><span class="sxs-lookup"><span data-stu-id="c51e0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c51e0-131">要求</span><span class="sxs-lookup"><span data-stu-id="c51e0-131">Request</span></span>
<span data-ttu-id="c51e0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c51e0-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c51e0-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c51e0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c51e0-134">C#</span><span class="sxs-lookup"><span data-stu-id="c51e0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c51e0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c51e0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c51e0-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="c51e0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c51e0-137">Java</span><span class="sxs-lookup"><span data-stu-id="c51e0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c51e0-138">応答</span><span class="sxs-lookup"><span data-stu-id="c51e0-138">Response</span></span>
<span data-ttu-id="c51e0-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c51e0-139">Here is an example of the response.</span></span> 
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
