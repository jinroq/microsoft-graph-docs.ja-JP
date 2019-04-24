---
title: 会社情報の取得
description: Dynamics 365 Business Central の会社情報オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ad49c3d4095283fc42c2e8f2046c646f3558ac18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454189"
---
# <a name="get-companyinformation"></a><span data-ttu-id="ffbff-103">会社情報の取得</span><span class="sxs-lookup"><span data-stu-id="ffbff-103">Get companyInformation</span></span>
<span data-ttu-id="ffbff-104">Dynamics 365 Business Central の会社情報オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ffbff-104">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffbff-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ffbff-105">Permissions</span></span>
<span data-ttu-id="ffbff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffbff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffbff-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffbff-108">Permission type</span></span> |<span data-ttu-id="ffbff-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffbff-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ffbff-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffbff-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ffbff-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffbff-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ffbff-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="ffbff-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ffbff-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffbff-113">Not supported.</span></span>|
|<span data-ttu-id="ffbff-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffbff-114">Application</span></span>|<span data-ttu-id="ffbff-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffbff-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffbff-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffbff-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/companyInformation('{id}')
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffbff-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ffbff-117">Optional query parameters</span></span>
<span data-ttu-id="ffbff-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ffbff-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffbff-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffbff-119">Request headers</span></span>
|<span data-ttu-id="ffbff-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffbff-120">Header</span></span>|<span data-ttu-id="ffbff-121">値</span><span class="sxs-lookup"><span data-stu-id="ffbff-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="ffbff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffbff-122">Authorization</span></span>  |<span data-ttu-id="ffbff-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ffbff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffbff-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffbff-125">Request body</span></span>
<span data-ttu-id="ffbff-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ffbff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffbff-127">応答</span><span class="sxs-lookup"><span data-stu-id="ffbff-127">Response</span></span>
<span data-ttu-id="ffbff-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で会社**情報**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffbff-128">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffbff-129">例</span><span class="sxs-lookup"><span data-stu-id="ffbff-129">Example</span></span>

<span data-ttu-id="ffbff-130">**要求**</span><span class="sxs-lookup"><span data-stu-id="ffbff-130">**Request**</span></span>

<span data-ttu-id="ffbff-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffbff-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/companyInformation('{id}')
```

<span data-ttu-id="ffbff-132">**応答**</span><span class="sxs-lookup"><span data-stu-id="ffbff-132">**Response**</span></span>

<span data-ttu-id="ffbff-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ffbff-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="ffbff-134">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="ffbff-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ffbff-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ffbff-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "displayName": "CRONUS USA, Inc.",
  "address": {
    "street": "7122 South Ashford Street\r\nWestminster",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "+1 425 555 0100",
  "faxNumber": "+1 425 555 0101",
  "email": "",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/companyInformation('{id}')/picture",
  "businessProfileId": "",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
}
```
