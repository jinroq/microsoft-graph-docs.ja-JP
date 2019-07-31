---
title: 顧客を作成する
description: Dynamics 365 Business Central に customer オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 5aab0dab11d1b56a9eb230836fe157f87a99a07e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956724"
---
# <a name="create-customers"></a><span data-ttu-id="04112-103">顧客を作成する</span><span class="sxs-lookup"><span data-stu-id="04112-103">Create customers</span></span>
<span data-ttu-id="04112-104">Dynamics 365 Business Central で customer オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="04112-104">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="04112-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04112-105">Permissions</span></span>
<span data-ttu-id="04112-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04112-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04112-108">Permission type</span></span> |<span data-ttu-id="04112-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04112-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="04112-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04112-110">Delegated (work or school account)</span></span>|<span data-ttu-id="04112-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04112-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="04112-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="04112-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="04112-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04112-113">Not supported.</span></span>|
|<span data-ttu-id="04112-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04112-114">Application</span></span>|<span data-ttu-id="04112-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04112-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04112-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04112-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04112-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="04112-117">Optional query parameters</span></span>
<span data-ttu-id="04112-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="04112-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04112-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04112-119">Request headers</span></span>
|<span data-ttu-id="04112-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04112-120">Header</span></span>         |<span data-ttu-id="04112-121">値</span><span class="sxs-lookup"><span data-stu-id="04112-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="04112-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04112-122">Authorization</span></span>  |<span data-ttu-id="04112-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04112-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04112-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04112-125">Content-Type</span></span>   |<span data-ttu-id="04112-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04112-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="04112-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04112-127">Request body</span></span>
<span data-ttu-id="04112-128">要求本文で、 **customers**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04112-128">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="04112-129">応答</span><span class="sxs-lookup"><span data-stu-id="04112-129">Response</span></span>
<span data-ttu-id="04112-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**customers**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04112-130">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04112-131">例</span><span class="sxs-lookup"><span data-stu-id="04112-131">Example</span></span>

<span data-ttu-id="04112-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="04112-132">**Request**</span></span>

<span data-ttu-id="04112-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="04112-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customers
Content-type: application/json

{
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
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
}

```

<span data-ttu-id="04112-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="04112-134">**Response**</span></span>

<span data-ttu-id="04112-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04112-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="04112-136">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="04112-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04112-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="04112-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

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
  "currencyCode": "USD",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}

```

