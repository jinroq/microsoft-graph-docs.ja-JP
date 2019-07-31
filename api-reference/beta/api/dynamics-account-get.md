---
title: アカウントを取得する
description: Dynamics 365 Business Central の account オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f0441a3c2f9385378e767d721c09cb28e87a5682
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956878"
---
# <a name="get-accounts"></a><span data-ttu-id="e65ea-103">アカウントを取得する</span><span class="sxs-lookup"><span data-stu-id="e65ea-103">Get accounts</span></span>
<span data-ttu-id="e65ea-104">Dynamics 365 Business Central の account オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e65ea-104">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e65ea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e65ea-105">Permissions</span></span>
<span data-ttu-id="e65ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e65ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e65ea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e65ea-108">Permission type</span></span> |<span data-ttu-id="e65ea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e65ea-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e65ea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e65ea-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e65ea-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e65ea-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e65ea-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="e65ea-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e65ea-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65ea-113">Not supported.</span></span>|
|<span data-ttu-id="e65ea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e65ea-114">Application</span></span>|<span data-ttu-id="e65ea-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e65ea-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="e65ea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e65ea-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/accounts('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e65ea-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e65ea-117">Optional query parameters</span></span>
<span data-ttu-id="e65ea-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e65ea-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e65ea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e65ea-119">Request headers</span></span>
|<span data-ttu-id="e65ea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e65ea-120">Header</span></span>|<span data-ttu-id="e65ea-121">値</span><span class="sxs-lookup"><span data-stu-id="e65ea-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="e65ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e65ea-122">Authorization</span></span>  |<span data-ttu-id="e65ea-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e65ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e65ea-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e65ea-125">Request body</span></span>
<span data-ttu-id="e65ea-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e65ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e65ea-127">応答</span><span class="sxs-lookup"><span data-stu-id="e65ea-127">Response</span></span>
<span data-ttu-id="e65ea-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**accounts**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e65ea-128">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e65ea-129">例</span><span class="sxs-lookup"><span data-stu-id="e65ea-129">Example</span></span>

<span data-ttu-id="e65ea-130">**要求**要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e65ea-130">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/accounts('{id}')
```

<span data-ttu-id="e65ea-131">**応答**</span><span class="sxs-lookup"><span data-stu-id="e65ea-131">**Response**</span></span>

<span data-ttu-id="e65ea-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e65ea-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="e65ea-133">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="e65ea-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e65ea-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e65ea-134">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "id-value",
    "number": "10700",
    "displayName": "Inventory",
    "category": "Assets",
    "subCategory": "Inventory",
    "blocked": false,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```