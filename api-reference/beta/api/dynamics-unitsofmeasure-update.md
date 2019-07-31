---
title: UnitsOfMeasure の更新
description: Dynamics 365 Business Central の測定単位オブジェクトを更新します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 1d18b2093c5b00a6e08ad4a8c8e91161c2d5216e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955842"
---
# <a name="update-unitsofmeasure"></a><span data-ttu-id="412f9-103">UnitsOfMeasure の更新</span><span class="sxs-lookup"><span data-stu-id="412f9-103">Update unitsOfMeasure</span></span>
<span data-ttu-id="412f9-104">Dynamics 365 Business Central の測定単位オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="412f9-104">Update the properties of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="412f9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="412f9-105">Permissions</span></span>
<span data-ttu-id="412f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="412f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="412f9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="412f9-108">Permission type</span></span> |<span data-ttu-id="412f9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="412f9-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="412f9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="412f9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="412f9-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="412f9-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="412f9-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="412f9-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="412f9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="412f9-113">Not supported.</span></span>|
|<span data-ttu-id="412f9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="412f9-114">Application</span></span>|<span data-ttu-id="412f9-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="412f9-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="412f9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="412f9-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/unitsOfMeasure('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="412f9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="412f9-117">Optional query parameters</span></span>
<span data-ttu-id="412f9-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="412f9-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="412f9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="412f9-119">Request headers</span></span>
|<span data-ttu-id="412f9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="412f9-120">Header</span></span>|<span data-ttu-id="412f9-121">値</span><span class="sxs-lookup"><span data-stu-id="412f9-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="412f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="412f9-122">Authorization</span></span> |<span data-ttu-id="412f9-123">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="412f9-123">Bearer.</span></span> <span data-ttu-id="412f9-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="412f9-124">Required.</span></span>|
|<span data-ttu-id="412f9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="412f9-125">Content-Type</span></span>  |<span data-ttu-id="412f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="412f9-126">application/json</span></span>|
|<span data-ttu-id="412f9-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="412f9-127">If-Match</span></span>      |<span data-ttu-id="412f9-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="412f9-128">Required.</span></span> <span data-ttu-id="412f9-129">この要求ヘッダーが含まれていて、指定された eTag が**unitsOfMeasure**の現在のタグと一致しない場合、 **unitsOfMeasure**は更新されません。</span><span class="sxs-lookup"><span data-stu-id="412f9-129">When this request header is included and the eTag provided does not match the current tag on the **unitsOfMeasure**, the **unitsOfMeasure** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="412f9-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="412f9-130">Request body</span></span>
<span data-ttu-id="412f9-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="412f9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="412f9-134">応答</span><span class="sxs-lookup"><span data-stu-id="412f9-134">Response</span></span>
<span data-ttu-id="412f9-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された**unitsOfMeasure**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="412f9-135">If successful, this method returns a `200 OK` response code and an updated **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="412f9-136">例</span><span class="sxs-lookup"><span data-stu-id="412f9-136">Example</span></span>

<span data-ttu-id="412f9-137">**要求**</span><span class="sxs-lookup"><span data-stu-id="412f9-137">**Request**</span></span>

<span data-ttu-id="412f9-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="412f9-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/unitsOfMeasure('{id}')
Content-type: application/json

{
  "displayName": "One Piece"
}
```

<span data-ttu-id="412f9-139">**応答**</span><span class="sxs-lookup"><span data-stu-id="412f9-139">**Response**</span></span>

<span data-ttu-id="412f9-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="412f9-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="412f9-141">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="412f9-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="412f9-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="412f9-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "One Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```

