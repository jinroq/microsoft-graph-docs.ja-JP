---
title: AppliesTo の削除
description: 機能ロールアウトから directoryObject を削除します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1247cc352103bce040dc994feccd23ab9ba5a1bc
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062151"
---
# <a name="remove-appliesto"></a><span data-ttu-id="bd587-103">AppliesTo の削除</span><span class="sxs-lookup"><span data-stu-id="bd587-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd587-104">機能のロールアウトから[Directoryobject](../resources/directoryobject.md)を削除するには、 [FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトの appliesTo を削除します。</span><span class="sxs-lookup"><span data-stu-id="bd587-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd587-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bd587-105">Permissions</span></span>

<span data-ttu-id="bd587-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd587-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd587-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd587-108">Permission type</span></span>                        | <span data-ttu-id="bd587-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd587-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd587-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd587-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd587-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="bd587-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="bd587-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd587-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd587-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd587-113">Not supported.</span></span> |
| <span data-ttu-id="bd587-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd587-114">Application</span></span>                            | <span data-ttu-id="bd587-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd587-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd587-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd587-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bd587-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd587-117">Request headers</span></span>

| <span data-ttu-id="bd587-118">名前</span><span class="sxs-lookup"><span data-stu-id="bd587-118">Name</span></span>          | <span data-ttu-id="bd587-119">説明</span><span class="sxs-lookup"><span data-stu-id="bd587-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd587-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd587-120">Authorization</span></span> | <span data-ttu-id="bd587-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bd587-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd587-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd587-122">Request body</span></span>

<span data-ttu-id="bd587-123">要求本文で、 [directoryobject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bd587-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bd587-124">応答</span><span class="sxs-lookup"><span data-stu-id="bd587-124">Response</span></span>

<span data-ttu-id="bd587-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bd587-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd587-127">例</span><span class="sxs-lookup"><span data-stu-id="bd587-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd587-128">要求</span><span class="sxs-lookup"><span data-stu-id="bd587-128">Request</span></span>

<span data-ttu-id="bd587-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bd587-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```

### <a name="response"></a><span data-ttu-id="bd587-130">応答</span><span class="sxs-lookup"><span data-stu-id="bd587-130">Response</span></span>

<span data-ttu-id="bd587-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bd587-131">The following is an example of the response.</span></span>

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