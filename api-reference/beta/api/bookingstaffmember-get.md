---
title: BookingStaffMember を取得する
description: 指定した bookingbusiness の bookingStaffMember のプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9e5b40b3dd12bdf81268a2d548c95f8b1beb5dc7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636003"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="85d9f-103">BookingStaffMember を取得する</span><span class="sxs-lookup"><span data-stu-id="85d9f-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85d9f-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[bookingStaffMember](../resources/bookingstaffmember.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="85d9f-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85d9f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85d9f-105">Permissions</span></span>
<span data-ttu-id="85d9f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85d9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d9f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85d9f-108">Permission type</span></span>      | <span data-ttu-id="85d9f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85d9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85d9f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85d9f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="85d9f-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="85d9f-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="85d9f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85d9f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d9f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85d9f-113">Not supported.</span></span>   |
|<span data-ttu-id="85d9f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85d9f-114">Application</span></span> | <span data-ttu-id="85d9f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85d9f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="85d9f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85d9f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85d9f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="85d9f-117">Optional query parameters</span></span>
<span data-ttu-id="85d9f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="85d9f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85d9f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85d9f-119">Request headers</span></span>
| <span data-ttu-id="85d9f-120">名前</span><span class="sxs-lookup"><span data-stu-id="85d9f-120">Name</span></span>      |<span data-ttu-id="85d9f-121">説明</span><span class="sxs-lookup"><span data-stu-id="85d9f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85d9f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85d9f-122">Authorization</span></span>  | <span data-ttu-id="85d9f-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="85d9f-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d9f-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="85d9f-124">Request body</span></span>
<span data-ttu-id="85d9f-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="85d9f-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="85d9f-126">応答</span><span class="sxs-lookup"><span data-stu-id="85d9f-126">Response</span></span>
<span data-ttu-id="85d9f-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="85d9f-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85d9f-128">例</span><span class="sxs-lookup"><span data-stu-id="85d9f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85d9f-129">要求</span><span class="sxs-lookup"><span data-stu-id="85d9f-129">Request</span></span>
<span data-ttu-id="85d9f-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85d9f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
##### <a name="response"></a><span data-ttu-id="85d9f-131">応答</span><span class="sxs-lookup"><span data-stu-id="85d9f-131">Response</span></span>
<span data-ttu-id="85d9f-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85d9f-132">The following is an example of the response.</span></span> <span data-ttu-id="85d9f-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="85d9f-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="85d9f-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="85d9f-134">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="85d9f-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="85d9f-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85d9f-136">Visual</span><span class="sxs-lookup"><span data-stu-id="85d9f-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85d9f-137">Java</span><span class="sxs-lookup"><span data-stu-id="85d9f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
