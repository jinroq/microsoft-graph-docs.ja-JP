---
title: 脅威インテリジェンス指標の取得
description: Tiindicator オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: f192327d12f68a72686808db480f82c2907e45da
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868222"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="89e47-103">脅威インテリジェンス指標の取得</span><span class="sxs-lookup"><span data-stu-id="89e47-103">Get threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e47-104">[Tiindicator](../resources/tiindicator.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="89e47-104">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89e47-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89e47-105">Permissions</span></span>

<span data-ttu-id="89e47-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89e47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89e47-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89e47-108">Permission type</span></span>                        | <span data-ttu-id="89e47-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89e47-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89e47-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89e47-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="89e47-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="89e47-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="89e47-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89e47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e47-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89e47-113">Not supported.</span></span> |
| <span data-ttu-id="89e47-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89e47-114">Application</span></span>                            | <span data-ttu-id="89e47-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="89e47-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="89e47-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89e47-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89e47-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="89e47-117">Optional query parameters</span></span>

<span data-ttu-id="89e47-118">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="89e47-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="89e47-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89e47-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89e47-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89e47-120">Request headers</span></span>

| <span data-ttu-id="89e47-121">名前</span><span class="sxs-lookup"><span data-stu-id="89e47-121">Name</span></span>      |<span data-ttu-id="89e47-122">説明</span><span class="sxs-lookup"><span data-stu-id="89e47-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89e47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e47-123">Authorization</span></span> | <span data-ttu-id="89e47-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="89e47-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="89e47-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="89e47-125">Request body</span></span>

<span data-ttu-id="89e47-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89e47-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89e47-127">応答</span><span class="sxs-lookup"><span data-stu-id="89e47-127">Response</span></span>

<span data-ttu-id="89e47-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89e47-128">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89e47-129">例</span><span class="sxs-lookup"><span data-stu-id="89e47-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89e47-130">要求</span><span class="sxs-lookup"><span data-stu-id="89e47-130">Request</span></span>

<span data-ttu-id="89e47-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89e47-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89e47-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="89e47-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89e47-133">C#</span><span class="sxs-lookup"><span data-stu-id="89e47-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89e47-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="89e47-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89e47-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="89e47-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89e47-136">Java</span><span class="sxs-lookup"><span data-stu-id="89e47-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89e47-137">応答</span><span class="sxs-lookup"><span data-stu-id="89e47-137">Response</span></span>

<span data-ttu-id="89e47-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89e47-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="89e47-139">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="89e47-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89e47-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89e47-140">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
