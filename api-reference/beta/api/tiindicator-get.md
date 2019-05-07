---
title: 脅威インテリジェンス指標の取得
description: Tiindicator オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 74501125b5504b365281cfee5fa12f6169b1c2aa
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637564"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="cd9d0-103">脅威インテリジェンス指標の取得</span><span class="sxs-lookup"><span data-stu-id="cd9d0-103">Get threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd9d0-104">[Tiindicator](../resources/tiindicator.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-104">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd9d0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cd9d0-105">Permissions</span></span>

<span data-ttu-id="cd9d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd9d0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd9d0-108">Permission type</span></span>                        | <span data-ttu-id="cd9d0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd9d0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cd9d0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd9d0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd9d0-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cd9d0-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="cd9d0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd9d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd9d0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-113">Not supported.</span></span> |
| <span data-ttu-id="cd9d0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd9d0-114">Application</span></span>                            | <span data-ttu-id="cd9d0-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cd9d0-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd9d0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd9d0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd9d0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cd9d0-117">Optional query parameters</span></span>

<span data-ttu-id="cd9d0-118">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cd9d0-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd9d0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd9d0-120">Request headers</span></span>

| <span data-ttu-id="cd9d0-121">名前</span><span class="sxs-lookup"><span data-stu-id="cd9d0-121">Name</span></span>      |<span data-ttu-id="cd9d0-122">説明</span><span class="sxs-lookup"><span data-stu-id="cd9d0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cd9d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd9d0-123">Authorization</span></span> | <span data-ttu-id="cd9d0-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cd9d0-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd9d0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd9d0-125">Request body</span></span>

<span data-ttu-id="cd9d0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd9d0-127">応答</span><span class="sxs-lookup"><span data-stu-id="cd9d0-127">Response</span></span>

<span data-ttu-id="cd9d0-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tiindicator](../resources/tiindicator.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-128">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd9d0-129">例</span><span class="sxs-lookup"><span data-stu-id="cd9d0-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd9d0-130">要求</span><span class="sxs-lookup"><span data-stu-id="cd9d0-130">Request</span></span>

<span data-ttu-id="cd9d0-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="cd9d0-132">応答</span><span class="sxs-lookup"><span data-stu-id="cd9d0-132">Response</span></span>

<span data-ttu-id="cd9d0-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cd9d0-134">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cd9d0-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cd9d0-135">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cd9d0-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="cd9d0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cd9d0-137">Visual</span><span class="sxs-lookup"><span data-stu-id="cd9d0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd9d0-138">Java</span><span class="sxs-lookup"><span data-stu-id="cd9d0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tiindicator-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
