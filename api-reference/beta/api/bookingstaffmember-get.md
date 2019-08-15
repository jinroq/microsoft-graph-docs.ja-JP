---
title: BookingStaffMember を取得する
description: 指定した bookingbusiness の bookingStaffMember のプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ff4e82fa69063e25154ce6487248c3ac4150c6d4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419287"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="3979e-103">BookingStaffMember を取得する</span><span class="sxs-lookup"><span data-stu-id="3979e-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3979e-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[bookingStaffMember](../resources/bookingstaffmember.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3979e-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3979e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3979e-105">Permissions</span></span>
<span data-ttu-id="3979e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3979e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3979e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3979e-108">Permission type</span></span>      | <span data-ttu-id="3979e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3979e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3979e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3979e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3979e-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="3979e-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3979e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3979e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3979e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3979e-113">Not supported.</span></span>   |
|<span data-ttu-id="3979e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3979e-114">Application</span></span> | <span data-ttu-id="3979e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3979e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3979e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3979e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3979e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3979e-117">Optional query parameters</span></span>
<span data-ttu-id="3979e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3979e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3979e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3979e-119">Request headers</span></span>
| <span data-ttu-id="3979e-120">名前</span><span class="sxs-lookup"><span data-stu-id="3979e-120">Name</span></span>      |<span data-ttu-id="3979e-121">説明</span><span class="sxs-lookup"><span data-stu-id="3979e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3979e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3979e-122">Authorization</span></span>  | <span data-ttu-id="3979e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3979e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3979e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="3979e-124">Request body</span></span>
<span data-ttu-id="3979e-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3979e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3979e-126">応答</span><span class="sxs-lookup"><span data-stu-id="3979e-126">Response</span></span>
<span data-ttu-id="3979e-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3979e-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3979e-128">例</span><span class="sxs-lookup"><span data-stu-id="3979e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3979e-129">要求</span><span class="sxs-lookup"><span data-stu-id="3979e-129">Request</span></span>
<span data-ttu-id="3979e-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3979e-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3979e-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3979e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3979e-132">C#</span><span class="sxs-lookup"><span data-stu-id="3979e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3979e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3979e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3979e-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="3979e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3979e-135">応答</span><span class="sxs-lookup"><span data-stu-id="3979e-135">Response</span></span>
<span data-ttu-id="3979e-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3979e-136">The following is an example of the response.</span></span> <span data-ttu-id="3979e-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3979e-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3979e-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3979e-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id": "71d64d0e-7225-49b6-b0b1-070d476cda51",
    "displayName": "Samantha Booth",
    "emailAddress": "samanthab@M365B489948.OnMicrosoft.com",
    "availabilityIsAffectedByPersonalCalendar": true,
    "colorIndex": 0,
    "role": "administrator",
    "useBusinessHours": true,
    "workingHours": [
        {
            "day": "monday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "tuesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "wednesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "thursday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "friday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "saturday",
            "timeSlots": []
        },
        {
            "day": "sunday",
            "timeSlots": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
