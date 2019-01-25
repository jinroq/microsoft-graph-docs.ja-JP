---
title: BookingStaffMember を作成します。
description: 指定された bookingbusiness で、新しいスタッフのメンバーを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f3f13f30f646da8bf0fc8e32075002c0e591e902
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518612"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="c0c6e-103">BookingStaffMember を作成します。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0c6e-104">指定された[bookingbusiness](../resources/bookingbusiness.md)で、新しい[スタッフのメンバー](../resources/bookingstaffmember.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c0c6e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0c6e-105">Permissions</span></span>
<span data-ttu-id="c0c6e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c6e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0c6e-108">Permission type</span></span>      | <span data-ttu-id="c0c6e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0c6e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c6e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0c6e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0c6e-111">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c0c6e-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c0c6e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0c6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c6e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-113">Not supported.</span></span>   |
|<span data-ttu-id="c0c6e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0c6e-114">Application</span></span> | <span data-ttu-id="c0c6e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c0c6e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0c6e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="c0c6e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0c6e-117">Request headers</span></span>
| <span data-ttu-id="c0c6e-118">名前</span><span class="sxs-lookup"><span data-stu-id="c0c6e-118">Name</span></span>       | <span data-ttu-id="c0c6e-119">説明</span><span class="sxs-lookup"><span data-stu-id="c0c6e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0c6e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c6e-120">Authorization</span></span>  | <span data-ttu-id="c0c6e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c0c6e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c6e-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0c6e-122">Request body</span></span>
<span data-ttu-id="c0c6e-123">要求の本文には、 [bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="c0c6e-124">次のプロパティを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-124">You must include the following properties:</span></span>

- <span data-ttu-id="c0c6e-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="c0c6e-125">**displayName**</span></span>
- <span data-ttu-id="c0c6e-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="c0c6e-126">**emailAddress**</span></span>
- <span data-ttu-id="c0c6e-127">**役割**</span><span class="sxs-lookup"><span data-stu-id="c0c6e-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="c0c6e-128">応答</span><span class="sxs-lookup"><span data-stu-id="c0c6e-128">Response</span></span>
<span data-ttu-id="c0c6e-129">かどうかは成功すると、このメソッドを返します`201, Created`、応答の本体で応答コードと[bookingStaffMember](../resources/bookingstaffmember.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c6e-130">例</span><span class="sxs-lookup"><span data-stu-id="c0c6e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0c6e-131">要求</span><span class="sxs-lookup"><span data-stu-id="c0c6e-131">Request</span></span>
<span data-ttu-id="c0c6e-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="c0c6e-133">要求の本文には、 [bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-133">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c0c6e-134">応答</span><span class="sxs-lookup"><span data-stu-id="c0c6e-134">Response</span></span>
<span data-ttu-id="c0c6e-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-135">The following is an example of the response.</span></span> <span data-ttu-id="c0c6e-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c0c6e-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c0c6e-137">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
