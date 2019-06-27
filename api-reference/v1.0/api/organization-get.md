---
title: 組織を取得する
description: 現在認証されている組織のプロパティとリレーションシップを取得します。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6233a9fdf9db149a622b95eb18962bc16c355624
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274411"
---
# <a name="get-organization"></a><span data-ttu-id="bdbe6-103">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="bdbe6-103">Get organization</span></span>

<span data-ttu-id="bdbe6-104">現在認証されている組織のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdbe6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bdbe6-105">Permissions</span></span>

<span data-ttu-id="bdbe6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdbe6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdbe6-108">Permission type</span></span>      | <span data-ttu-id="bdbe6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdbe6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdbe6-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdbe6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdbe6-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdbe6-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="bdbe6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdbe6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdbe6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-113">Not supported.</span></span>    |
|<span data-ttu-id="bdbe6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdbe6-114">Application</span></span> | <span data-ttu-id="bdbe6-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdbe6-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bdbe6-116">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="bdbe6-117">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="bdbe6-118">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="bdbe6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdbe6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bdbe6-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bdbe6-120">Optional query parameters</span></span>

<span data-ttu-id="bdbe6-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdbe6-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdbe6-122">Request headers</span></span>

| <span data-ttu-id="bdbe6-123">名前</span><span class="sxs-lookup"><span data-stu-id="bdbe6-123">Name</span></span>       | <span data-ttu-id="bdbe6-124">型</span><span class="sxs-lookup"><span data-stu-id="bdbe6-124">Type</span></span> | <span data-ttu-id="bdbe6-125">説明</span><span class="sxs-lookup"><span data-stu-id="bdbe6-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bdbe6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdbe6-126">Authorization</span></span>  | <span data-ttu-id="bdbe6-127">string</span><span class="sxs-lookup"><span data-stu-id="bdbe6-127">string</span></span>  | <span data-ttu-id="bdbe6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdbe6-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdbe6-130">Request body</span></span>

<span data-ttu-id="bdbe6-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdbe6-132">応答</span><span class="sxs-lookup"><span data-stu-id="bdbe6-132">Response</span></span>

<span data-ttu-id="bdbe6-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で 1 つの [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdbe6-134">例</span><span class="sxs-lookup"><span data-stu-id="bdbe6-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bdbe6-135">要求</span><span class="sxs-lookup"><span data-stu-id="bdbe6-135">Request</span></span>

<span data-ttu-id="bdbe6-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```

##### <a name="response"></a><span data-ttu-id="bdbe6-137">応答</span><span class="sxs-lookup"><span data-stu-id="bdbe6-137">Response</span></span>

<span data-ttu-id="bdbe6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bdbe6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bdbe6-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="bdbe6-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bdbe6-142">C#</span><span class="sxs-lookup"><span data-stu-id="bdbe6-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdbe6-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="bdbe6-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bdbe6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdbe6-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
