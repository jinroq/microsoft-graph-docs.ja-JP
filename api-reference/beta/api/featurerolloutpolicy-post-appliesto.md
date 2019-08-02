---
title: AppliesTo を割り当てる
description: 機能のロールアウトに directoryObject を割り当てます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b5a01131adb20feccbccd55c2ce4f7e01ea1e214
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062154"
---
# <a name="assign-appliesto"></a><span data-ttu-id="610b4-103">AppliesTo を割り当てる</span><span class="sxs-lookup"><span data-stu-id="610b4-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="610b4-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトに appliesTo を追加して、 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)を適用する必要がある[directoryobject](../resources/directoryobject.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="610b4-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="610b4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="610b4-105">Permissions</span></span>

<span data-ttu-id="610b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="610b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="610b4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="610b4-108">Permission type</span></span>                        | <span data-ttu-id="610b4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="610b4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="610b4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="610b4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="610b4-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="610b4-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="610b4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="610b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="610b4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="610b4-113">Not supported.</span></span> |
| <span data-ttu-id="610b4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="610b4-114">Application</span></span>                            | <span data-ttu-id="610b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="610b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="610b4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="610b4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="610b4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="610b4-117">Request headers</span></span>

| <span data-ttu-id="610b4-118">名前</span><span class="sxs-lookup"><span data-stu-id="610b4-118">Name</span></span>          | <span data-ttu-id="610b4-119">説明</span><span class="sxs-lookup"><span data-stu-id="610b4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="610b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="610b4-120">Authorization</span></span> | <span data-ttu-id="610b4-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="610b4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="610b4-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="610b4-122">Request body</span></span>

<span data-ttu-id="610b4-123">要求本文で、 [directoryobject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="610b4-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="610b4-124">応答</span><span class="sxs-lookup"><span data-stu-id="610b4-124">Response</span></span>

<span data-ttu-id="610b4-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[directoryobject](../resources/directoryobject.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="610b4-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="610b4-126">例</span><span class="sxs-lookup"><span data-stu-id="610b4-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="610b4-127">要求</span><span class="sxs-lookup"><span data-stu-id="610b4-127">Request</span></span>

<span data-ttu-id="610b4-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="610b4-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```

### <a name="response"></a><span data-ttu-id="610b4-129">応答</span><span class="sxs-lookup"><span data-stu-id="610b4-129">Response</span></span>

<span data-ttu-id="610b4-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="610b4-130">The following is an example of the response.</span></span>

> <span data-ttu-id="610b4-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="610b4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "directoryObject": {
    "id": "2441b489-4f12-4882-b039-8f6006bd66da",
    "objectType": "group"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
