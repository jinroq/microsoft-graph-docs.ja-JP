---
title: 脅威インテリジェンス指標の削除
description: TiIndicator オブジェクトを削除します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 9da78dd3d762e77bb15bdbade131f435e6660300
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451417"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="d105e-103">脅威インテリジェンス指標の削除</span><span class="sxs-lookup"><span data-stu-id="d105e-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d105e-104">[Tiindicator](../resources/tiindicator.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d105e-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d105e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d105e-105">Permissions</span></span>

<span data-ttu-id="d105e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d105e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d105e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d105e-108">Permission type</span></span>                        | <span data-ttu-id="d105e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d105e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d105e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d105e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d105e-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d105e-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="d105e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d105e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d105e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d105e-113">Not supported.</span></span> |
| <span data-ttu-id="d105e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d105e-114">Application</span></span>                            | <span data-ttu-id="d105e-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d105e-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="d105e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d105e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d105e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d105e-117">Request headers</span></span>

| <span data-ttu-id="d105e-118">名前</span><span class="sxs-lookup"><span data-stu-id="d105e-118">Name</span></span>          | <span data-ttu-id="d105e-119">説明</span><span class="sxs-lookup"><span data-stu-id="d105e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d105e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d105e-120">Authorization</span></span> | <span data-ttu-id="d105e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d105e-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d105e-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="d105e-122">Request body</span></span>

<span data-ttu-id="d105e-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d105e-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d105e-124">応答</span><span class="sxs-lookup"><span data-stu-id="d105e-124">Response</span></span>

<span data-ttu-id="d105e-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d105e-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d105e-127">例</span><span class="sxs-lookup"><span data-stu-id="d105e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d105e-128">要求</span><span class="sxs-lookup"><span data-stu-id="d105e-128">Request</span></span>

<span data-ttu-id="d105e-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d105e-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d105e-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d105e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d105e-131">C#</span><span class="sxs-lookup"><span data-stu-id="d105e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d105e-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="d105e-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d105e-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="d105e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d105e-134">応答</span><span class="sxs-lookup"><span data-stu-id="d105e-134">Response</span></span>

<span data-ttu-id="d105e-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d105e-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
