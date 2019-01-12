---
title: リスト bookingBusinesses
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 51b8e049b45542de9940168c994bed8fbd273b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951454"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="23f2e-104">リスト bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="23f2e-104">List bookingBusinesses</span></span>

 > <span data-ttu-id="23f2e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23f2e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23f2e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23f2e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="23f2e-107">テナントの作成された[bookingbusiness](../resources/bookingbusiness.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="23f2e-107">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span> 

<span data-ttu-id="23f2e-108">この操作には、コレクション内の**id**と予約の各企業の**表示名**だけが返されます。</span><span class="sxs-lookup"><span data-stu-id="23f2e-108">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="23f2e-109">パフォーマンスに関する考慮事項、その他のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="23f2e-109">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="23f2e-110">[GET](bookingbusiness-get.md)操作でその**id**を指定することによって、予約のビジネスの他のプロパティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="23f2e-110">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="23f2e-111">照会することも予約企業内の文字列を指定することにより、`query`は、テナントの企業間で一致するサブスト リングのパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="23f2e-111">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="23f2e-112">次[の使用例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23f2e-112">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="23f2e-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="23f2e-113">Permissions</span></span>
<span data-ttu-id="23f2e-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23f2e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23f2e-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23f2e-116">Permission type</span></span>      | <span data-ttu-id="23f2e-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="23f2e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f2e-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23f2e-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="23f2e-119">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="23f2e-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="23f2e-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23f2e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f2e-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23f2e-121">Not supported.</span></span>   |
|<span data-ttu-id="23f2e-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23f2e-122">Application</span></span> | <span data-ttu-id="23f2e-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23f2e-123">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="23f2e-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23f2e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23f2e-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="23f2e-125">Optional query parameters</span></span>
<span data-ttu-id="23f2e-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="23f2e-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="23f2e-127">このメソッドもサポートしています、`query`パラメーターの文字列値を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="23f2e-127">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="23f2e-128">このパラメーターは、指定した文字列に一致する複数の企業に取得結果を制限します。</span><span class="sxs-lookup"><span data-stu-id="23f2e-128">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="23f2e-129">次[の使用例](#request-2)を表示できます。</span><span class="sxs-lookup"><span data-stu-id="23f2e-129">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="23f2e-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23f2e-130">Request headers</span></span>
| <span data-ttu-id="23f2e-131">名前</span><span class="sxs-lookup"><span data-stu-id="23f2e-131">Name</span></span>      |<span data-ttu-id="23f2e-132">説明</span><span class="sxs-lookup"><span data-stu-id="23f2e-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23f2e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="23f2e-133">Authorization</span></span>  | <span data-ttu-id="23f2e-134">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="23f2e-134">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="23f2e-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="23f2e-135">Request body</span></span>
<span data-ttu-id="23f2e-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="23f2e-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="23f2e-137">応答</span><span class="sxs-lookup"><span data-stu-id="23f2e-137">Response</span></span>
<span data-ttu-id="23f2e-138">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingBusiness](../resources/bookingbusiness.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="23f2e-138">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23f2e-139">例</span><span class="sxs-lookup"><span data-stu-id="23f2e-139">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="23f2e-140">要求 1</span><span class="sxs-lookup"><span data-stu-id="23f2e-140">Request 1</span></span>
<span data-ttu-id="23f2e-141">テナントの記帳業務を取得する例を次にします。</span><span class="sxs-lookup"><span data-stu-id="23f2e-141">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="23f2e-142">応答 1</span><span class="sxs-lookup"><span data-stu-id="23f2e-142">Response 1</span></span>
<span data-ttu-id="23f2e-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23f2e-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="23f2e-144">要求 2</span><span class="sxs-lookup"><span data-stu-id="23f2e-144">Request 2</span></span>
<span data-ttu-id="23f2e-145">使用する方法の例を次の`query`、テナントの 1 つまたは複数の一致する受注企業を取得するパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="23f2e-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="23f2e-146">応答 2</span><span class="sxs-lookup"><span data-stu-id="23f2e-146">Response 2</span></span>
<span data-ttu-id="23f2e-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23f2e-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
