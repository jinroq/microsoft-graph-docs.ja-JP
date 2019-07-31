---
title: 従業員を作成する
description: Dynamics 365 Business Central に employee オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ddfef594c622030b5f0d87a99e7cadeccf8b935c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956682"
---
# <a name="create-employees"></a><span data-ttu-id="4a725-103">従業員を作成する</span><span class="sxs-lookup"><span data-stu-id="4a725-103">Create employees</span></span>
<span data-ttu-id="4a725-104">Dynamics 365 Business Central で employee オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4a725-104">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a725-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a725-105">Permissions</span></span>
<span data-ttu-id="4a725-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a725-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a725-108">Permission type</span></span> |<span data-ttu-id="4a725-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a725-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4a725-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a725-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4a725-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a725-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4a725-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="4a725-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4a725-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a725-113">Not supported.</span></span>|
|<span data-ttu-id="4a725-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a725-114">Application</span></span>|<span data-ttu-id="4a725-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a725-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a725-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a725-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a725-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a725-117">Optional query parameters</span></span>
<span data-ttu-id="4a725-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4a725-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a725-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a725-119">Request headers</span></span>
|<span data-ttu-id="4a725-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a725-120">Header</span></span>        |<span data-ttu-id="4a725-121">値</span><span class="sxs-lookup"><span data-stu-id="4a725-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="4a725-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a725-122">Authorization</span></span> |<span data-ttu-id="4a725-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a725-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4a725-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a725-125">Content-Type</span></span>  |<span data-ttu-id="4a725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a725-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="4a725-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a725-127">Request body</span></span>
<span data-ttu-id="4a725-128">要求本文で、 **employees**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a725-128">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="4a725-129">応答</span><span class="sxs-lookup"><span data-stu-id="4a725-129">Response</span></span>
<span data-ttu-id="4a725-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**employees**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4a725-130">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a725-131">例</span><span class="sxs-lookup"><span data-stu-id="4a725-131">Example</span></span>

<span data-ttu-id="4a725-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="4a725-132">**Request**</span></span>

<span data-ttu-id="4a725-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a725-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/employees
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "givenName": "Annette",
  "surname": "Hill",
  "jobTitle": "Production Assistant",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "birthDate": "1973-12-12"  
}

```

<span data-ttu-id="4a725-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="4a725-134">**Response**</span></span>

<span data-ttu-id="4a725-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4a725-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="4a725-136">**注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="4a725-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a725-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a725-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

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

