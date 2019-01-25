---
title: リスト bookingCurrencies
description: Microsoft 予約業務に利用可能な bookingCurrency のオブジェクトの一覧を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c29ad5780deac5e5e338052c72661f834e483054
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513222"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="04e80-103">リスト bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="04e80-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04e80-104">Microsoft 予約業務に利用可能な[bookingCurrency](../resources/bookingcurrency.md)のオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="04e80-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="04e80-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04e80-105">Permissions</span></span>
<span data-ttu-id="04e80-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04e80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e80-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04e80-108">Permission type</span></span>      | <span data-ttu-id="04e80-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04e80-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04e80-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04e80-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04e80-111">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="04e80-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="04e80-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04e80-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04e80-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e80-113">Not supported.</span></span>   |
|<span data-ttu-id="04e80-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04e80-114">Application</span></span> | <span data-ttu-id="04e80-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e80-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="04e80-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04e80-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04e80-117">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="04e80-117">Optional query parameters</span></span>
<span data-ttu-id="04e80-118">このメソッドは、$count、$filter、$select、$skip、$top など、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="04e80-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04e80-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04e80-119">Request headers</span></span>
| <span data-ttu-id="04e80-120">名前</span><span class="sxs-lookup"><span data-stu-id="04e80-120">Name</span></span>      |<span data-ttu-id="04e80-121">説明</span><span class="sxs-lookup"><span data-stu-id="04e80-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="04e80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e80-122">Authorization</span></span>  | <span data-ttu-id="04e80-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="04e80-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e80-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="04e80-124">Request body</span></span>
<span data-ttu-id="04e80-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04e80-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="04e80-126">応答</span><span class="sxs-lookup"><span data-stu-id="04e80-126">Response</span></span>
<span data-ttu-id="04e80-127">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingCurrency](../resources/bookingcurrency.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="04e80-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04e80-128">例</span><span class="sxs-lookup"><span data-stu-id="04e80-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04e80-129">要求</span><span class="sxs-lookup"><span data-stu-id="04e80-129">Request</span></span>
<span data-ttu-id="04e80-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="04e80-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="04e80-131">応答</span><span class="sxs-lookup"><span data-stu-id="04e80-131">Response</span></span>
<span data-ttu-id="04e80-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="04e80-132">The following is an example of the response.</span></span> <span data-ttu-id="04e80-133">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="04e80-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="04e80-134">すべてのサポートされている通貨とプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04e80-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
