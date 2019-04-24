---
title: bookingcustomer を取得する
description: bookingcustomer オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 34497c35dd4bd0e46764b8c025c93570b8332713
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462019"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="d6e60-103">bookingcustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="d6e60-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e60-104">[bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="d6e60-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6e60-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6e60-105">Permissions</span></span>
<span data-ttu-id="d6e60-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e60-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6e60-108">Permission type</span></span>      | <span data-ttu-id="d6e60-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6e60-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6e60-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6e60-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d6e60-111">予約します。 all、bookingsappointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="d6e60-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d6e60-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6e60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6e60-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6e60-113">Not supported.</span></span>   |
|<span data-ttu-id="d6e60-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6e60-114">Application</span></span> | <span data-ttu-id="d6e60-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6e60-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d6e60-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6e60-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6e60-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d6e60-117">Optional query parameters</span></span>
<span data-ttu-id="d6e60-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d6e60-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6e60-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6e60-119">Request headers</span></span>
| <span data-ttu-id="d6e60-120">名前</span><span class="sxs-lookup"><span data-stu-id="d6e60-120">Name</span></span>      |<span data-ttu-id="d6e60-121">説明</span><span class="sxs-lookup"><span data-stu-id="d6e60-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6e60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6e60-122">Authorization</span></span>  | <span data-ttu-id="d6e60-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d6e60-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e60-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6e60-124">Request body</span></span>
<span data-ttu-id="d6e60-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d6e60-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d6e60-126">応答</span><span class="sxs-lookup"><span data-stu-id="d6e60-126">Response</span></span>
<span data-ttu-id="d6e60-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6e60-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6e60-128">例</span><span class="sxs-lookup"><span data-stu-id="d6e60-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6e60-129">要求</span><span class="sxs-lookup"><span data-stu-id="d6e60-129">Request</span></span>
<span data-ttu-id="d6e60-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6e60-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="d6e60-131">応答</span><span class="sxs-lookup"><span data-stu-id="d6e60-131">Response</span></span>
<span data-ttu-id="d6e60-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6e60-132">The following is an example of the response.</span></span> <span data-ttu-id="d6e60-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d6e60-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d6e60-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d6e60-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
