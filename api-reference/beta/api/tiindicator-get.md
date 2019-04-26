---
title: 脅威インテリジェンス指標の取得
description: tiindicator オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5376200bc2824d51dd1eec2a442b797836855fdb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335268"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="e8112-103">脅威インテリジェンス指標の取得</span><span class="sxs-lookup"><span data-stu-id="e8112-103">Get threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8112-104">[tiindicator](../resources/tiindicator.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8112-104">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8112-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8112-105">Permissions</span></span>

<span data-ttu-id="e8112-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8112-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8112-108">Permission type</span></span>                        | <span data-ttu-id="e8112-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8112-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8112-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8112-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8112-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e8112-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e8112-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8112-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8112-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8112-113">Not supported.</span></span> |
| <span data-ttu-id="e8112-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8112-114">Application</span></span>                            | <span data-ttu-id="e8112-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e8112-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8112-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8112-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8112-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e8112-117">Optional query parameters</span></span>

<span data-ttu-id="e8112-118">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e8112-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8112-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8112-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8112-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8112-120">Request headers</span></span>

| <span data-ttu-id="e8112-121">名前</span><span class="sxs-lookup"><span data-stu-id="e8112-121">Name</span></span>      |<span data-ttu-id="e8112-122">説明</span><span class="sxs-lookup"><span data-stu-id="e8112-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8112-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8112-123">Authorization</span></span> | <span data-ttu-id="e8112-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e8112-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8112-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8112-125">Request body</span></span>

<span data-ttu-id="e8112-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8112-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8112-127">応答</span><span class="sxs-lookup"><span data-stu-id="e8112-127">Response</span></span>

<span data-ttu-id="e8112-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e8112-128">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8112-129">例</span><span class="sxs-lookup"><span data-stu-id="e8112-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8112-130">要求</span><span class="sxs-lookup"><span data-stu-id="e8112-130">Request</span></span>

<span data-ttu-id="e8112-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8112-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="e8112-132">応答</span><span class="sxs-lookup"><span data-stu-id="e8112-132">Response</span></span>

<span data-ttu-id="e8112-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8112-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e8112-134">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="e8112-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8112-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e8112-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "action": "action-value",
  "activityGroupNames": [
    "activityGroupNames-value"
  ],
  "additionalInformation": "additionalInformation-value",
  "azureTenantId": "azureTenantId-value",
  "confidence": 99,
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
