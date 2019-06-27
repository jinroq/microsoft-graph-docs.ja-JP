---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: 複数の要求ではなく1つの要求で複数の脅威インテリジェンス (TI) インジケーターを削除し、要求には Id ではなく外部 Id が含まれます。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 835bc4bfdda1cda355b907e0cdf143d09bbc0ccb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270687"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="086f2-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="086f2-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="086f2-104">要求に Id ではなく外部 Id が含まれている場合は、複数の要求ではなく、1つの要求で複数の脅威インテリジェンス (TI) インジケーターを削除します。</span><span class="sxs-lookup"><span data-stu-id="086f2-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="086f2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="086f2-105">Permissions</span></span>

<span data-ttu-id="086f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="086f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="086f2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="086f2-108">Permission type</span></span>  | <span data-ttu-id="086f2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="086f2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="086f2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="086f2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="086f2-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="086f2-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="086f2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="086f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="086f2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="086f2-113">Not supported.</span></span> |
| <span data-ttu-id="086f2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="086f2-114">Application</span></span>                            | <span data-ttu-id="086f2-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="086f2-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="086f2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="086f2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="086f2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="086f2-117">Request headers</span></span>

| <span data-ttu-id="086f2-118">名前</span><span class="sxs-lookup"><span data-stu-id="086f2-118">Name</span></span>          | <span data-ttu-id="086f2-119">説明</span><span class="sxs-lookup"><span data-stu-id="086f2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="086f2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="086f2-120">Authorization</span></span> | <span data-ttu-id="086f2-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="086f2-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="086f2-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="086f2-122">Request body</span></span>

<span data-ttu-id="086f2-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="086f2-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="086f2-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="086f2-124">Parameter</span></span>    | <span data-ttu-id="086f2-125">型</span><span class="sxs-lookup"><span data-stu-id="086f2-125">Type</span></span>        | <span data-ttu-id="086f2-126">説明</span><span class="sxs-lookup"><span data-stu-id="086f2-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="086f2-127">value</span><span class="sxs-lookup"><span data-stu-id="086f2-127">value</span></span>|<span data-ttu-id="086f2-128">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="086f2-128">String collection</span></span>| <span data-ttu-id="086f2-129">`externalIds`削除する**tiindicator**オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="086f2-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="086f2-130">応答</span><span class="sxs-lookup"><span data-stu-id="086f2-130">Response</span></span>

<span data-ttu-id="086f2-131">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[resultinfo](../resources/resultinfo.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="086f2-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="086f2-132">例</span><span class="sxs-lookup"><span data-stu-id="086f2-132">Examples</span></span>

<span data-ttu-id="086f2-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="086f2-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="086f2-134">要求</span><span class="sxs-lookup"><span data-stu-id="086f2-134">Request</span></span>

<span data-ttu-id="086f2-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="086f2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="086f2-136">応答</span><span class="sxs-lookup"><span data-stu-id="086f2-136">Response</span></span>

<span data-ttu-id="086f2-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="086f2-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="086f2-138">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="086f2-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="086f2-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="086f2-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="086f2-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="086f2-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="086f2-141">C#</span><span class="sxs-lookup"><span data-stu-id="086f2-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="086f2-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="086f2-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="086f2-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="086f2-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
