---
title: FeatureRolloutPolicy の更新
description: Featurerolloutpolicy オブジェクトのプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdbe19a401f10acead10884f02de5d380465e0a
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062155"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="58963-103">Featurerolloutpolicy の更新</span><span class="sxs-lookup"><span data-stu-id="58963-103">Update featurerolloutpolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58963-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58963-104">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58963-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58963-105">Permissions</span></span>

<span data-ttu-id="58963-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58963-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58963-108">Permission type</span></span>                        | <span data-ttu-id="58963-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58963-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="58963-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58963-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="58963-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="58963-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="58963-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58963-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58963-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58963-113">Not supported.</span></span> |
| <span data-ttu-id="58963-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58963-114">Application</span></span>                            | <span data-ttu-id="58963-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58963-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58963-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58963-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="58963-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58963-117">Request headers</span></span>

| <span data-ttu-id="58963-118">名前</span><span class="sxs-lookup"><span data-stu-id="58963-118">Name</span></span>       | <span data-ttu-id="58963-119">説明</span><span class="sxs-lookup"><span data-stu-id="58963-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="58963-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="58963-120">Authorization</span></span> | <span data-ttu-id="58963-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="58963-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58963-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="58963-122">Request body</span></span>

<span data-ttu-id="58963-123">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="58963-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="58963-124">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="58963-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="58963-125">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="58963-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="58963-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58963-126">Property</span></span>     | <span data-ttu-id="58963-127">型</span><span class="sxs-lookup"><span data-stu-id="58963-127">Type</span></span>        | <span data-ttu-id="58963-128">説明</span><span class="sxs-lookup"><span data-stu-id="58963-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58963-129">description</span><span class="sxs-lookup"><span data-stu-id="58963-129">description</span></span>|<span data-ttu-id="58963-130">String</span><span class="sxs-lookup"><span data-stu-id="58963-130">String</span></span>|<span data-ttu-id="58963-131">このポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="58963-131">A description for this policy.</span></span>|
|<span data-ttu-id="58963-132">displayName</span><span class="sxs-lookup"><span data-stu-id="58963-132">displayName</span></span>|<span data-ttu-id="58963-133">String</span><span class="sxs-lookup"><span data-stu-id="58963-133">String</span></span>|<span data-ttu-id="58963-134">このポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="58963-134">The display name for this policy.</span></span>|
|<span data-ttu-id="58963-135">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="58963-135">isAppliedToOrganization</span></span>|<span data-ttu-id="58963-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="58963-136">Boolean</span></span>|<span data-ttu-id="58963-137">この機能ロールアウトポリシーを組織全体に適用する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58963-137">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="58963-138">isEnabled</span><span class="sxs-lookup"><span data-stu-id="58963-138">isEnabled</span></span>|<span data-ttu-id="58963-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="58963-139">Boolean</span></span>|<span data-ttu-id="58963-140">機能ロールアウトが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58963-140">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="58963-141">応答</span><span class="sxs-lookup"><span data-stu-id="58963-141">Response</span></span>

<span data-ttu-id="58963-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="58963-142">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58963-143">例</span><span class="sxs-lookup"><span data-stu-id="58963-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58963-144">要求</span><span class="sxs-lookup"><span data-stu-id="58963-144">Request</span></span>

<span data-ttu-id="58963-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58963-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a

Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="58963-146">応答</span><span class="sxs-lookup"><span data-stu-id="58963-146">Response</span></span>

<span data-ttu-id="58963-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58963-147">The following is an example of the response.</span></span>

> <span data-ttu-id="58963-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="58963-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update featurerolloutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
