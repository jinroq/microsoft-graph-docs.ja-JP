---
title: FeatureRolloutPolicy の削除
description: FeatureRolloutPolicy オブジェクトを削除します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72163a15beb9b6b82c4ad60640add3849d60a8b1
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062152"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="f1f00-103">FeatureRolloutPolicy の削除</span><span class="sxs-lookup"><span data-stu-id="f1f00-103">Delete featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f00-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f1f00-104">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1f00-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1f00-105">Permissions</span></span>

<span data-ttu-id="f1f00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1f00-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1f00-108">Permission type</span></span>                        | <span data-ttu-id="f1f00-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1f00-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1f00-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1f00-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1f00-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="f1f00-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="f1f00-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1f00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1f00-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1f00-113">Not supported.</span></span> |
| <span data-ttu-id="f1f00-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1f00-114">Application</span></span>                            | <span data-ttu-id="f1f00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1f00-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1f00-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1f00-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1f00-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1f00-117">Request headers</span></span>

| <span data-ttu-id="f1f00-118">名前</span><span class="sxs-lookup"><span data-stu-id="f1f00-118">Name</span></span>          | <span data-ttu-id="f1f00-119">説明</span><span class="sxs-lookup"><span data-stu-id="f1f00-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1f00-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1f00-120">Authorization</span></span> | <span data-ttu-id="f1f00-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f1f00-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1f00-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1f00-122">Request body</span></span>

<span data-ttu-id="f1f00-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1f00-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1f00-124">応答</span><span class="sxs-lookup"><span data-stu-id="f1f00-124">Response</span></span>

<span data-ttu-id="f1f00-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f1f00-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1f00-127">例</span><span class="sxs-lookup"><span data-stu-id="f1f00-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1f00-128">要求</span><span class="sxs-lookup"><span data-stu-id="f1f00-128">Request</span></span>

<span data-ttu-id="f1f00-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1f00-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="f1f00-130">応答</span><span class="sxs-lookup"><span data-stu-id="f1f00-130">Response</span></span>

<span data-ttu-id="f1f00-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1f00-131">The following is an example of the response.</span></span>

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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->