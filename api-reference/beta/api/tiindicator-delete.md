---
title: 脅威インテリジェンス指標の削除
description: TiIndicator オブジェクトを削除します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e7a1f3af86ec603c360d66d1b3c9d757d1da2254
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270729"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="e8c18-103">脅威インテリジェンス指標の削除</span><span class="sxs-lookup"><span data-stu-id="e8c18-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8c18-104">[Tiindicator](../resources/tiindicator.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e8c18-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8c18-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8c18-105">Permissions</span></span>

<span data-ttu-id="e8c18-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8c18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8c18-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8c18-108">Permission type</span></span>                        | <span data-ttu-id="e8c18-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8c18-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8c18-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8c18-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8c18-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e8c18-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e8c18-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8c18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8c18-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8c18-113">Not supported.</span></span> |
| <span data-ttu-id="e8c18-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8c18-114">Application</span></span>                            | <span data-ttu-id="e8c18-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e8c18-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8c18-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8c18-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8c18-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8c18-117">Request headers</span></span>

| <span data-ttu-id="e8c18-118">名前</span><span class="sxs-lookup"><span data-stu-id="e8c18-118">Name</span></span>          | <span data-ttu-id="e8c18-119">説明</span><span class="sxs-lookup"><span data-stu-id="e8c18-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e8c18-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8c18-120">Authorization</span></span> | <span data-ttu-id="e8c18-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e8c18-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8c18-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8c18-122">Request body</span></span>

<span data-ttu-id="e8c18-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8c18-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8c18-124">応答</span><span class="sxs-lookup"><span data-stu-id="e8c18-124">Response</span></span>

<span data-ttu-id="e8c18-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e8c18-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8c18-127">例</span><span class="sxs-lookup"><span data-stu-id="e8c18-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8c18-128">要求</span><span class="sxs-lookup"><span data-stu-id="e8c18-128">Request</span></span>

<span data-ttu-id="e8c18-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8c18-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="e8c18-130">応答</span><span class="sxs-lookup"><span data-stu-id="e8c18-130">Response</span></span>

<span data-ttu-id="e8c18-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8c18-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8c18-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e8c18-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8c18-133">C#</span><span class="sxs-lookup"><span data-stu-id="e8c18-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8c18-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8c18-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e8c18-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="e8c18-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
