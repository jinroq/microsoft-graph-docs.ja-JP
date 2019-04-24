---
title: 顧客を取得する
description: Dynamics 365 Business Central の customer オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0512a493032e738bba41362ecdc40e78de951baf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458594"
---
# <a name="get-customers"></a><span data-ttu-id="59a8d-103">顧客を取得する</span><span class="sxs-lookup"><span data-stu-id="59a8d-103">Get customers</span></span>
<span data-ttu-id="59a8d-104">Dynamics 365 Business Central の customer オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="59a8d-104">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="59a8d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59a8d-105">Permissions</span></span>
<span data-ttu-id="59a8d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59a8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a8d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59a8d-108">Permission type</span></span> |<span data-ttu-id="59a8d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59a8d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="59a8d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59a8d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="59a8d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a8d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="59a8d-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="59a8d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="59a8d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59a8d-113">Not supported.</span></span>|
|<span data-ttu-id="59a8d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59a8d-114">Application</span></span>|<span data-ttu-id="59a8d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a8d-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59a8d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59a8d-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/customers('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59a8d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="59a8d-117">Optional query parameters</span></span>
<span data-ttu-id="59a8d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59a8d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59a8d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59a8d-119">Request headers</span></span>
|<span data-ttu-id="59a8d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59a8d-120">Header</span></span>|<span data-ttu-id="59a8d-121">値</span><span class="sxs-lookup"><span data-stu-id="59a8d-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="59a8d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59a8d-122">Authorization</span></span>  |<span data-ttu-id="59a8d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59a8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59a8d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="59a8d-125">Request body</span></span>
<span data-ttu-id="59a8d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="59a8d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59a8d-127">応答</span><span class="sxs-lookup"><span data-stu-id="59a8d-127">Response</span></span>
<span data-ttu-id="59a8d-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**customers**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="59a8d-128">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="59a8d-129">**要求**</span><span class="sxs-lookup"><span data-stu-id="59a8d-129">**Request**</span></span>

<span data-ttu-id="59a8d-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59a8d-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customers('{id}')
```

<span data-ttu-id="59a8d-131">**応答**</span><span class="sxs-lookup"><span data-stu-id="59a8d-131">**Response**</span></span>

<span data-ttu-id="59a8d-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="59a8d-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="59a8d-133">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="59a8d-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59a8d-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="59a8d-134">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```

