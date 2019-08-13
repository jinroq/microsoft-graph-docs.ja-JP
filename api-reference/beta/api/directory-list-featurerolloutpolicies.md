---
title: リスト featureRolloutPolicies
description: FeatureRolloutPolicy オブジェクトのリストを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a4abaa831d16704b0e1c630fb56f50123b9f6ff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322598"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="9a720-103">リスト featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="9a720-103">List featureRolloutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a720-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a720-104">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a720-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a720-105">Permissions</span></span>

<span data-ttu-id="9a720-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a720-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a720-108">Permission type</span></span>                        | <span data-ttu-id="9a720-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a720-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a720-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a720-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a720-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a720-111">Policy.Read.All</span></span> |
| <span data-ttu-id="9a720-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a720-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a720-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a720-113">Not supported.</span></span> |
| <span data-ttu-id="9a720-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a720-114">Application</span></span>                            | <span data-ttu-id="9a720-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a720-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a720-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a720-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a720-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a720-117">Optional query parameters</span></span>

<span data-ttu-id="9a720-118">このメソッドは、応答をカスタマイズするために、、、、 `$count`、 `$expand`、 `$filter`、 `$orderby`、 `$select`の`$skip`各`$top`OData クエリパラメーターをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="9a720-118">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="9a720-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a720-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a720-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a720-120">Request headers</span></span>

| <span data-ttu-id="9a720-121">名前</span><span class="sxs-lookup"><span data-stu-id="9a720-121">Name</span></span>      |<span data-ttu-id="9a720-122">説明</span><span class="sxs-lookup"><span data-stu-id="9a720-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a720-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a720-123">Authorization</span></span> | <span data-ttu-id="9a720-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9a720-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a720-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a720-125">Request body</span></span>

<span data-ttu-id="9a720-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a720-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a720-127">応答</span><span class="sxs-lookup"><span data-stu-id="9a720-127">Response</span></span>

<span data-ttu-id="9a720-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9a720-128">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a720-129">例</span><span class="sxs-lookup"><span data-stu-id="9a720-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a720-130">要求</span><span class="sxs-lookup"><span data-stu-id="9a720-130">Request</span></span>

<span data-ttu-id="9a720-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a720-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a720-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9a720-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a720-133">C#</span><span class="sxs-lookup"><span data-stu-id="9a720-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a720-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a720-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a720-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="9a720-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a720-136">Java</span><span class="sxs-lookup"><span data-stu-id="9a720-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a720-137">応答</span><span class="sxs-lookup"><span data-stu-id="9a720-137">Response</span></span>

<span data-ttu-id="9a720-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a720-138">The following is an example of the response.</span></span>

> <span data-ttu-id="9a720-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a720-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
