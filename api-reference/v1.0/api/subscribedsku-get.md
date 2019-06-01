---
title: subscribedSku を取得する
description: 組織で取得した特定の商用サブスクリプションを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db970aa787626c835c3dea88d07a7ee663a4b8cf
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655706"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="0ea4d-103">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="0ea4d-103">Get subscribedSku</span></span>
<span data-ttu-id="0ea4d-104">組織で取得した特定の商用サブスクリプションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea4d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0ea4d-105">Permissions</span></span>
<span data-ttu-id="0ea4d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0ea4d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ea4d-108">Permission type</span></span>      | <span data-ttu-id="0ea4d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ea4d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea4d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea4d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea4d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ea4d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ea4d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea4d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea4d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-113">Not supported.</span></span>    |
|<span data-ttu-id="0ea4d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ea4d-114">Application</span></span> | <span data-ttu-id="0ea4d-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea4d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea4d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ea4d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ea4d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0ea4d-117">Optional query parameters</span></span>
<span data-ttu-id="0ea4d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea4d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea4d-119">Request headers</span></span>
| <span data-ttu-id="0ea4d-120">名前</span><span class="sxs-lookup"><span data-stu-id="0ea4d-120">Name</span></span>       | <span data-ttu-id="0ea4d-121">型</span><span class="sxs-lookup"><span data-stu-id="0ea4d-121">Type</span></span> | <span data-ttu-id="0ea4d-122">説明</span><span class="sxs-lookup"><span data-stu-id="0ea4d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ea4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea4d-123">Authorization</span></span>  | <span data-ttu-id="0ea4d-124">string</span><span class="sxs-lookup"><span data-stu-id="0ea4d-124">string</span></span>  | <span data-ttu-id="0ea4d-p102">Bearer &lt;token&gt;。*必須*</span><span class="sxs-lookup"><span data-stu-id="0ea4d-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ea4d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ea4d-127">Request body</span></span>
<span data-ttu-id="0ea4d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea4d-129">応答</span><span class="sxs-lookup"><span data-stu-id="0ea4d-129">Response</span></span>

<span data-ttu-id="0ea4d-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscribedSku](../resources/subscribedsku.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ea4d-131">例</span><span class="sxs-lookup"><span data-stu-id="0ea4d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ea4d-132">要求</span><span class="sxs-lookup"><span data-stu-id="0ea4d-132">Request</span></span>
<span data-ttu-id="0ea4d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="0ea4d-134">応答</span><span class="sxs-lookup"><span data-stu-id="0ea4d-134">Response</span></span>
<span data-ttu-id="0ea4d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus/$entity",
    "capabilityStatus": "Enabled",
    "consumedUnits": 14,
    "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
    "prepaidUnits": {
        "enabled": 25,
        "suspended": 0,
        "warning": 0
    },
    "servicePlans": [
        {
            "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
            "servicePlanName": "ADALLOM_S_O365",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ea4d-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0ea4d-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ea4d-139">C#</span><span class="sxs-lookup"><span data-stu-id="0ea4d-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ea4d-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ea4d-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
