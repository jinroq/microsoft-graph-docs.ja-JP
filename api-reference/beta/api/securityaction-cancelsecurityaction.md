---
title: 'securityAction: cancelSecurityAction'
description: セキュリティ操作をキャンセルします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 953fa3ce38597c84f3f87f71f5b6746ad86e495e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870314"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="ad4c2-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="ad4c2-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad4c2-104">セキュリティ操作をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad4c2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad4c2-105">Permissions</span></span>

<span data-ttu-id="ad4c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad4c2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad4c2-108">Permission type</span></span>                        | <span data-ttu-id="ad4c2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad4c2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ad4c2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad4c2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad4c2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-111">Not supported.</span></span> |
| <span data-ttu-id="ad4c2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad4c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad4c2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-113">Not supported.</span></span> |
| <span data-ttu-id="ad4c2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad4c2-114">Application</span></span>                            | <span data-ttu-id="ad4c2-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4c2-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad4c2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad4c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="ad4c2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad4c2-117">Request headers</span></span>

| <span data-ttu-id="ad4c2-118">名前</span><span class="sxs-lookup"><span data-stu-id="ad4c2-118">Name</span></span>          | <span data-ttu-id="ad4c2-119">説明</span><span class="sxs-lookup"><span data-stu-id="ad4c2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ad4c2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad4c2-120">Authorization</span></span> | <span data-ttu-id="ad4c2-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ad4c2-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad4c2-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad4c2-122">Request body</span></span>

<span data-ttu-id="ad4c2-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad4c2-124">応答</span><span class="sxs-lookup"><span data-stu-id="ad4c2-124">Response</span></span>

<span data-ttu-id="ad4c2-p102">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad4c2-127">例</span><span class="sxs-lookup"><span data-stu-id="ad4c2-127">Examples</span></span>

<span data-ttu-id="ad4c2-128">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ad4c2-129">要求</span><span class="sxs-lookup"><span data-stu-id="ad4c2-129">Request</span></span>

<span data-ttu-id="ad4c2-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad4c2-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ad4c2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad4c2-132">C#</span><span class="sxs-lookup"><span data-stu-id="ad4c2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad4c2-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad4c2-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad4c2-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="ad4c2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ad4c2-135">Java</span><span class="sxs-lookup"><span data-stu-id="ad4c2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad4c2-136">応答</span><span class="sxs-lookup"><span data-stu-id="ad4c2-136">Response</span></span>

<span data-ttu-id="ad4c2-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad4c2-137">The following is an example of the response.</span></span>
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
