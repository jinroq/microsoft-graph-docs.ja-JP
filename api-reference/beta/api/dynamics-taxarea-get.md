---
title: taxAreas を取得する
description: Dynamics 365 Business Central の tax area オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b4d5ca27c1248d07ddfa38b4b282282c282e5eef
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366600"
---
# <a name="get-taxareas"></a><span data-ttu-id="0fe63-103">taxAreas を取得する</span><span class="sxs-lookup"><span data-stu-id="0fe63-103">Get taxAreas</span></span>
<span data-ttu-id="0fe63-104">Dynamics 365 Business Central の税エリアオブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="0fe63-104">Retrieve the properties and relationships of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe63-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0fe63-105">Permissions</span></span>
<span data-ttu-id="0fe63-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fe63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe63-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fe63-108">Permission type</span></span> |<span data-ttu-id="0fe63-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fe63-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0fe63-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fe63-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0fe63-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe63-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0fe63-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="0fe63-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0fe63-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fe63-113">Not supported.</span></span>|
|<span data-ttu-id="0fe63-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fe63-114">Application</span></span>|<span data-ttu-id="0fe63-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe63-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fe63-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fe63-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fe63-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fe63-117">Optional query parameters</span></span>
<span data-ttu-id="0fe63-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0fe63-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fe63-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fe63-119">Request headers</span></span>
|<span data-ttu-id="0fe63-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fe63-120">Header</span></span>|<span data-ttu-id="0fe63-121">値</span><span class="sxs-lookup"><span data-stu-id="0fe63-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="0fe63-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fe63-122">Authorization</span></span>  |<span data-ttu-id="0fe63-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fe63-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fe63-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fe63-125">Request body</span></span>
<span data-ttu-id="0fe63-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0fe63-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe63-127">応答</span><span class="sxs-lookup"><span data-stu-id="0fe63-127">Response</span></span>
<span data-ttu-id="0fe63-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**taxAreas**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0fe63-128">If successful, this method returns a `200 OK` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe63-129">例</span><span class="sxs-lookup"><span data-stu-id="0fe63-129">Example</span></span>

<span data-ttu-id="0fe63-130">**要求**</span><span class="sxs-lookup"><span data-stu-id="0fe63-130">**Request**</span></span>

<span data-ttu-id="0fe63-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0fe63-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas('{id}')
```

<span data-ttu-id="0fe63-132">**応答**</span><span class="sxs-lookup"><span data-stu-id="0fe63-132">**Response**</span></span>

<span data-ttu-id="0fe63-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0fe63-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="0fe63-134">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="0fe63-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0fe63-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0fe63-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

