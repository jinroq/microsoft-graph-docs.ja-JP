---
title: AgedAccountsReceivable を取得する
description: Dynamics 365 Business Central の期限切れの売掛金勘定オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.author: solsen
ms.openlocfilehash: 7270e50881b9e6358052fef4ae879bbb3dcfc5fe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712821"
---
# <a name="get-agedaccountsreceivable"></a><span data-ttu-id="be30e-103">AgedAccountsReceivable を取得する</span><span class="sxs-lookup"><span data-stu-id="be30e-103">Get agedAccountsReceivable</span></span>
<span data-ttu-id="be30e-104">Dynamics 365 Business Central の、古くなった売掛金勘定レポートオブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="be30e-104">Retrieve the properties and relationships of an aged accounts receivable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="be30e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be30e-105">Permissions</span></span>
<span data-ttu-id="be30e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be30e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be30e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be30e-108">Permission type</span></span> |<span data-ttu-id="be30e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be30e-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="be30e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be30e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="be30e-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be30e-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="be30e-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="be30e-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="be30e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be30e-113">Not supported.</span></span>|
|<span data-ttu-id="be30e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be30e-114">Application</span></span>|<span data-ttu-id="be30e-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be30e-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be30e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be30e-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be30e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="be30e-117">Optional query parameters</span></span>
<span data-ttu-id="be30e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="be30e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be30e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be30e-119">Request headers</span></span>
|<span data-ttu-id="be30e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be30e-120">Header</span></span>|<span data-ttu-id="be30e-121">値</span><span class="sxs-lookup"><span data-stu-id="be30e-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="be30e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be30e-122">Authorization</span></span>  |<span data-ttu-id="be30e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be30e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be30e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="be30e-125">Request body</span></span>
<span data-ttu-id="be30e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="be30e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be30e-127">応答</span><span class="sxs-lookup"><span data-stu-id="be30e-127">Response</span></span>
<span data-ttu-id="be30e-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**agedAccountsReceivable**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be30e-128">If successful, this method returns a `200 OK` response code and an **agedAccountsReceivable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be30e-129">例</span><span class="sxs-lookup"><span data-stu-id="be30e-129">Example</span></span>

<span data-ttu-id="be30e-130">**要求**</span><span class="sxs-lookup"><span data-stu-id="be30e-130">**Request**</span></span>

<span data-ttu-id="be30e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be30e-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="be30e-132">**応答**</span><span class="sxs-lookup"><span data-stu-id="be30e-132">**Response**</span></span>

<span data-ttu-id="be30e-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="be30e-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="be30e-134">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="be30e-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be30e-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="be30e-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "customerId": "id-value",
  "customerNumber": "30000",
  "name": "Relecloud",
  "currencyCode": "USD",
  "balanceDue": 349615.45,
  "currentAmount": 0,
  "period1Amount": 349615.45,
  "period2Amount": 0,
  "period3Amount": 0,
  "agedAsOfDate": "2017-04-25",
  "periodLengthFilter": "3M"   
}
```
