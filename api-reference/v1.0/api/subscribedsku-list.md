---
title: subscribedSkus を一覧表示する
description: 組織で取得した商用サブスクリプションの一覧を取得します。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 360c7d1ad6242af1569e5c81bf98d06276fc5a7d
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639116"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="a2d44-103">subscribedSkus を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a2d44-103">List subscribedSkus</span></span>

<span data-ttu-id="a2d44-104">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2d44-104">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2d44-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2d44-105">Permissions</span></span>
<span data-ttu-id="a2d44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2d44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a2d44-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2d44-108">Permission type</span></span>      | <span data-ttu-id="a2d44-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2d44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2d44-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2d44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2d44-111">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2d44-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2d44-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2d44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2d44-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2d44-113">Not supported.</span></span>    |
|<span data-ttu-id="a2d44-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2d44-114">Application</span></span> | <span data-ttu-id="a2d44-115">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2d44-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2d44-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2d44-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2d44-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2d44-117">Optional query parameters</span></span>
<span data-ttu-id="a2d44-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="a2d44-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2d44-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2d44-119">Request headers</span></span>

| <span data-ttu-id="a2d44-120">名前</span><span class="sxs-lookup"><span data-stu-id="a2d44-120">Name</span></span>       | <span data-ttu-id="a2d44-121">説明</span><span class="sxs-lookup"><span data-stu-id="a2d44-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="a2d44-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2d44-122">Authorization</span></span>  | <span data-ttu-id="a2d44-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2d44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2d44-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2d44-125">Request body</span></span>
<span data-ttu-id="a2d44-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2d44-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2d44-127">応答</span><span class="sxs-lookup"><span data-stu-id="a2d44-127">Response</span></span>

<span data-ttu-id="a2d44-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscribedSku](../resources/subscribedsku.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a2d44-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2d44-129">例</span><span class="sxs-lookup"><span data-stu-id="a2d44-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2d44-130">要求</span><span class="sxs-lookup"><span data-stu-id="a2d44-130">Request</span></span>
<span data-ttu-id="a2d44-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2d44-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a2d44-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2d44-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2d44-133">C#</span><span class="sxs-lookup"><span data-stu-id="a2d44-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2d44-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2d44-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2d44-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2d44-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a2d44-136">応答</span><span class="sxs-lookup"><span data-stu-id="a2d44-136">Response</span></span>
<span data-ttu-id="a2d44-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2d44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus",
    "value": [
        {
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
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
