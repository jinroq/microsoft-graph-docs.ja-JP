---
title: 一般に備えた gerentries エントリを取得する
description: Dynamics 365 Business Central の総勘定元帳エントリオブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 06884308987eb8010be965d30d09e064e3d67d5e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458510"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="9530b-103">一般に備えた gerentries エントリを取得する</span><span class="sxs-lookup"><span data-stu-id="9530b-103">Get generalLedgerEntries</span></span>
<span data-ttu-id="9530b-104">Dynamics 365 Business Central の総勘定元帳エントリオブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="9530b-104">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9530b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9530b-105">Permissions</span></span>
<span data-ttu-id="9530b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9530b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9530b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9530b-108">Permission type</span></span> |<span data-ttu-id="9530b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9530b-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9530b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9530b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9530b-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530b-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9530b-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="9530b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9530b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9530b-113">Not supported.</span></span>|
|<span data-ttu-id="9530b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9530b-114">Application</span></span>|<span data-ttu-id="9530b-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530b-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="9530b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9530b-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/generalLedgerEntries('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9530b-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9530b-117">Optional query parameters</span></span>
<span data-ttu-id="9530b-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9530b-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9530b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9530b-119">Request headers</span></span>
|<span data-ttu-id="9530b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9530b-120">Header</span></span>       |<span data-ttu-id="9530b-121">値</span><span class="sxs-lookup"><span data-stu-id="9530b-121">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="9530b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9530b-122">Authorization</span></span>|<span data-ttu-id="9530b-123">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="9530b-123">Bearer.</span></span> <span data-ttu-id="9530b-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="9530b-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9530b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9530b-125">Request body</span></span>
<span data-ttu-id="9530b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9530b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9530b-127">応答</span><span class="sxs-lookup"><span data-stu-id="9530b-127">Response</span></span>
<span data-ttu-id="9530b-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で一般に指定された**gergerentries**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9530b-128">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9530b-129">例</span><span class="sxs-lookup"><span data-stu-id="9530b-129">Example</span></span>

<span data-ttu-id="9530b-130">**要求**</span><span class="sxs-lookup"><span data-stu-id="9530b-130">**Request**</span></span>

<span data-ttu-id="9530b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9530b-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/generalLedgerEntries('{id}')
```

<span data-ttu-id="9530b-132">**応答**</span><span class="sxs-lookup"><span data-stu-id="9530b-132">**Response**</span></span>

<span data-ttu-id="9530b-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9530b-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="9530b-134">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9530b-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9530b-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9530b-135">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "10700",
    "postingDate": "2017-03-15",
    "documentNumber": "108027",
    "documentType": "Invoice",
    "accountId": "id-value",
    "accountNumber": "7210",
    "description": "Order 106003",
    "debitAmount": 6943.8,
    "creditAmount": 0,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```

