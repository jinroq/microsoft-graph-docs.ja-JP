---
title: subscribedSku を取得する
description: 組織で取得した特定の商用サブスクリプションを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ae0d4fbd302be8952ddeb91350a62d9b5933201
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409918"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="2d55d-103">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="2d55d-103">Get subscribedSku</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d55d-104">組織が取得した特定の商用サブスクリプションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2d55d-104">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d55d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2d55d-105">Permissions</span></span>
<span data-ttu-id="2d55d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d55d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2d55d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d55d-108">Permission type</span></span>      | <span data-ttu-id="2d55d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d55d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d55d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d55d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d55d-111">Directory.accessasuser.all。すべて、ディレクトリの読み取り、すべてのディレクトリを取得します。すべての</span><span class="sxs-lookup"><span data-stu-id="2d55d-111">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d55d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d55d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d55d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d55d-113">Not supported.</span></span>    |
|<span data-ttu-id="2d55d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d55d-114">Application</span></span> | <span data-ttu-id="2d55d-115">。すべて、ディレクトリの読み取り、すべての読み取り、すべての書き込み、すべての.</span><span class="sxs-lookup"><span data-stu-id="2d55d-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d55d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d55d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d55d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2d55d-117">Optional query parameters</span></span>
<span data-ttu-id="2d55d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2d55d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2d55d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d55d-119">Request headers</span></span>

| <span data-ttu-id="2d55d-120">名前</span><span class="sxs-lookup"><span data-stu-id="2d55d-120">Name</span></span>       | <span data-ttu-id="2d55d-121">説明</span><span class="sxs-lookup"><span data-stu-id="2d55d-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="2d55d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d55d-122">Authorization</span></span>  | <span data-ttu-id="2d55d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2d55d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d55d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d55d-125">Request body</span></span>
<span data-ttu-id="2d55d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2d55d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d55d-127">応答</span><span class="sxs-lookup"><span data-stu-id="2d55d-127">Response</span></span>

<span data-ttu-id="2d55d-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscribedSku](../resources/subscribedsku.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d55d-128">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d55d-129">例</span><span class="sxs-lookup"><span data-stu-id="2d55d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d55d-130">要求</span><span class="sxs-lookup"><span data-stu-id="2d55d-130">Request</span></span>
<span data-ttu-id="2d55d-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d55d-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d55d-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2d55d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d55d-133">C#</span><span class="sxs-lookup"><span data-stu-id="2d55d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d55d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d55d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d55d-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="2d55d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d55d-136">応答</span><span class="sxs-lookup"><span data-stu-id="2d55d-136">Response</span></span>
<span data-ttu-id="2d55d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d55d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 450

{
  "capabilityStatus": "capabilityStatus-value",
  "consumedUnits": 99,
  "prepaidUnits": {
    "enabled": 99,
    "suspended": 99,
    "warning": 99
  },
  "servicePlans": [
    {
      "servicePlanId": "servicePlanId-value",
      "servicePlanName": "servicePlanName-value",
      "provisioningStatus": "provisioningStatus-value",
      "appliesTo": "appliesTo-value"
    }
  ],
  "skuId": "skuId-value",
  "skuPartNumber": "skuPartNumber-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
