---
title: paymentTerms の更新
description: Dynamics 365 Business Central の支払い用語オブジェクトを更新します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 04b04461bdf46ec08c1c0230949c3bed89acebd6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458496"
---
# <a name="update-paymentterms"></a><span data-ttu-id="33a2c-103">paymentTerms の更新</span><span class="sxs-lookup"><span data-stu-id="33a2c-103">Update paymentTerms</span></span>
<span data-ttu-id="33a2c-104">Dynamics 365 Business Central の支払い用語オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="33a2c-104">Update the properties of a payment terms object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="33a2c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33a2c-105">Permissions</span></span>
<span data-ttu-id="33a2c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33a2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a2c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33a2c-108">Permission type</span></span> |<span data-ttu-id="33a2c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33a2c-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="33a2c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33a2c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="33a2c-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a2c-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="33a2c-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="33a2c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="33a2c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33a2c-113">Not supported.</span></span>|
|<span data-ttu-id="33a2c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33a2c-114">Application</span></span>|<span data-ttu-id="33a2c-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a2c-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33a2c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33a2c-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/paymentTerms('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33a2c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="33a2c-117">Optional query parameters</span></span>
<span data-ttu-id="33a2c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="33a2c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33a2c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33a2c-119">Request headers</span></span>
|<span data-ttu-id="33a2c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33a2c-120">Header</span></span>        |<span data-ttu-id="33a2c-121">値</span><span class="sxs-lookup"><span data-stu-id="33a2c-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="33a2c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33a2c-122">Authorization</span></span> |<span data-ttu-id="33a2c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33a2c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="33a2c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33a2c-125">Content-Type</span></span>  |<span data-ttu-id="33a2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33a2c-126">application/json</span></span>         |
|<span data-ttu-id="33a2c-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="33a2c-127">If-Match</span></span>      |<span data-ttu-id="33a2c-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="33a2c-128">Required.</span></span> <span data-ttu-id="33a2c-129">この要求ヘッダーが含まれていて、指定された eTag が**paymentTerms**の現在のタグと一致しない場合、 **paymentTerms**は更新されません。</span><span class="sxs-lookup"><span data-stu-id="33a2c-129">When this request header is included and the eTag provided does not match the current tag on the **paymentTerms**, the **paymentTerms** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33a2c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="33a2c-130">Request body</span></span>
<span data-ttu-id="33a2c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="33a2c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="33a2c-134">応答</span><span class="sxs-lookup"><span data-stu-id="33a2c-134">Response</span></span>
<span data-ttu-id="33a2c-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された**paymentTerms**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33a2c-135">If successful, this method returns a `200 OK` response code and an updated **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a2c-136">例</span><span class="sxs-lookup"><span data-stu-id="33a2c-136">Example</span></span>

<span data-ttu-id="33a2c-137">**要求**</span><span class="sxs-lookup"><span data-stu-id="33a2c-137">**Request**</span></span>

<span data-ttu-id="33a2c-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33a2c-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms('{id}')
Content-type: application/json

{
  "displayName": "Net 7 days with Discount",
  "discountPercent": 10
}
```

<span data-ttu-id="33a2c-139">**応答**</span><span class="sxs-lookup"><span data-stu-id="33a2c-139">**Response**</span></span>

<span data-ttu-id="33a2c-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33a2c-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="33a2c-141">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="33a2c-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="33a2c-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="33a2c-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days with Discount",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 10,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-15T02:20:55.203Z"
}
```

