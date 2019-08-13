---
title: PublishedResource の削除
description: '[Publishedresource](../resources/publishedresource.md)オブジェクトを削除します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b5c520746acc71e99e5297df06f630dde783e56
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342188"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="4f431-103">PublishedResource の削除</span><span class="sxs-lookup"><span data-stu-id="4f431-103">Delete publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f431-104">[Publishedresource](../resources/publishedresource.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4f431-104">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f431-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f431-105">Permissions</span></span>

<span data-ttu-id="4f431-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f431-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f431-108">Permission type</span></span>                        | <span data-ttu-id="4f431-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f431-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="4f431-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f431-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f431-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="4f431-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="4f431-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f431-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f431-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f431-113">Not supported.</span></span> |
| <span data-ttu-id="4f431-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f431-114">Application</span></span>                            | <span data-ttu-id="4f431-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f431-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f431-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f431-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4f431-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f431-117">Request headers</span></span>

| <span data-ttu-id="4f431-118">名前</span><span class="sxs-lookup"><span data-stu-id="4f431-118">Name</span></span>          | <span data-ttu-id="4f431-119">説明</span><span class="sxs-lookup"><span data-stu-id="4f431-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4f431-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f431-120">Authorization</span></span> | <span data-ttu-id="4f431-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="4f431-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f431-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f431-122">Request body</span></span>

<span data-ttu-id="4f431-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4f431-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f431-124">応答</span><span class="sxs-lookup"><span data-stu-id="4f431-124">Response</span></span>

<span data-ttu-id="4f431-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4f431-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f431-127">例</span><span class="sxs-lookup"><span data-stu-id="4f431-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f431-128">要求</span><span class="sxs-lookup"><span data-stu-id="4f431-128">Request</span></span>

<span data-ttu-id="4f431-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f431-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f431-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4f431-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f431-131">C#</span><span class="sxs-lookup"><span data-stu-id="4f431-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f431-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f431-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f431-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="4f431-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f431-134">Java</span><span class="sxs-lookup"><span data-stu-id="4f431-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f431-135">応答</span><span class="sxs-lookup"><span data-stu-id="4f431-135">Response</span></span>

<span data-ttu-id="4f431-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f431-136">The following is an example of the response.</span></span>

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
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
