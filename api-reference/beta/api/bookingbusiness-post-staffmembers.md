---
title: BookingStaffMember を作成する
description: 指定した bookingbusiness に新しいスタッフメンバーを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 2e14e849bfa25c01efa2d912292ccfd3268b20a0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865496"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="cf4b2-103">BookingStaffMember を作成する</span><span class="sxs-lookup"><span data-stu-id="cf4b2-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf4b2-104">指定した[bookingbusiness](../resources/bookingbusiness.md)に新しい[スタッフメンバー](../resources/bookingstaffmember.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="cf4b2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf4b2-105">Permissions</span></span>
<span data-ttu-id="cf4b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf4b2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf4b2-108">Permission type</span></span>      | <span data-ttu-id="cf4b2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf4b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf4b2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf4b2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="cf4b2-111">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="cf4b2-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cf4b2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf4b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf4b2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-113">Not supported.</span></span>   |
|<span data-ttu-id="cf4b2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf4b2-114">Application</span></span> | <span data-ttu-id="cf4b2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cf4b2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf4b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="cf4b2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf4b2-117">Request headers</span></span>
| <span data-ttu-id="cf4b2-118">名前</span><span class="sxs-lookup"><span data-stu-id="cf4b2-118">Name</span></span>       | <span data-ttu-id="cf4b2-119">説明</span><span class="sxs-lookup"><span data-stu-id="cf4b2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf4b2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf4b2-120">Authorization</span></span>  | <span data-ttu-id="cf4b2-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cf4b2-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf4b2-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf4b2-122">Request body</span></span>
<span data-ttu-id="cf4b2-123">要求本文で、 [bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="cf4b2-124">次のプロパティを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-124">You must include the following properties:</span></span>

- <span data-ttu-id="cf4b2-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="cf4b2-125">**displayName**</span></span>
- <span data-ttu-id="cf4b2-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="cf4b2-126">**emailAddress**</span></span>
- <span data-ttu-id="cf4b2-127">**role**</span><span class="sxs-lookup"><span data-stu-id="cf4b2-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="cf4b2-128">応答</span><span class="sxs-lookup"><span data-stu-id="cf4b2-128">Response</span></span>
<span data-ttu-id="cf4b2-129">成功した場合、この`201, Created`メソッドは応答コードと、応答本文で[bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf4b2-130">例</span><span class="sxs-lookup"><span data-stu-id="cf4b2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf4b2-131">要求</span><span class="sxs-lookup"><span data-stu-id="cf4b2-131">Request</span></span>
<span data-ttu-id="cf4b2-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cf4b2-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cf4b2-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf4b2-134">C#</span><span class="sxs-lookup"><span data-stu-id="cf4b2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingstaffmember-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf4b2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cf4b2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingstaffmember-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf4b2-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="cf4b2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingstaffmember-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cf4b2-137">Java</span><span class="sxs-lookup"><span data-stu-id="cf4b2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingstaffmember-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cf4b2-138">要求本文で、 [bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-138">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cf4b2-139">応答</span><span class="sxs-lookup"><span data-stu-id="cf4b2-139">Response</span></span>
<span data-ttu-id="cf4b2-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-140">The following is an example of the response.</span></span> <span data-ttu-id="cf4b2-141">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cf4b2-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cf4b2-142">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
