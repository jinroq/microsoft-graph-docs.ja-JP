---
title: 'tiIndicator: updateTiIndicators'
description: 複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ac40a7690a70e49ae823779bf86569e078c4a3db
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637592"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="c1e8f-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="c1e8f-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1e8f-104">複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1e8f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c1e8f-105">Permissions</span></span>

<span data-ttu-id="c1e8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1e8f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1e8f-108">Permission type</span></span>   | <span data-ttu-id="c1e8f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1e8f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1e8f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1e8f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1e8f-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c1e8f-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c1e8f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1e8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1e8f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-113">Not supported.</span></span> |
| <span data-ttu-id="c1e8f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1e8f-114">Application</span></span>                            | <span data-ttu-id="c1e8f-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c1e8f-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1e8f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1e8f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="c1e8f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1e8f-117">Request headers</span></span>

| <span data-ttu-id="c1e8f-118">名前</span><span class="sxs-lookup"><span data-stu-id="c1e8f-118">Name</span></span>          | <span data-ttu-id="c1e8f-119">説明</span><span class="sxs-lookup"><span data-stu-id="c1e8f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c1e8f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1e8f-120">Authorization</span></span> | <span data-ttu-id="c1e8f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c1e8f-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1e8f-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1e8f-122">Request body</span></span>

<span data-ttu-id="c1e8f-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="c1e8f-124">更新できるプロパティの詳細については、「 [Update tiIndicator](tiindicator-update.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="c1e8f-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c1e8f-125">Parameter</span></span>    | <span data-ttu-id="c1e8f-126">型</span><span class="sxs-lookup"><span data-stu-id="c1e8f-126">Type</span></span>        | <span data-ttu-id="c1e8f-127">説明</span><span class="sxs-lookup"><span data-stu-id="c1e8f-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1e8f-128">value</span><span class="sxs-lookup"><span data-stu-id="c1e8f-128">value</span></span>|<span data-ttu-id="c1e8f-129">tiIndicator コレクション</span><span class="sxs-lookup"><span data-stu-id="c1e8f-129">tiIndicator collection</span></span>| <span data-ttu-id="c1e8f-130">更新する**Tiindicators**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="c1e8f-131">各エンティティには、更新する**id**およびその他の編集可能なプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="c1e8f-132">応答</span><span class="sxs-lookup"><span data-stu-id="c1e8f-132">Response</span></span>

<span data-ttu-id="c1e8f-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1e8f-134">例</span><span class="sxs-lookup"><span data-stu-id="c1e8f-134">Examples</span></span>

<span data-ttu-id="c1e8f-135">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c1e8f-136">要求</span><span class="sxs-lookup"><span data-stu-id="c1e8f-136">Request</span></span>

<span data-ttu-id="c1e8f-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1e8f-138">応答</span><span class="sxs-lookup"><span data-stu-id="c1e8f-138">Response</span></span>

<span data-ttu-id="c1e8f-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c1e8f-140">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1e8f-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c1e8f-141">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c1e8f-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c1e8f-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c1e8f-143">Visual</span><span class="sxs-lookup"><span data-stu-id="c1e8f-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_updatetiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1e8f-144">Java</span><span class="sxs-lookup"><span data-stu-id="c1e8f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_updatetiindicators-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-updatetiindicators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-updatetiindicators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
