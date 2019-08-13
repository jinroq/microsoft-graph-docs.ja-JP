---
title: FeatureRolloutPolicy を作成する
description: 新しい featureRolloutPolicy オブジェクトを作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1b1a21455253a79c2ef6a1f40d106838e58e54d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321363"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="a1fb1-103">FeatureRolloutPolicy を作成する</span><span class="sxs-lookup"><span data-stu-id="a1fb1-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1fb1-104">新しい[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1fb1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1fb1-105">Permissions</span></span>

<span data-ttu-id="a1fb1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1fb1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1fb1-108">Permission type</span></span>                        | <span data-ttu-id="a1fb1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1fb1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1fb1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1fb1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1fb1-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="a1fb1-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="a1fb1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1fb1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1fb1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-113">Not supported.</span></span> |
| <span data-ttu-id="a1fb1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1fb1-114">Application</span></span>                            | <span data-ttu-id="a1fb1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1fb1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1fb1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a1fb1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1fb1-117">Request headers</span></span>

| <span data-ttu-id="a1fb1-118">名前</span><span class="sxs-lookup"><span data-stu-id="a1fb1-118">Name</span></span>          | <span data-ttu-id="a1fb1-119">説明</span><span class="sxs-lookup"><span data-stu-id="a1fb1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a1fb1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1fb1-120">Authorization</span></span> | <span data-ttu-id="a1fb1-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a1fb1-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1fb1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1fb1-122">Request body</span></span>

<span data-ttu-id="a1fb1-123">要求本文で、 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="a1fb1-124">次の表に、 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="a1fb1-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a1fb1-125">Parameter</span></span> | <span data-ttu-id="a1fb1-126">型</span><span class="sxs-lookup"><span data-stu-id="a1fb1-126">Type</span></span> | <span data-ttu-id="a1fb1-127">説明</span><span class="sxs-lookup"><span data-stu-id="a1fb1-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1fb1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="a1fb1-128">displayName</span></span> |<span data-ttu-id="a1fb1-129">string</span><span class="sxs-lookup"><span data-stu-id="a1fb1-129">string</span></span> |<span data-ttu-id="a1fb1-130">この機能ロールアウトポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="a1fb1-131">特徴</span><span class="sxs-lookup"><span data-stu-id="a1fb1-131">feature</span></span> |<span data-ttu-id="a1fb1-132">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="a1fb1-132">stagedFeatureName</span></span> |<span data-ttu-id="a1fb1-133">このポリシーを使用してロールアウトされる機能。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="a1fb1-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a1fb1-134">isEnabled</span></span> |<span data-ttu-id="a1fb1-135">string</span><span class="sxs-lookup"><span data-stu-id="a1fb1-135">string</span></span> |<span data-ttu-id="a1fb1-136">機能ロールアウトが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="a1fb1-137">応答</span><span class="sxs-lookup"><span data-stu-id="a1fb1-137">Response</span></span>

<span data-ttu-id="a1fb1-138">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1fb1-139">例</span><span class="sxs-lookup"><span data-stu-id="a1fb1-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1fb1-140">要求</span><span class="sxs-lookup"><span data-stu-id="a1fb1-140">Request</span></span>

<span data-ttu-id="a1fb1-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1fb1-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a1fb1-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1fb1-143">C#</span><span class="sxs-lookup"><span data-stu-id="a1fb1-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1fb1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1fb1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1fb1-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="a1fb1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a1fb1-146">Java</span><span class="sxs-lookup"><span data-stu-id="a1fb1-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1fb1-147">応答</span><span class="sxs-lookup"><span data-stu-id="a1fb1-147">Response</span></span>

<span data-ttu-id="a1fb1-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-148">The following is an example of the response.</span></span>

> <span data-ttu-id="a1fb1-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a1fb1-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
