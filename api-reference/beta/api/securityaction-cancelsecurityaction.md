---
title: 'securityAction: cancelSecurityAction'
description: セキュリティ操作をキャンセルします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 33fa78176dcb32bad889c7d3336177ef96aaa0b6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638908"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="8d3dd-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="8d3dd-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d3dd-104">セキュリティ操作をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d3dd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d3dd-105">Permissions</span></span>

<span data-ttu-id="8d3dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d3dd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d3dd-108">Permission type</span></span>                        | <span data-ttu-id="8d3dd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d3dd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d3dd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d3dd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d3dd-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-111">Not supported.</span></span> |
| <span data-ttu-id="8d3dd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d3dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3dd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-113">Not supported.</span></span> |
| <span data-ttu-id="8d3dd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d3dd-114">Application</span></span>                            | <span data-ttu-id="8d3dd-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d3dd-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d3dd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d3dd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="8d3dd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d3dd-117">Request headers</span></span>

| <span data-ttu-id="8d3dd-118">名前</span><span class="sxs-lookup"><span data-stu-id="8d3dd-118">Name</span></span>          | <span data-ttu-id="8d3dd-119">説明</span><span class="sxs-lookup"><span data-stu-id="8d3dd-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d3dd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d3dd-120">Authorization</span></span> | <span data-ttu-id="8d3dd-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8d3dd-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d3dd-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d3dd-122">Request body</span></span>

<span data-ttu-id="8d3dd-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d3dd-124">応答</span><span class="sxs-lookup"><span data-stu-id="8d3dd-124">Response</span></span>

<span data-ttu-id="8d3dd-p102">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d3dd-127">例</span><span class="sxs-lookup"><span data-stu-id="8d3dd-127">Examples</span></span>

<span data-ttu-id="8d3dd-128">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8d3dd-129">要求</span><span class="sxs-lookup"><span data-stu-id="8d3dd-129">Request</span></span>

<span data-ttu-id="8d3dd-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="8d3dd-131">応答</span><span class="sxs-lookup"><span data-stu-id="8d3dd-131">Response</span></span>

<span data-ttu-id="8d3dd-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d3dd-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d3dd-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8d3dd-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d3dd-134">Visual</span><span class="sxs-lookup"><span data-stu-id="8d3dd-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d3dd-135">Java</span><span class="sxs-lookup"><span data-stu-id="8d3dd-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
