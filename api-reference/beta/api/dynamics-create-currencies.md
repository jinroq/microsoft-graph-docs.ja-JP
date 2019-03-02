---
title: 通貨の作成
description: Dynamics 365 Business Central に currency オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 53da84723042439505a91dee3838426db6ced820
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365872"
---
# <a name="create-currencies"></a><span data-ttu-id="5ca90-103">通貨の作成</span><span class="sxs-lookup"><span data-stu-id="5ca90-103">Create currencies</span></span>
<span data-ttu-id="5ca90-104">Dynamics 365 Business Central で currency オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ca90-104">Create a currency object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca90-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ca90-105">Permissions</span></span>
<span data-ttu-id="5ca90-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ca90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca90-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ca90-108">Permission type</span></span> |<span data-ttu-id="5ca90-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ca90-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5ca90-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ca90-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5ca90-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca90-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5ca90-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="5ca90-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5ca90-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ca90-113">Not supported.</span></span>|
|<span data-ttu-id="5ca90-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ca90-114">Application</span></span>|<span data-ttu-id="5ca90-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca90-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ca90-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ca90-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/currencies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ca90-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ca90-117">Optional query parameters</span></span>
<span data-ttu-id="5ca90-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5ca90-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ca90-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ca90-119">Request headers</span></span>
|<span data-ttu-id="5ca90-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ca90-120">Header</span></span>         |<span data-ttu-id="5ca90-121">値</span><span class="sxs-lookup"><span data-stu-id="5ca90-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="5ca90-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ca90-122">Authorization</span></span>  |<span data-ttu-id="5ca90-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ca90-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5ca90-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ca90-125">Content-Type</span></span>   |<span data-ttu-id="5ca90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ca90-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="5ca90-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ca90-127">Request body</span></span>
<span data-ttu-id="5ca90-128">要求本文で、**通貨**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ca90-128">In the request body, supply a JSON representation of **currencies** object.</span></span>

## <a name="response"></a><span data-ttu-id="5ca90-129">応答</span><span class="sxs-lookup"><span data-stu-id="5ca90-129">Response</span></span>
<span data-ttu-id="5ca90-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**通貨**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ca90-130">If successful, this method returns ```201 Created``` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca90-131">例</span><span class="sxs-lookup"><span data-stu-id="5ca90-131">Example</span></span>

<span data-ttu-id="5ca90-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="5ca90-132">**Request**</span></span>

<span data-ttu-id="5ca90-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ca90-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/currencies
Content-type: application/json

{
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01
}
```

<span data-ttu-id="5ca90-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="5ca90-134">**Response**</span></span>

<span data-ttu-id="5ca90-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5ca90-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="5ca90-136">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5ca90-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5ca90-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ca90-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.002Z"
}

```
