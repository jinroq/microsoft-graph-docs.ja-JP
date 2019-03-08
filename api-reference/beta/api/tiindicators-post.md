---
title: 脅威インテリジェンス指標の作成
description: 新しい tiindicator を作成します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 440515a45b4c530f32dd20fe29497e338b54a6bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481441"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="44642-103">脅威インテリジェンス指標の作成</span><span class="sxs-lookup"><span data-stu-id="44642-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44642-104">新しい[tiindicator](../resources/tiindicator.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="44642-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44642-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44642-105">Permissions</span></span>

<span data-ttu-id="44642-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44642-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44642-108">Permission type</span></span>                        | <span data-ttu-id="44642-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44642-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44642-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44642-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="44642-111">ThreatIndicators application.readwrite.ownedby</span><span class="sxs-lookup"><span data-stu-id="44642-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="44642-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44642-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44642-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44642-113">Not supported.</span></span> |
| <span data-ttu-id="44642-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44642-114">Application</span></span>                            | <span data-ttu-id="44642-115">ThreatIndicators application.readwrite.ownedby</span><span class="sxs-lookup"><span data-stu-id="44642-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="44642-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44642-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="44642-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44642-117">Request headers</span></span>

| <span data-ttu-id="44642-118">名前</span><span class="sxs-lookup"><span data-stu-id="44642-118">Name</span></span>          | <span data-ttu-id="44642-119">説明</span><span class="sxs-lookup"><span data-stu-id="44642-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44642-120">承認</span><span class="sxs-lookup"><span data-stu-id="44642-120">Authorization</span></span> | <span data-ttu-id="44642-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="44642-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="44642-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="44642-122">Request body</span></span>

<span data-ttu-id="44642-123">要求本文で、少なくとも1つの[メール](../resources/tiindicator.md#indicator-observables---email)、[ファイル](../resources/tiindicator.md#indicator-observables---file)、または観測可能な[ネットワーク](../resources/tiindicator.md#indicator-observables---network)を含む[tiindicator](../resources/tiindicator.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44642-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="44642-124">応答</span><span class="sxs-lookup"><span data-stu-id="44642-124">Response</span></span>

<span data-ttu-id="44642-125">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44642-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44642-126">例</span><span class="sxs-lookup"><span data-stu-id="44642-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44642-127">要求</span><span class="sxs-lookup"><span data-stu-id="44642-127">Request</span></span>

<span data-ttu-id="44642-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44642-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```

### <a name="response"></a><span data-ttu-id="44642-129">応答</span><span class="sxs-lookup"><span data-stu-id="44642-129">Response</span></span>

<span data-ttu-id="44642-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44642-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="44642-131">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="44642-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="44642-132">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="44642-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
