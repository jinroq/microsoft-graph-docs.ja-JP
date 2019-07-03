---
title: subscribedSku を取得する
description: 組織で取得した特定の商用サブスクリプションを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c08884a68cce7f7f85275324d23b7948654e2dd1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446193"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="b7e7a-103">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="b7e7a-103">Get subscribedSku</span></span>
<span data-ttu-id="b7e7a-104">組織で取得した特定の商用サブスクリプションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7e7a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7e7a-105">Permissions</span></span>
<span data-ttu-id="b7e7a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7e7a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7e7a-108">Permission type</span></span>      | <span data-ttu-id="b7e7a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7e7a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7e7a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7e7a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7e7a-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7e7a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7e7a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7e7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e7a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-113">Not supported.</span></span>    |
|<span data-ttu-id="b7e7a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7e7a-114">Application</span></span> | <span data-ttu-id="b7e7a-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e7a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7e7a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7e7a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7e7a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7e7a-117">Optional query parameters</span></span>
<span data-ttu-id="b7e7a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7e7a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7e7a-119">Request headers</span></span>
| <span data-ttu-id="b7e7a-120">名前</span><span class="sxs-lookup"><span data-stu-id="b7e7a-120">Name</span></span>       | <span data-ttu-id="b7e7a-121">型</span><span class="sxs-lookup"><span data-stu-id="b7e7a-121">Type</span></span> | <span data-ttu-id="b7e7a-122">説明</span><span class="sxs-lookup"><span data-stu-id="b7e7a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7e7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7e7a-123">Authorization</span></span>  | <span data-ttu-id="b7e7a-124">string</span><span class="sxs-lookup"><span data-stu-id="b7e7a-124">string</span></span>  | <span data-ttu-id="b7e7a-p102">Bearer &lt;token&gt;。*必須*</span><span class="sxs-lookup"><span data-stu-id="b7e7a-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7e7a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7e7a-127">Request body</span></span>
<span data-ttu-id="b7e7a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7e7a-129">応答</span><span class="sxs-lookup"><span data-stu-id="b7e7a-129">Response</span></span>

<span data-ttu-id="b7e7a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscribedSku](../resources/subscribedsku.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7e7a-131">例</span><span class="sxs-lookup"><span data-stu-id="b7e7a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7e7a-132">要求</span><span class="sxs-lookup"><span data-stu-id="b7e7a-132">Request</span></span>
<span data-ttu-id="b7e7a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b7e7a-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b7e7a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7e7a-135">C#</span><span class="sxs-lookup"><span data-stu-id="b7e7a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7e7a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7e7a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7e7a-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="b7e7a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b7e7a-138">応答</span><span class="sxs-lookup"><span data-stu-id="b7e7a-138">Response</span></span>
<span data-ttu-id="b7e7a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7e7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
