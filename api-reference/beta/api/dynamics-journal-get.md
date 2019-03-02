---
title: ジャーナルを取得する
description: Dynamics 365 Business Central のジャーナルオブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 79811e0287a7a5c285ec0cb33c754dda06644a2b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365851"
---
# <a name="get-journals"></a><span data-ttu-id="fcef5-103">ジャーナルを取得する</span><span class="sxs-lookup"><span data-stu-id="fcef5-103">Get journals</span></span>
<span data-ttu-id="fcef5-104">Dynamics 365 Business Central の journal オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="fcef5-104">Retrieve the properties and relationships of a journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcef5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fcef5-105">Permissions</span></span>
<span data-ttu-id="fcef5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcef5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fcef5-108">Permission type</span></span> |<span data-ttu-id="fcef5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fcef5-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="fcef5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fcef5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="fcef5-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcef5-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="fcef5-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="fcef5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fcef5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcef5-113">Not supported.</span></span>|
|<span data-ttu-id="fcef5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fcef5-114">Application</span></span>|<span data-ttu-id="fcef5-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcef5-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcef5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fcef5-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/journals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcef5-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fcef5-117">Optional query parameters</span></span>
<span data-ttu-id="fcef5-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fcef5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcef5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fcef5-119">Request headers</span></span>
|<span data-ttu-id="fcef5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fcef5-120">Header</span></span>|<span data-ttu-id="fcef5-121">値</span><span class="sxs-lookup"><span data-stu-id="fcef5-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="fcef5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcef5-122">Authorization</span></span>  |<span data-ttu-id="fcef5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fcef5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcef5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fcef5-125">Request body</span></span>
<span data-ttu-id="fcef5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fcef5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcef5-127">応答</span><span class="sxs-lookup"><span data-stu-id="fcef5-127">Response</span></span>
<span data-ttu-id="fcef5-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**ジャーナル**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fcef5-128">If successful, this method returns a `200 OK` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcef5-129">例</span><span class="sxs-lookup"><span data-stu-id="fcef5-129">Example</span></span>

<span data-ttu-id="fcef5-130">**要求**</span><span class="sxs-lookup"><span data-stu-id="fcef5-130">**Request**</span></span>

<span data-ttu-id="fcef5-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fcef5-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')
```

<span data-ttu-id="fcef5-132">**応答**</span><span class="sxs-lookup"><span data-stu-id="fcef5-132">**Response**</span></span>

<span data-ttu-id="fcef5-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fcef5-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="fcef5-134">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="fcef5-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fcef5-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fcef5-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

