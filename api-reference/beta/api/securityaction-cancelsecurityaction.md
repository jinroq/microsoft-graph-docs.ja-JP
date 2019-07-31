---
title: 'securityAction: cancelSecurityAction'
description: セキュリティ操作をキャンセルします。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 25e08b3e751ca532f334710f24db0a0a7bde2d0f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991542"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="2b5ad-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="2b5ad-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b5ad-104">セキュリティ操作をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b5ad-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b5ad-105">Permissions</span></span>

<span data-ttu-id="2b5ad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b5ad-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b5ad-108">Permission type</span></span>                        | <span data-ttu-id="2b5ad-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b5ad-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2b5ad-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b5ad-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b5ad-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-111">Not supported.</span></span> |
| <span data-ttu-id="2b5ad-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b5ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b5ad-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-113">Not supported.</span></span> |
| <span data-ttu-id="2b5ad-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b5ad-114">Application</span></span>                            | <span data-ttu-id="2b5ad-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5ad-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b5ad-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b5ad-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="2b5ad-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b5ad-117">Request headers</span></span>

| <span data-ttu-id="2b5ad-118">名前</span><span class="sxs-lookup"><span data-stu-id="2b5ad-118">Name</span></span>          | <span data-ttu-id="2b5ad-119">説明</span><span class="sxs-lookup"><span data-stu-id="2b5ad-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2b5ad-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b5ad-120">Authorization</span></span> | <span data-ttu-id="2b5ad-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2b5ad-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b5ad-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b5ad-122">Request body</span></span>

<span data-ttu-id="2b5ad-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b5ad-124">応答</span><span class="sxs-lookup"><span data-stu-id="2b5ad-124">Response</span></span>

<span data-ttu-id="2b5ad-p102">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b5ad-127">例</span><span class="sxs-lookup"><span data-stu-id="2b5ad-127">Examples</span></span>

<span data-ttu-id="2b5ad-128">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2b5ad-129">要求</span><span class="sxs-lookup"><span data-stu-id="2b5ad-129">Request</span></span>

<span data-ttu-id="2b5ad-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2b5ad-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2b5ad-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b5ad-132">C#</span><span class="sxs-lookup"><span data-stu-id="2b5ad-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b5ad-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b5ad-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b5ad-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="2b5ad-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2b5ad-135">Java</span><span class="sxs-lookup"><span data-stu-id="2b5ad-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2b5ad-136">応答</span><span class="sxs-lookup"><span data-stu-id="2b5ad-136">Response</span></span>

<span data-ttu-id="2b5ad-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b5ad-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
