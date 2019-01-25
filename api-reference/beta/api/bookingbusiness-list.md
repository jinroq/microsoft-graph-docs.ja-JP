---
title: リスト bookingBusinesses
description: テナントの作成された bookingbusiness オブジェクトのコレクションを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8018b8ac7f9d2e5f74e4233dbc36c2a6faa2d9a8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523156"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d5920-103">リスト bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="d5920-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5920-104">テナントの作成された[bookingbusiness](../resources/bookingbusiness.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d5920-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="d5920-105">この操作には、コレクション内の**id**と予約の各企業の**表示名**だけが返されます。</span><span class="sxs-lookup"><span data-stu-id="d5920-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d5920-106">パフォーマンスに関する考慮事項、その他のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="d5920-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d5920-107">[GET](bookingbusiness-get.md)操作でその**id**を指定することによって、予約のビジネスの他のプロパティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d5920-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d5920-108">照会することも予約企業内の文字列を指定することにより、`query`は、テナントの企業間で一致するサブスト リングのパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="d5920-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d5920-109">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5920-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d5920-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5920-110">Permissions</span></span>
<span data-ttu-id="d5920-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5920-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5920-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5920-113">Permission type</span></span>      | <span data-ttu-id="d5920-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5920-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5920-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5920-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d5920-116">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d5920-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d5920-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5920-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5920-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5920-118">Not supported.</span></span>   |
|<span data-ttu-id="d5920-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5920-119">Application</span></span> | <span data-ttu-id="d5920-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5920-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d5920-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5920-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5920-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d5920-122">Optional query parameters</span></span>
<span data-ttu-id="d5920-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d5920-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d5920-124">このメソッドもサポートしています、`query`パラメーターの文字列値を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="d5920-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d5920-125">このパラメーターは、指定した文字列に一致する複数の企業に取得結果を制限します。</span><span class="sxs-lookup"><span data-stu-id="d5920-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d5920-126">次[の使用例](#request-2)を表示できます。</span><span class="sxs-lookup"><span data-stu-id="d5920-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d5920-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5920-127">Request headers</span></span>
| <span data-ttu-id="d5920-128">名前</span><span class="sxs-lookup"><span data-stu-id="d5920-128">Name</span></span>      |<span data-ttu-id="d5920-129">説明</span><span class="sxs-lookup"><span data-stu-id="d5920-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5920-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5920-130">Authorization</span></span>  | <span data-ttu-id="d5920-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d5920-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5920-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5920-132">Request body</span></span>
<span data-ttu-id="d5920-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d5920-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d5920-134">応答</span><span class="sxs-lookup"><span data-stu-id="d5920-134">Response</span></span>
<span data-ttu-id="d5920-135">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingBusiness](../resources/bookingbusiness.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d5920-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5920-136">例</span><span class="sxs-lookup"><span data-stu-id="d5920-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d5920-137">要求 1</span><span class="sxs-lookup"><span data-stu-id="d5920-137">Request 1</span></span>
<span data-ttu-id="d5920-138">テナントの記帳業務を取得する例を次にします。</span><span class="sxs-lookup"><span data-stu-id="d5920-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="d5920-139">応答 1</span><span class="sxs-lookup"><span data-stu-id="d5920-139">Response 1</span></span>
<span data-ttu-id="d5920-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5920-140">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="d5920-141">要求 2</span><span class="sxs-lookup"><span data-stu-id="d5920-141">Request 2</span></span>
<span data-ttu-id="d5920-142">使用する方法の例を次の`query`、テナントの 1 つまたは複数の一致する受注企業を取得するパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="d5920-142">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="d5920-143">応答 2</span><span class="sxs-lookup"><span data-stu-id="d5920-143">Response 2</span></span>
<span data-ttu-id="d5920-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5920-144">The following is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
