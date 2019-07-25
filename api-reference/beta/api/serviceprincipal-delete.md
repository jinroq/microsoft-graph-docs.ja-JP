---
title: ServicePrincipal の削除
description: ServicePrincipal を削除します。
localization_priority: Normal
ms.openlocfilehash: c604886416eba49ae7bbd8c614ce2200a3bc9948
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870223"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="faaf5-103">ServicePrincipal の削除</span><span class="sxs-lookup"><span data-stu-id="faaf5-103">Delete servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faaf5-104">ServicePrincipal を削除します。</span><span class="sxs-lookup"><span data-stu-id="faaf5-104">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="faaf5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="faaf5-105">Permissions</span></span>
<span data-ttu-id="faaf5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="faaf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faaf5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="faaf5-108">Permission type</span></span>      | <span data-ttu-id="faaf5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="faaf5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faaf5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="faaf5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="faaf5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="faaf5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="faaf5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="faaf5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faaf5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faaf5-113">Not supported.</span></span>    |
|<span data-ttu-id="faaf5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="faaf5-114">Application</span></span> | <span data-ttu-id="faaf5-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faaf5-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="faaf5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="faaf5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="faaf5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faaf5-117">Request headers</span></span>
| <span data-ttu-id="faaf5-118">名前</span><span class="sxs-lookup"><span data-stu-id="faaf5-118">Name</span></span>       | <span data-ttu-id="faaf5-119">型</span><span class="sxs-lookup"><span data-stu-id="faaf5-119">Type</span></span> | <span data-ttu-id="faaf5-120">説明</span><span class="sxs-lookup"><span data-stu-id="faaf5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="faaf5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="faaf5-121">Authorization</span></span>  | <span data-ttu-id="faaf5-122">string</span><span class="sxs-lookup"><span data-stu-id="faaf5-122">string</span></span>  | <span data-ttu-id="faaf5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="faaf5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="faaf5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="faaf5-125">Request body</span></span>
<span data-ttu-id="faaf5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="faaf5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faaf5-127">応答</span><span class="sxs-lookup"><span data-stu-id="faaf5-127">Response</span></span>

<span data-ttu-id="faaf5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="faaf5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faaf5-130">例</span><span class="sxs-lookup"><span data-stu-id="faaf5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="faaf5-131">要求</span><span class="sxs-lookup"><span data-stu-id="faaf5-131">Request</span></span>
<span data-ttu-id="faaf5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="faaf5-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="faaf5-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="faaf5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="faaf5-134">C#</span><span class="sxs-lookup"><span data-stu-id="faaf5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="faaf5-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="faaf5-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="faaf5-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="faaf5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="faaf5-137">Java</span><span class="sxs-lookup"><span data-stu-id="faaf5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="faaf5-138">応答</span><span class="sxs-lookup"><span data-stu-id="faaf5-138">Response</span></span>
<span data-ttu-id="faaf5-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="faaf5-139">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
