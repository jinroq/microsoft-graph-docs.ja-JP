---
title: BookingStaffMember を作成します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 43935dbeeda30fb5f69b799993f772ffffa3eeed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838774"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="96046-104">BookingStaffMember を作成します。</span><span class="sxs-lookup"><span data-stu-id="96046-104">Create bookingStaffMember</span></span>

 > <span data-ttu-id="96046-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="96046-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96046-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96046-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="96046-107">指定された[bookingbusiness](../resources/bookingbusiness.md)で、新しい[スタッフのメンバー](../resources/bookingstaffmember.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="96046-107">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="96046-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96046-108">Permissions</span></span>
<span data-ttu-id="96046-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96046-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96046-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96046-111">Permission type</span></span>      | <span data-ttu-id="96046-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96046-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96046-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96046-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="96046-114">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="96046-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="96046-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96046-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96046-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96046-116">Not supported.</span></span>   |
|<span data-ttu-id="96046-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96046-117">Application</span></span> | <span data-ttu-id="96046-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96046-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="96046-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96046-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="96046-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96046-120">Request headers</span></span>
| <span data-ttu-id="96046-121">名前</span><span class="sxs-lookup"><span data-stu-id="96046-121">Name</span></span>       | <span data-ttu-id="96046-122">説明</span><span class="sxs-lookup"><span data-stu-id="96046-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96046-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96046-123">Authorization</span></span>  | <span data-ttu-id="96046-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="96046-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="96046-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="96046-125">Request body</span></span>
<span data-ttu-id="96046-126">要求の本文には、 [bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="96046-126">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="96046-127">次のプロパティを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="96046-127">You must include the following properties:</span></span>

- <span data-ttu-id="96046-128">**displayName**</span><span class="sxs-lookup"><span data-stu-id="96046-128">**displayName**</span></span>
- <span data-ttu-id="96046-129">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="96046-129">**emailAddress**</span></span>
- <span data-ttu-id="96046-130">**ロール**</span><span class="sxs-lookup"><span data-stu-id="96046-130">**role**</span></span>


## <a name="response"></a><span data-ttu-id="96046-131">応答</span><span class="sxs-lookup"><span data-stu-id="96046-131">Response</span></span>
<span data-ttu-id="96046-132">かどうかは成功すると、このメソッドを返します`201, Created`、応答の本体で応答コードと[bookingStaffMember](../resources/bookingstaffmember.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="96046-132">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96046-133">例</span><span class="sxs-lookup"><span data-stu-id="96046-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96046-134">要求</span><span class="sxs-lookup"><span data-stu-id="96046-134">Request</span></span>
<span data-ttu-id="96046-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96046-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Content-type: application/json
Content-length: 309

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "colorIndex":1,
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "role@odata.type":"#microsoft.graph.bookingStaffRole",
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours@odata.type":"#Collection(microsoft.graph.bookingWorkHours)",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
<span data-ttu-id="96046-136">要求の本文には、 [bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="96046-136">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="96046-137">応答</span><span class="sxs-lookup"><span data-stu-id="96046-137">Response</span></span>
<span data-ttu-id="96046-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96046-138">The following is an example of the response.</span></span> <span data-ttu-id="96046-139">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="96046-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="96046-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="96046-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "availabilityIsAffectedByPersonalCalendar":false,
    "colorIndex":1,
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
