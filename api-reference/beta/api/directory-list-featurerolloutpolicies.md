---
title: リスト featureRolloutPolicies
description: FeatureRolloutPolicy オブジェクトのリストを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 782771ab560101996182099ace532dc08f41b10f
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062150"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="1f3f4-103">リスト featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="1f3f4-103">List featureRolloutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f3f4-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-104">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f3f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f3f4-105">Permissions</span></span>

<span data-ttu-id="1f3f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f3f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f3f4-108">Permission type</span></span>                        | <span data-ttu-id="1f3f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f3f4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f3f4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f3f4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f3f4-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f3f4-111">Policy.Read.All</span></span> |
| <span data-ttu-id="1f3f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f3f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f3f4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-113">Not supported.</span></span> |
| <span data-ttu-id="1f3f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f3f4-114">Application</span></span>                            | <span data-ttu-id="1f3f4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f3f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f3f4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f3f4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1f3f4-117">Optional query parameters</span></span>

<span data-ttu-id="1f3f4-118">このメソッドは、応答をカスタマイズするために、、、、 `$count`、 `$expand`、 `$filter`、 `$orderby`、 `$select`の`$skip`各`$top`OData クエリパラメーターをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-118">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="1f3f4-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f3f4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f3f4-120">Request headers</span></span>

| <span data-ttu-id="1f3f4-121">名前</span><span class="sxs-lookup"><span data-stu-id="1f3f4-121">Name</span></span>      |<span data-ttu-id="1f3f4-122">説明</span><span class="sxs-lookup"><span data-stu-id="1f3f4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f3f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f3f4-123">Authorization</span></span> | <span data-ttu-id="1f3f4-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1f3f4-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f3f4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f3f4-125">Request body</span></span>

<span data-ttu-id="1f3f4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f3f4-127">応答</span><span class="sxs-lookup"><span data-stu-id="1f3f4-127">Response</span></span>

<span data-ttu-id="1f3f4-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[featureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-128">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f3f4-129">例</span><span class="sxs-lookup"><span data-stu-id="1f3f4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f3f4-130">要求</span><span class="sxs-lookup"><span data-stu-id="1f3f4-130">Request</span></span>

<span data-ttu-id="1f3f4-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```

### <a name="response"></a><span data-ttu-id="1f3f4-132">応答</span><span class="sxs-lookup"><span data-stu-id="1f3f4-132">Response</span></span>

<span data-ttu-id="1f3f4-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-133">The following is an example of the response.</span></span>

> <span data-ttu-id="1f3f4-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1f3f4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
