---
title: bookingStaffMember を取得する
description: 指定した bookingbusiness の bookingStaffMember のプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6228bc87c2d4ac4d31b388aacc9b033443f3d389
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462110"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="a4139-103">bookingStaffMember を取得する</span><span class="sxs-lookup"><span data-stu-id="a4139-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4139-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[bookingStaffMember](../resources/bookingstaffmember.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a4139-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a4139-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a4139-105">Permissions</span></span>
<span data-ttu-id="a4139-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4139-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4139-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4139-108">Permission type</span></span>      | <span data-ttu-id="a4139-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4139-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4139-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4139-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a4139-111">予約します。 all、bookingsappointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="a4139-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a4139-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4139-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4139-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4139-113">Not supported.</span></span>   |
|<span data-ttu-id="a4139-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4139-114">Application</span></span> | <span data-ttu-id="a4139-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4139-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a4139-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4139-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4139-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a4139-117">Optional query parameters</span></span>
<span data-ttu-id="a4139-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a4139-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4139-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4139-119">Request headers</span></span>
| <span data-ttu-id="a4139-120">名前</span><span class="sxs-lookup"><span data-stu-id="a4139-120">Name</span></span>      |<span data-ttu-id="a4139-121">説明</span><span class="sxs-lookup"><span data-stu-id="a4139-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a4139-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4139-122">Authorization</span></span>  | <span data-ttu-id="a4139-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a4139-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4139-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4139-124">Request body</span></span>
<span data-ttu-id="a4139-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a4139-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a4139-126">応答</span><span class="sxs-lookup"><span data-stu-id="a4139-126">Response</span></span>
<span data-ttu-id="a4139-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4139-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4139-128">例</span><span class="sxs-lookup"><span data-stu-id="a4139-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4139-129">要求</span><span class="sxs-lookup"><span data-stu-id="a4139-129">Request</span></span>
<span data-ttu-id="a4139-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4139-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
##### <a name="response"></a><span data-ttu-id="a4139-131">応答</span><span class="sxs-lookup"><span data-stu-id="a4139-131">Response</span></span>
<span data-ttu-id="a4139-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4139-132">The following is an example of the response.</span></span> <span data-ttu-id="a4139-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a4139-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a4139-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a4139-134">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
