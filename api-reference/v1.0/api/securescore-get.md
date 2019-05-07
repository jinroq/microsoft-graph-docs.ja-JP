---
title: SecureScore を取得する
description: SecureScore オブジェクトのプロパティとリレーションシップを取得します。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 48b6f74fb298a0b9064f2abc7b2c8055ea60b6a8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629762"
---
# <a name="get-securescore"></a><span data-ttu-id="93cea-103">SecureScore を取得する</span><span class="sxs-lookup"><span data-stu-id="93cea-103">Get secureScore</span></span>

<span data-ttu-id="93cea-104">[SecureScore](../resources/securescore.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="93cea-104">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93cea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93cea-105">Permissions</span></span>

<span data-ttu-id="93cea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93cea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93cea-108">Permission type</span></span>      | <span data-ttu-id="93cea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93cea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93cea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93cea-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="93cea-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93cea-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="93cea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93cea-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93cea-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93cea-113">Not supported.</span></span>  |
|<span data-ttu-id="93cea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93cea-114">Application</span></span> | <span data-ttu-id="93cea-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93cea-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93cea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93cea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93cea-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93cea-117">Request headers</span></span>

| <span data-ttu-id="93cea-118">名前</span><span class="sxs-lookup"><span data-stu-id="93cea-118">Name</span></span>      |<span data-ttu-id="93cea-119">説明</span><span class="sxs-lookup"><span data-stu-id="93cea-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93cea-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="93cea-120">Authorization</span></span>  | <span data-ttu-id="93cea-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="93cea-121">Bearer {code}.</span></span> <span data-ttu-id="93cea-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="93cea-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93cea-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="93cea-123">Request body</span></span>

<span data-ttu-id="93cea-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="93cea-124">Do not supply a request body for this method.</span></span> <span data-ttu-id="93cea-125">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="93cea-125">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="93cea-126">応答</span><span class="sxs-lookup"><span data-stu-id="93cea-126">Response</span></span>

<span data-ttu-id="93cea-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScore**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="93cea-127">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="93cea-128">プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に`206 Partial Content` 状態コードになります。</span><span class="sxs-lookup"><span data-stu-id="93cea-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="93cea-129">詳細については、[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93cea-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="93cea-130">例</span><span class="sxs-lookup"><span data-stu-id="93cea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="93cea-131">要求</span><span class="sxs-lookup"><span data-stu-id="93cea-131">Request</span></span>

<span data-ttu-id="93cea-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93cea-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```

### <a name="response"></a><span data-ttu-id="93cea-133">応答</span><span class="sxs-lookup"><span data-stu-id="93cea-133">Response</span></span>

<span data-ttu-id="93cea-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93cea-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "activeUserCount": 0,
  "createdDateTime": "2019-03-19T15:21:00Z",
  "currentScore": 387.0,
  "enabledServices": [
    "HasExchange",
    "HasSharePoint",
    "HasInTune"
  ],
  "licensedUserCount": 100,
  "maxScore": 697.0,
  "averageComparativeScores": [
    {
      "basis": "AllTenants",
      "averageScore": 37.0
    },
    {
      "basis": "TotalSeats",
      "averageScore": 46.0
    },
    {
      "basis": "IndustryTypes",
      "averageScore": 109.0
    }
  ],
  "controlScores": [
    {
      "controlCategory": "Identity",
      "controlName": "AdminMFA",
      "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
      "score": 35.0
    },
    {
      "controlCategory": "Data",
      "controlName": "DLPEnabled",
      "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
      "score": 20.0
    }
  ],
"vendorInformation": {
  "provider": "SecureScore",
  "providerVersion": null,
  "subProvider": null,
  "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
