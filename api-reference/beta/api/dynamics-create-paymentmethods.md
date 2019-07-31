---
title: PaymentMethods を作成する
description: Dynamics 365 Business Central に支払い方法オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 682b59383c9e6c791f57162871ed4ecbb8ab8c93
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956612"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="caf57-103">PaymentMethods を作成する</span><span class="sxs-lookup"><span data-stu-id="caf57-103">Create paymentMethods</span></span>
<span data-ttu-id="caf57-104">DDynamics 365 Business Central で支払い方法オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="caf57-104">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="caf57-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="caf57-105">Permissions</span></span>
<span data-ttu-id="caf57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="caf57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caf57-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="caf57-108">Permission type</span></span> |<span data-ttu-id="caf57-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="caf57-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="caf57-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="caf57-110">Delegated (work or school account)</span></span>|<span data-ttu-id="caf57-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf57-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="caf57-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="caf57-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="caf57-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caf57-113">Not supported.</span></span>|
|<span data-ttu-id="caf57-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="caf57-114">Application</span></span>|<span data-ttu-id="caf57-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf57-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="caf57-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="caf57-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="caf57-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="caf57-117">Optional query parameters</span></span>
<span data-ttu-id="caf57-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="caf57-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="caf57-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caf57-119">Request headers</span></span>
|<span data-ttu-id="caf57-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caf57-120">Header</span></span>         |<span data-ttu-id="caf57-121">値</span><span class="sxs-lookup"><span data-stu-id="caf57-121">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="caf57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="caf57-122">Authorization</span></span>  |<span data-ttu-id="caf57-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="caf57-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="caf57-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="caf57-125">Content-Type</span></span>   |<span data-ttu-id="caf57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="caf57-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="caf57-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="caf57-127">Request body</span></span>
<span data-ttu-id="caf57-128">要求本文で、 **paymentMethods**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="caf57-128">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="caf57-129">応答</span><span class="sxs-lookup"><span data-stu-id="caf57-129">Response</span></span>
<span data-ttu-id="caf57-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**paymentMethods**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="caf57-130">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caf57-131">例</span><span class="sxs-lookup"><span data-stu-id="caf57-131">Example</span></span>

<span data-ttu-id="caf57-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="caf57-132">**Request**</span></span>

<span data-ttu-id="caf57-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="caf57-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="caf57-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="caf57-134">**Response**</span></span>

<span data-ttu-id="caf57-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="caf57-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="caf57-136">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="caf57-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="caf57-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="caf57-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```

