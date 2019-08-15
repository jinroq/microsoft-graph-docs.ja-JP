---
title: AppliesTo の削除
description: 機能ロールアウトから directoryObject を削除します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 020dd8bcd01e78cfe194df148cb57a3307dbe6ed
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419805"
---
# <a name="remove-appliesto"></a><span data-ttu-id="5066d-103">AppliesTo の削除</span><span class="sxs-lookup"><span data-stu-id="5066d-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5066d-104">機能のロールアウトから[Directoryobject](../resources/directoryobject.md)を削除するには、 [FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトの appliesTo を削除します。</span><span class="sxs-lookup"><span data-stu-id="5066d-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="5066d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5066d-105">Permissions</span></span>

<span data-ttu-id="5066d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5066d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5066d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5066d-108">Permission type</span></span>                        | <span data-ttu-id="5066d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5066d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5066d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5066d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5066d-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="5066d-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="5066d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5066d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5066d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5066d-113">Not supported.</span></span> |
| <span data-ttu-id="5066d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5066d-114">Application</span></span>                            | <span data-ttu-id="5066d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5066d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5066d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5066d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5066d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5066d-117">Request headers</span></span>

| <span data-ttu-id="5066d-118">名前</span><span class="sxs-lookup"><span data-stu-id="5066d-118">Name</span></span>          | <span data-ttu-id="5066d-119">説明</span><span class="sxs-lookup"><span data-stu-id="5066d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5066d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5066d-120">Authorization</span></span> | <span data-ttu-id="5066d-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5066d-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5066d-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="5066d-122">Request body</span></span>

<span data-ttu-id="5066d-123">要求本文で、 [directoryobject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5066d-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5066d-124">応答</span><span class="sxs-lookup"><span data-stu-id="5066d-124">Response</span></span>

<span data-ttu-id="5066d-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5066d-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5066d-127">例</span><span class="sxs-lookup"><span data-stu-id="5066d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5066d-128">要求</span><span class="sxs-lookup"><span data-stu-id="5066d-128">Request</span></span>

<span data-ttu-id="5066d-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5066d-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5066d-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5066d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5066d-131">C#</span><span class="sxs-lookup"><span data-stu-id="5066d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5066d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5066d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5066d-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="5066d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5066d-134">応答</span><span class="sxs-lookup"><span data-stu-id="5066d-134">Response</span></span>

<span data-ttu-id="5066d-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5066d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
