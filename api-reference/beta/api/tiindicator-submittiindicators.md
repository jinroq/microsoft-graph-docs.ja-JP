---
title: 'tiIndicator: submitTiIndicators'
description: 複数の脅威インテリジェンス (TI) インジケーターを、複数の要求ではなく1つの要求でアップロードします。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4b0067aeb0945db706ff24c667489f33ce49feff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987909"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="c9aa1-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="c9aa1-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9aa1-104">複数の脅威インテリジェンス (TI) インジケーターを、複数の要求ではなく1つの要求でアップロードします。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9aa1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c9aa1-105">Permissions</span></span>

<span data-ttu-id="c9aa1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9aa1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9aa1-108">Permission type</span></span> | <span data-ttu-id="c9aa1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9aa1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c9aa1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9aa1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9aa1-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c9aa1-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c9aa1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9aa1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9aa1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-113">Not supported.</span></span> |
| <span data-ttu-id="c9aa1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9aa1-114">Application</span></span>                            | <span data-ttu-id="c9aa1-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c9aa1-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9aa1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9aa1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="c9aa1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9aa1-117">Request headers</span></span>

| <span data-ttu-id="c9aa1-118">名前</span><span class="sxs-lookup"><span data-stu-id="c9aa1-118">Name</span></span>          | <span data-ttu-id="c9aa1-119">説明</span><span class="sxs-lookup"><span data-stu-id="c9aa1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c9aa1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9aa1-120">Authorization</span></span> | <span data-ttu-id="c9aa1-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c9aa1-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9aa1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9aa1-122">Request body</span></span>

<span data-ttu-id="c9aa1-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9aa1-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c9aa1-124">Parameter</span></span>    | <span data-ttu-id="c9aa1-125">型</span><span class="sxs-lookup"><span data-stu-id="c9aa1-125">Type</span></span>        | <span data-ttu-id="c9aa1-126">説明</span><span class="sxs-lookup"><span data-stu-id="c9aa1-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9aa1-127">value</span><span class="sxs-lookup"><span data-stu-id="c9aa1-127">value</span></span>|<span data-ttu-id="c9aa1-128">tiIndicator コレクション</span><span class="sxs-lookup"><span data-stu-id="c9aa1-128">tiIndicator collection</span></span>| <span data-ttu-id="c9aa1-129">作成する**tiindicators**の JSON コレクション。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-129">JSON collection of **tiIndicators** to be created.</span></span> |

## <a name="response"></a><span data-ttu-id="c9aa1-130">応答</span><span class="sxs-lookup"><span data-stu-id="c9aa1-130">Response</span></span>

<span data-ttu-id="c9aa1-131">成功した場合、この`200, OK`メソッドは応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-131">If successful, this method returns `200, OK` response code and a [tiIndicator](../resources/tiindicator.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9aa1-132">例</span><span class="sxs-lookup"><span data-stu-id="c9aa1-132">Examples</span></span>

<span data-ttu-id="c9aa1-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c9aa1-134">要求</span><span class="sxs-lookup"><span data-stu-id="c9aa1-134">Request</span></span>

<span data-ttu-id="c9aa1-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9aa1-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c9aa1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-Type: application/json

{
  "value": [
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1668987+00:00",
      "externalId": "Test--8586509942423126760MS164-0",
      "fileHashType": "sha256",
      "fileHashValue": "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    },
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1748779+00:00",
      "externalId": "Test--8586509942423126760MS164-1",
      "fileHashType": "sha256",
      "fileHashValue": "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9aa1-137">C#</span><span class="sxs-lookup"><span data-stu-id="c9aa1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9aa1-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9aa1-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9aa1-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="c9aa1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9aa1-140">Java</span><span class="sxs-lookup"><span data-stu-id="c9aa1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-submittiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9aa1-141">応答</span><span class="sxs-lookup"><span data-stu-id="c9aa1-141">Response</span></span>

<span data-ttu-id="c9aa1-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c9aa1-143">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c9aa1-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c9aa1-144">All the properties will be returned from an actual call.</span></span>

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
      "azureTenantId": "XXXXXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": null,
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
  "description": "tiIndicator: submitTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
