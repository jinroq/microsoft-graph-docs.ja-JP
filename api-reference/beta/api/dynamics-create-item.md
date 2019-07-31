---
title: アイテムを作成する
description: Dynamics 365 Business Central にアイテムオブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: db6622a6f58bb4fb84a19b56b62f20d305fc74f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956668"
---
# <a name="create-items"></a><span data-ttu-id="43931-103">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="43931-103">Create items</span></span>
<span data-ttu-id="43931-104">「Dynamics 365 Business Central」に、請求書、見積もりなどで使用するアイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="43931-104">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="43931-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="43931-105">Permissions</span></span>
<span data-ttu-id="43931-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43931-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43931-108">Permission type</span></span> |<span data-ttu-id="43931-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="43931-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="43931-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43931-110">Delegated (work or school account)</span></span>|<span data-ttu-id="43931-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43931-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="43931-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="43931-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="43931-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43931-113">Not supported.</span></span>|
|<span data-ttu-id="43931-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43931-114">Application</span></span>|<span data-ttu-id="43931-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43931-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43931-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43931-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43931-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="43931-117">Optional query parameters</span></span>
<span data-ttu-id="43931-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="43931-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43931-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43931-119">Request headers</span></span>
|<span data-ttu-id="43931-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43931-120">Header</span></span>       |<span data-ttu-id="43931-121">値</span><span class="sxs-lookup"><span data-stu-id="43931-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="43931-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43931-122">Authorization</span></span>|<span data-ttu-id="43931-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="43931-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43931-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43931-125">Content-Type</span></span> |<span data-ttu-id="43931-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43931-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="43931-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="43931-127">Request body</span></span>
<span data-ttu-id="43931-128">要求本文で、 **items**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="43931-128">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="43931-129">応答</span><span class="sxs-lookup"><span data-stu-id="43931-129">Response</span></span>
<span data-ttu-id="43931-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**items**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43931-130">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43931-131">例</span><span class="sxs-lookup"><span data-stu-id="43931-131">Example</span></span>
<span data-ttu-id="43931-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="43931-132">**Request**</span></span>

<span data-ttu-id="43931-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43931-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/items
Content-type: application/json

{
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "65bdbd3a-39f1-49f4-bf24-598cbac36230",
  "gtin": "",
  "itemCategoryId": "5b0b9c1c-312d-4809-96b2-056690a11057",
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupCode": "FURNITURE"
} 

```

<span data-ttu-id="43931-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="43931-134">**Response**</span></span>

<span data-ttu-id="43931-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="43931-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="43931-136">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="43931-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="43931-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="43931-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```

