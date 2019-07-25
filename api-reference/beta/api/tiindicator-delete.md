---
title: 脅威インテリジェンス指標の削除
description: TiIndicator オブジェクトを削除します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8ebe38fc4bb0727f53f4753d48885c98a47bca1c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868271"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="3c0ae-103">脅威インテリジェンス指標の削除</span><span class="sxs-lookup"><span data-stu-id="3c0ae-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c0ae-104">[Tiindicator](../resources/tiindicator.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c0ae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c0ae-105">Permissions</span></span>

<span data-ttu-id="3c0ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c0ae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c0ae-108">Permission type</span></span>                        | <span data-ttu-id="3c0ae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3c0ae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c0ae-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3c0ae-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="3c0ae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c0ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c0ae-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-113">Not supported.</span></span> |
| <span data-ttu-id="3c0ae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c0ae-114">Application</span></span>                            | <span data-ttu-id="3c0ae-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3c0ae-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c0ae-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c0ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3c0ae-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c0ae-117">Request headers</span></span>

| <span data-ttu-id="3c0ae-118">名前</span><span class="sxs-lookup"><span data-stu-id="3c0ae-118">Name</span></span>          | <span data-ttu-id="3c0ae-119">説明</span><span class="sxs-lookup"><span data-stu-id="3c0ae-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3c0ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c0ae-120">Authorization</span></span> | <span data-ttu-id="3c0ae-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3c0ae-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c0ae-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c0ae-122">Request body</span></span>

<span data-ttu-id="3c0ae-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c0ae-124">応答</span><span class="sxs-lookup"><span data-stu-id="3c0ae-124">Response</span></span>

<span data-ttu-id="3c0ae-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c0ae-127">例</span><span class="sxs-lookup"><span data-stu-id="3c0ae-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c0ae-128">要求</span><span class="sxs-lookup"><span data-stu-id="3c0ae-128">Request</span></span>

<span data-ttu-id="3c0ae-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c0ae-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3c0ae-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c0ae-131">C#</span><span class="sxs-lookup"><span data-stu-id="3c0ae-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c0ae-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c0ae-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c0ae-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="3c0ae-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c0ae-134">Java</span><span class="sxs-lookup"><span data-stu-id="3c0ae-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c0ae-135">応答</span><span class="sxs-lookup"><span data-stu-id="3c0ae-135">Response</span></span>

<span data-ttu-id="3c0ae-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3c0ae-136">The following is an example of the response.</span></span>

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
