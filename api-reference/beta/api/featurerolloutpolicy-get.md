---
title: FeatureRolloutPolicy を取得する
description: Featurerolloutpolicy オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58f2145ad897c142b09f0a26edad8e362f1778bf
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172850"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="fca37-103">FeatureRolloutPolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="fca37-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca37-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="fca37-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fca37-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fca37-105">Permissions</span></span>

<span data-ttu-id="fca37-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fca37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fca37-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fca37-108">Permission type</span></span>                        | <span data-ttu-id="fca37-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fca37-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fca37-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fca37-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fca37-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca37-111">Policy.Read.All</span></span> |
| <span data-ttu-id="fca37-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fca37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca37-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fca37-113">Not supported.</span></span> |
| <span data-ttu-id="fca37-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fca37-114">Application</span></span>                            | <span data-ttu-id="fca37-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fca37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca37-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fca37-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fca37-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fca37-117">Optional query parameters</span></span>

<span data-ttu-id="fca37-118">このメソッドは、 `$select`応答をカスタマイズするための OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="fca37-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="fca37-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fca37-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fca37-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fca37-120">Request headers</span></span>

| <span data-ttu-id="fca37-121">名前</span><span class="sxs-lookup"><span data-stu-id="fca37-121">Name</span></span>      |<span data-ttu-id="fca37-122">説明</span><span class="sxs-lookup"><span data-stu-id="fca37-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fca37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fca37-123">Authorization</span></span> | <span data-ttu-id="fca37-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fca37-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fca37-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fca37-125">Request body</span></span>

<span data-ttu-id="fca37-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fca37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca37-127">応答</span><span class="sxs-lookup"><span data-stu-id="fca37-127">Response</span></span>

<span data-ttu-id="fca37-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fca37-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fca37-129">例</span><span class="sxs-lookup"><span data-stu-id="fca37-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fca37-130">要求</span><span class="sxs-lookup"><span data-stu-id="fca37-130">Request</span></span>

<span data-ttu-id="fca37-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fca37-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fca37-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fca37-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fca37-133">C#</span><span class="sxs-lookup"><span data-stu-id="fca37-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fca37-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fca37-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fca37-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="fca37-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fca37-136">Java</span><span class="sxs-lookup"><span data-stu-id="fca37-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fca37-137">応答</span><span class="sxs-lookup"><span data-stu-id="fca37-137">Response</span></span>

<span data-ttu-id="fca37-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fca37-138">The following is an example of the response.</span></span>

> <span data-ttu-id="fca37-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fca37-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="request"></a><span data-ttu-id="fca37-141">要求</span><span class="sxs-lookup"><span data-stu-id="fca37-141">Request</span></span>

<span data-ttu-id="fca37-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fca37-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fca37-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fca37-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fca37-144">C#</span><span class="sxs-lookup"><span data-stu-id="fca37-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fca37-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="fca37-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fca37-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="fca37-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fca37-147">Java</span><span class="sxs-lookup"><span data-stu-id="fca37-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fca37-148">応答</span><span class="sxs-lookup"><span data-stu-id="fca37-148">Response</span></span>

<span data-ttu-id="fca37-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fca37-149">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="fca37-150">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="fca37-150">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fca37-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fca37-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
