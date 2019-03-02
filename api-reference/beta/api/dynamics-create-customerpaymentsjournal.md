---
title: customerPaymentJournals を作成する
description: Dynamics 365 Business Central に顧客の支払仕訳帳オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a633ef91fe15b4999285d7290ca6eed8c10846a3
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365466"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="ff140-103">customerPaymentJournals を作成する</span><span class="sxs-lookup"><span data-stu-id="ff140-103">Create customerPaymentJournals</span></span>
<span data-ttu-id="ff140-104">Dynamics 365 Business Central に顧客支払仕訳帳オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ff140-104">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff140-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff140-105">Permissions</span></span>
<span data-ttu-id="ff140-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff140-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff140-108">Permission type</span></span> |<span data-ttu-id="ff140-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff140-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ff140-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff140-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ff140-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff140-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ff140-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="ff140-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ff140-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff140-113">Not supported.</span></span>|
|<span data-ttu-id="ff140-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff140-114">Application</span></span>|<span data-ttu-id="ff140-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff140-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff140-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff140-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff140-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff140-117">Optional query parameters</span></span>
<span data-ttu-id="ff140-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ff140-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff140-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff140-119">Request headers</span></span>
|<span data-ttu-id="ff140-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff140-120">Header</span></span>        |<span data-ttu-id="ff140-121">値</span><span class="sxs-lookup"><span data-stu-id="ff140-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="ff140-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff140-122">Authorization</span></span> |<span data-ttu-id="ff140-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff140-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ff140-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff140-125">Content-Type</span></span>  |<span data-ttu-id="ff140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff140-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="ff140-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff140-127">Request body</span></span>
<span data-ttu-id="ff140-128">要求本文で、 **customerPaymentJournals**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff140-128">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="ff140-129">応答</span><span class="sxs-lookup"><span data-stu-id="ff140-129">Response</span></span>
<span data-ttu-id="ff140-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**customerPaymentJournals**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff140-130">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff140-131">例</span><span class="sxs-lookup"><span data-stu-id="ff140-131">Example</span></span>

<span data-ttu-id="ff140-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="ff140-132">**Request**</span></span>

<span data-ttu-id="ff140-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff140-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="ff140-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="ff140-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


