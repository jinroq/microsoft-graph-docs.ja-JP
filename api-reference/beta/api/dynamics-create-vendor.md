---
title: 仕入先を作成する
description: Dynamics 365 Business Central にベンダーオブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 90c2c8a25602ac2a2c4197c916b9ce14e03b8e6d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365354"
---
# <a name="create-vendors"></a><span data-ttu-id="a10fd-103">仕入先を作成する</span><span class="sxs-lookup"><span data-stu-id="a10fd-103">Create vendors</span></span>
<span data-ttu-id="a10fd-104">Dynamics 365 Business Central でベンダーオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a10fd-104">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a10fd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a10fd-105">Permissions</span></span>
<span data-ttu-id="a10fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a10fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a10fd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a10fd-108">Permission type</span></span> |<span data-ttu-id="a10fd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a10fd-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a10fd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a10fd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a10fd-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10fd-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a10fd-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="a10fd-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a10fd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a10fd-113">Not supported.</span></span>|
|<span data-ttu-id="a10fd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a10fd-114">Application</span></span>|<span data-ttu-id="a10fd-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a10fd-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a10fd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a10fd-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a10fd-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a10fd-117">Optional query parameters</span></span>
<span data-ttu-id="a10fd-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a10fd-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a10fd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a10fd-119">Request headers</span></span>
|<span data-ttu-id="a10fd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a10fd-120">Header</span></span>|<span data-ttu-id="a10fd-121">値</span><span class="sxs-lookup"><span data-stu-id="a10fd-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="a10fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a10fd-122">Authorization</span></span>  |<span data-ttu-id="a10fd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a10fd-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a10fd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a10fd-125">Content-Type</span></span>  |<span data-ttu-id="a10fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a10fd-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="a10fd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a10fd-127">Request body</span></span>
<span data-ttu-id="a10fd-128">要求本文で、**ベンダー**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a10fd-128">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="a10fd-129">応答</span><span class="sxs-lookup"><span data-stu-id="a10fd-129">Response</span></span>
<span data-ttu-id="a10fd-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**ベンダー**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a10fd-130">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a10fd-131">例</span><span class="sxs-lookup"><span data-stu-id="a10fd-131">Example</span></span>

<span data-ttu-id="a10fd-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="a10fd-132">**Request**</span></span>

<span data-ttu-id="a10fd-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a10fd-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/vendors
Content-type: application/json

{
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="a10fd-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="a10fd-134">**Response**</span></span>

<span data-ttu-id="a10fd-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a10fd-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="a10fd-136">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="a10fd-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a10fd-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a10fd-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}

```

