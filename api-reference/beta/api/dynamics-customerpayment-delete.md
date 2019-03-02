---
title: 顧客の支払いを削除する
description: Dynamics 365 Business Central の customer 支払いオブジェクトを削除します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ab4f40785401353887cba22eaeca620c75276051
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365704"
---
# <a name="delete-customerpayments"></a><span data-ttu-id="d64a8-103">顧客の支払いを削除する</span><span class="sxs-lookup"><span data-stu-id="d64a8-103">Delete customerPayments</span></span>
<span data-ttu-id="d64a8-104">Dynamics 365 Business Central から、顧客の支払いを削除します。</span><span class="sxs-lookup"><span data-stu-id="d64a8-104">Delete a customerPayment from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d64a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d64a8-105">Permissions</span></span>
<span data-ttu-id="d64a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d64a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d64a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d64a8-108">Permission type</span></span> |<span data-ttu-id="d64a8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d64a8-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d64a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d64a8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d64a8-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64a8-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d64a8-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="d64a8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d64a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d64a8-113">Not supported.</span></span>|
|<span data-ttu-id="d64a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d64a8-114">Application</span></span>|<span data-ttu-id="d64a8-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64a8-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d64a8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d64a8-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d64a8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d64a8-117">Optional query parameters</span></span>
<span data-ttu-id="d64a8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d64a8-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d64a8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d64a8-119">Request headers</span></span>
|<span data-ttu-id="d64a8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d64a8-120">Header</span></span>         |<span data-ttu-id="d64a8-121">値</span><span class="sxs-lookup"><span data-stu-id="d64a8-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="d64a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d64a8-122">Authorization</span></span>  |<span data-ttu-id="d64a8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d64a8-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d64a8-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="d64a8-125">If-Match</span></span>       |<span data-ttu-id="d64a8-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="d64a8-126">Required.</span></span> <span data-ttu-id="d64a8-127">この要求ヘッダーが含まれていて、指定された eTag が、**顧客の支払い**の現在のタグと一致しない場合、その**顧客の支払い**は更新されません。</span><span class="sxs-lookup"><span data-stu-id="d64a8-127">When this request header is included and the eTag provided does not match the current tag on the **customerPayments**, the **customerPayments** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d64a8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d64a8-128">Request body</span></span>

<span data-ttu-id="d64a8-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d64a8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d64a8-130">応答</span><span class="sxs-lookup"><span data-stu-id="d64a8-130">Response</span></span>

<span data-ttu-id="d64a8-p104">成功した場合、このメソッドは ```204 No Content``` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d64a8-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d64a8-133">例</span><span class="sxs-lookup"><span data-stu-id="d64a8-133">Example</span></span>

<span data-ttu-id="d64a8-134">**要求**</span><span class="sxs-lookup"><span data-stu-id="d64a8-134">**Request**</span></span>

<span data-ttu-id="d64a8-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d64a8-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

<span data-ttu-id="d64a8-136">**応答**</span><span class="sxs-lookup"><span data-stu-id="d64a8-136">**Response**</span></span> 

<span data-ttu-id="d64a8-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d64a8-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
