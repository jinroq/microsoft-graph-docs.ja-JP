---
title: FeatureRolloutPolicy を作成する
description: 新しい featureRolloutPolicy オブジェクトを作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 716fa19e8fcccc69a33e53a22360638545ec81f5
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062153"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="b729a-103">FeatureRolloutPolicy を作成する</span><span class="sxs-lookup"><span data-stu-id="b729a-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b729a-104">新しい[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b729a-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b729a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b729a-105">Permissions</span></span>

<span data-ttu-id="b729a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b729a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b729a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b729a-108">Permission type</span></span>                        | <span data-ttu-id="b729a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b729a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b729a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b729a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b729a-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="b729a-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="b729a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b729a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b729a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b729a-113">Not supported.</span></span> |
| <span data-ttu-id="b729a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b729a-114">Application</span></span>                            | <span data-ttu-id="b729a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b729a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b729a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b729a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b729a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b729a-117">Request headers</span></span>

| <span data-ttu-id="b729a-118">名前</span><span class="sxs-lookup"><span data-stu-id="b729a-118">Name</span></span>          | <span data-ttu-id="b729a-119">説明</span><span class="sxs-lookup"><span data-stu-id="b729a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b729a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b729a-120">Authorization</span></span> | <span data-ttu-id="b729a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b729a-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b729a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="b729a-122">Request body</span></span>

<span data-ttu-id="b729a-123">要求本文で、 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b729a-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="b729a-124">次の表に、 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b729a-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="b729a-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b729a-125">Parameter</span></span> | <span data-ttu-id="b729a-126">型</span><span class="sxs-lookup"><span data-stu-id="b729a-126">Type</span></span> | <span data-ttu-id="b729a-127">説明</span><span class="sxs-lookup"><span data-stu-id="b729a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b729a-128">displayName</span><span class="sxs-lookup"><span data-stu-id="b729a-128">displayName</span></span> |<span data-ttu-id="b729a-129">string</span><span class="sxs-lookup"><span data-stu-id="b729a-129">string</span></span> |<span data-ttu-id="b729a-130">この機能ロールアウトポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="b729a-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="b729a-131">特徴</span><span class="sxs-lookup"><span data-stu-id="b729a-131">feature</span></span> |<span data-ttu-id="b729a-132">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="b729a-132">stagedFeatureName</span></span> |<span data-ttu-id="b729a-133">このポリシーを使用してロールアウトされる機能。</span><span class="sxs-lookup"><span data-stu-id="b729a-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="b729a-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b729a-134">isEnabled</span></span> |<span data-ttu-id="b729a-135">string</span><span class="sxs-lookup"><span data-stu-id="b729a-135">string</span></span> |<span data-ttu-id="b729a-136">機能ロールアウトが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b729a-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="b729a-137">応答</span><span class="sxs-lookup"><span data-stu-id="b729a-137">Response</span></span>

<span data-ttu-id="b729a-138">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b729a-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b729a-139">例</span><span class="sxs-lookup"><span data-stu-id="b729a-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b729a-140">要求</span><span class="sxs-lookup"><span data-stu-id="b729a-140">Request</span></span>

<span data-ttu-id="b729a-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b729a-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_directory"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="b729a-142">応答</span><span class="sxs-lookup"><span data-stu-id="b729a-142">Response</span></span>

<span data-ttu-id="b729a-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b729a-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b729a-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b729a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
