---
title: 組織を取得する
description: 現在認証されている組織のプロパティとリレーションシップを取得します。
localization_priority: Priority
ms.openlocfilehash: f2fc708ea2d1841987f8b2a757a5388735227007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871198"
---
# <a name="get-organization"></a><span data-ttu-id="10678-103">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="10678-103">Get organization</span></span>

<span data-ttu-id="10678-104">現在認証されている組織のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="10678-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="10678-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="10678-105">Permissions</span></span>

<span data-ttu-id="10678-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10678-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="10678-108">Permission type</span></span>      | <span data-ttu-id="10678-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="10678-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10678-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="10678-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10678-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10678-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="10678-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="10678-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10678-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10678-113">Not supported.</span></span>    |
|<span data-ttu-id="10678-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="10678-114">Application</span></span> | <span data-ttu-id="10678-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10678-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="10678-116">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="10678-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="10678-117">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="10678-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="10678-118">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="10678-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="10678-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="10678-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10678-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="10678-120">Optional query parameters</span></span>

<span data-ttu-id="10678-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="10678-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10678-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="10678-122">Request headers</span></span>

| <span data-ttu-id="10678-123">名前</span><span class="sxs-lookup"><span data-stu-id="10678-123">Name</span></span>       | <span data-ttu-id="10678-124">種類</span><span class="sxs-lookup"><span data-stu-id="10678-124">Type</span></span> | <span data-ttu-id="10678-125">説明</span><span class="sxs-lookup"><span data-stu-id="10678-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10678-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="10678-126">Authorization</span></span>  | <span data-ttu-id="10678-127">string</span><span class="sxs-lookup"><span data-stu-id="10678-127">string</span></span>  | <span data-ttu-id="10678-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="10678-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10678-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="10678-130">Request body</span></span>

<span data-ttu-id="10678-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="10678-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10678-132">応答</span><span class="sxs-lookup"><span data-stu-id="10678-132">Response</span></span>

<span data-ttu-id="10678-133">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の 1 つの[組織](../resources/organization.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="10678-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10678-134">例</span><span class="sxs-lookup"><span data-stu-id="10678-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10678-135">要求</span><span class="sxs-lookup"><span data-stu-id="10678-135">Request</span></span>

<span data-ttu-id="10678-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="10678-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```

##### <a name="response"></a><span data-ttu-id="10678-137">応答</span><span class="sxs-lookup"><span data-stu-id="10678-137">Response</span></span>

<span data-ttu-id="10678-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="10678-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
