---
title: AppliesTo を割り当てる
description: 機能のロールアウトに directoryObject を割り当てます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efdc9e04e7e8554ef6acf5f3df7b2292b2c618e1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323571"
---
# <a name="assign-appliesto"></a><span data-ttu-id="89428-103">AppliesTo を割り当てる</span><span class="sxs-lookup"><span data-stu-id="89428-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89428-104">[FeatureRolloutPolicy](../resources/featurerolloutpolicy.md)オブジェクトに appliesTo を追加して、 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)を適用する必要がある[directoryobject](../resources/directoryobject.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="89428-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="89428-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89428-105">Permissions</span></span>

<span data-ttu-id="89428-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89428-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89428-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89428-108">Permission type</span></span>                        | <span data-ttu-id="89428-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89428-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89428-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89428-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="89428-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="89428-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="89428-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89428-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89428-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89428-113">Not supported.</span></span> |
| <span data-ttu-id="89428-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89428-114">Application</span></span>                            | <span data-ttu-id="89428-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89428-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89428-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89428-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="89428-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89428-117">Request headers</span></span>

| <span data-ttu-id="89428-118">名前</span><span class="sxs-lookup"><span data-stu-id="89428-118">Name</span></span>          | <span data-ttu-id="89428-119">説明</span><span class="sxs-lookup"><span data-stu-id="89428-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="89428-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="89428-120">Authorization</span></span> | <span data-ttu-id="89428-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="89428-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="89428-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="89428-122">Request body</span></span>

<span data-ttu-id="89428-123">要求本文で、 [directoryobject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="89428-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89428-124">応答</span><span class="sxs-lookup"><span data-stu-id="89428-124">Response</span></span>

<span data-ttu-id="89428-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[directoryobject](../resources/directoryobject.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89428-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89428-126">例</span><span class="sxs-lookup"><span data-stu-id="89428-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89428-127">要求</span><span class="sxs-lookup"><span data-stu-id="89428-127">Request</span></span>

<span data-ttu-id="89428-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89428-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89428-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="89428-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="89428-130">C#</span><span class="sxs-lookup"><span data-stu-id="89428-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89428-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89428-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89428-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="89428-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89428-133">Java</span><span class="sxs-lookup"><span data-stu-id="89428-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89428-134">応答</span><span class="sxs-lookup"><span data-stu-id="89428-134">Response</span></span>

<span data-ttu-id="89428-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89428-135">The following is an example of the response.</span></span>

> <span data-ttu-id="89428-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89428-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
