---
title: 'tiIndicator: updateTiIndicators'
description: 複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b50699925efab2d5baf3f67d9937ee281c88d2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868151"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="06825-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="06825-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06825-104">複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを更新します。</span><span class="sxs-lookup"><span data-stu-id="06825-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="06825-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06825-105">Permissions</span></span>

<span data-ttu-id="06825-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06825-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06825-108">Permission type</span></span>   | <span data-ttu-id="06825-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="06825-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06825-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06825-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="06825-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="06825-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="06825-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06825-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06825-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06825-113">Not supported.</span></span> |
| <span data-ttu-id="06825-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06825-114">Application</span></span>                            | <span data-ttu-id="06825-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="06825-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="06825-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06825-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="06825-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06825-117">Request headers</span></span>

| <span data-ttu-id="06825-118">名前</span><span class="sxs-lookup"><span data-stu-id="06825-118">Name</span></span>          | <span data-ttu-id="06825-119">説明</span><span class="sxs-lookup"><span data-stu-id="06825-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="06825-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="06825-120">Authorization</span></span> | <span data-ttu-id="06825-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="06825-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="06825-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="06825-122">Request body</span></span>

<span data-ttu-id="06825-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="06825-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="06825-124">更新できるプロパティの詳細については、「 [Update tiIndicator](tiindicator-update.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06825-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="06825-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="06825-125">Parameter</span></span>    | <span data-ttu-id="06825-126">型</span><span class="sxs-lookup"><span data-stu-id="06825-126">Type</span></span>        | <span data-ttu-id="06825-127">説明</span><span class="sxs-lookup"><span data-stu-id="06825-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="06825-128">value</span><span class="sxs-lookup"><span data-stu-id="06825-128">value</span></span>|<span data-ttu-id="06825-129">tiIndicator コレクション</span><span class="sxs-lookup"><span data-stu-id="06825-129">tiIndicator collection</span></span>| <span data-ttu-id="06825-130">更新する**Tiindicators**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="06825-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="06825-131">各エンティティには、更新する**id**およびその他の編集可能なプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="06825-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="06825-132">応答</span><span class="sxs-lookup"><span data-stu-id="06825-132">Response</span></span>

<span data-ttu-id="06825-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="06825-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06825-134">例</span><span class="sxs-lookup"><span data-stu-id="06825-134">Examples</span></span>

<span data-ttu-id="06825-135">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="06825-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="06825-136">要求</span><span class="sxs-lookup"><span data-stu-id="06825-136">Request</span></span>

<span data-ttu-id="06825-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06825-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06825-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="06825-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators",
  "isCollection":true
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06825-139">C#</span><span class="sxs-lookup"><span data-stu-id="06825-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06825-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="06825-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06825-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="06825-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="06825-142">Java</span><span class="sxs-lookup"><span data-stu-id="06825-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-updatetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06825-143">応答</span><span class="sxs-lookup"><span data-stu-id="06825-143">Response</span></span>

<span data-ttu-id="06825-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06825-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="06825-145">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="06825-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="06825-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="06825-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
