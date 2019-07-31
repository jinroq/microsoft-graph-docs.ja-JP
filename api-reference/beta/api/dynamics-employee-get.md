---
title: 従業員の取得
description: Dynamics 365 Business Central の employee オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 565c4f1222b143ed9635a68bf29d88e544e4c8e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956304"
---
# <a name="get-employees"></a><span data-ttu-id="fa9f9-103">従業員の取得</span><span class="sxs-lookup"><span data-stu-id="fa9f9-103">Get employees</span></span>
<span data-ttu-id="fa9f9-104">Dynamics 365 Business Central の employee オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-104">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa9f9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa9f9-105">Permissions</span></span>
<span data-ttu-id="fa9f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa9f9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa9f9-108">Permission type</span></span> |<span data-ttu-id="fa9f9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa9f9-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="fa9f9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa9f9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="fa9f9-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa9f9-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="fa9f9-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="fa9f9-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fa9f9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-113">Not supported.</span></span>|
|<span data-ttu-id="fa9f9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa9f9-114">Application</span></span>|<span data-ttu-id="fa9f9-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa9f9-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa9f9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa9f9-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/employees('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa9f9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa9f9-117">Optional query parameters</span></span>
<span data-ttu-id="fa9f9-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa9f9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa9f9-119">Request headers</span></span>
|<span data-ttu-id="fa9f9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa9f9-120">Header</span></span>       |<span data-ttu-id="fa9f9-121">値</span><span class="sxs-lookup"><span data-stu-id="fa9f9-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="fa9f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa9f9-122">Authorization</span></span>|<span data-ttu-id="fa9f9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa9f9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa9f9-125">Request body</span></span>
<span data-ttu-id="fa9f9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa9f9-127">応答</span><span class="sxs-lookup"><span data-stu-id="fa9f9-127">Response</span></span>
<span data-ttu-id="fa9f9-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**employees**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-128">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="fa9f9-129">**要求**</span><span class="sxs-lookup"><span data-stu-id="fa9f9-129">**Request**</span></span>

<span data-ttu-id="fa9f9-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/employees('{id}')
```

<span data-ttu-id="fa9f9-131">**応答**</span><span class="sxs-lookup"><span data-stu-id="fa9f9-131">**Response**</span></span>

<span data-ttu-id="fa9f9-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="fa9f9-133">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa9f9-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fa9f9-134">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "AH",
  "displayName": "Annette Hill",
  "givenName": "Annette",
  "middleName": "",
  "surname": "Hill",
  "jobTitle": "Secretary",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "email": "",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "terminationDate": "0001-01-01",
  "status": "Active",
  "birthDate": "1973-12-12",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/employees('{id}')/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"  
}
```


