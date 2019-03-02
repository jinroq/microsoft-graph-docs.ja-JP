---
title: 顧客の支払いを作成する
description: Dynamics 365 Business Central に顧客の支払いオブジェクトを作成します。
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 99bdd4a227be12269eb4ac3937937686089f325c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365697"
---
# <a name="create-customerpayments"></a><span data-ttu-id="eefcd-103">顧客の支払いを作成する</span><span class="sxs-lookup"><span data-stu-id="eefcd-103">Create customerPayments</span></span>
<span data-ttu-id="eefcd-104">Dynamics 365 Business Central に顧客の支払いオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eefcd-104">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="eefcd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eefcd-105">Permissions</span></span>
<span data-ttu-id="eefcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eefcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eefcd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eefcd-108">Permission type</span></span> |<span data-ttu-id="eefcd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eefcd-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="eefcd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eefcd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="eefcd-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eefcd-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="eefcd-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="eefcd-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eefcd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eefcd-113">Not supported.</span></span>|
|<span data-ttu-id="eefcd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eefcd-114">Application</span></span>|<span data-ttu-id="eefcd-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eefcd-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eefcd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eefcd-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eefcd-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eefcd-117">Optional query parameters</span></span>
<span data-ttu-id="eefcd-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eefcd-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eefcd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eefcd-119">Request headers</span></span>
|<span data-ttu-id="eefcd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eefcd-120">Header</span></span>        |<span data-ttu-id="eefcd-121">値</span><span class="sxs-lookup"><span data-stu-id="eefcd-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="eefcd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eefcd-122">Authorization</span></span> |<span data-ttu-id="eefcd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eefcd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eefcd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eefcd-125">Content-Type</span></span>  |<span data-ttu-id="eefcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eefcd-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="eefcd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="eefcd-127">Request body</span></span>
<span data-ttu-id="eefcd-128">要求本文で、**顧客の支払い**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eefcd-128">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="eefcd-129">応答</span><span class="sxs-lookup"><span data-stu-id="eefcd-129">Response</span></span>
<span data-ttu-id="eefcd-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で、**顧客の支払い**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eefcd-130">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eefcd-131">例</span><span class="sxs-lookup"><span data-stu-id="eefcd-131">Example</span></span>

<span data-ttu-id="eefcd-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="eefcd-132">**Request**</span></span>

<span data-ttu-id="eefcd-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eefcd-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournal('{id}')/customerPayments
Content-type: application/json

{
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": -1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
}
```
<span data-ttu-id="eefcd-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="eefcd-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

