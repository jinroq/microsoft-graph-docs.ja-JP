---
title: bookingstaffmember の更新
description: 指定した bookingbusiness の bookingStaffMember のプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4124a681332a91d2d909c141b54d412cae9bcc69
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322332"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="1388d-103">bookingstaffmember の更新</span><span class="sxs-lookup"><span data-stu-id="1388d-103">Update bookingstaffmember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1388d-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[bookingStaffMember](../resources/bookingstaffmember.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1388d-104">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1388d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1388d-105">Permissions</span></span>
<span data-ttu-id="1388d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1388d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1388d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1388d-108">Permission type</span></span>      | <span data-ttu-id="1388d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1388d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1388d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1388d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1388d-111">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="1388d-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1388d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1388d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1388d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1388d-113">Not supported.</span></span>   |
|<span data-ttu-id="1388d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1388d-114">Application</span></span> | <span data-ttu-id="1388d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1388d-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1388d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1388d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1388d-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1388d-117">Optional request headers</span></span>
| <span data-ttu-id="1388d-118">名前</span><span class="sxs-lookup"><span data-stu-id="1388d-118">Name</span></span>       | <span data-ttu-id="1388d-119">説明</span><span class="sxs-lookup"><span data-stu-id="1388d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1388d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1388d-120">Authorization</span></span>  | <span data-ttu-id="1388d-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1388d-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1388d-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="1388d-122">Request body</span></span>
<span data-ttu-id="1388d-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1388d-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1388d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1388d-126">Property</span></span>     | <span data-ttu-id="1388d-127">型</span><span class="sxs-lookup"><span data-stu-id="1388d-127">Type</span></span>   |<span data-ttu-id="1388d-128">説明</span><span class="sxs-lookup"><span data-stu-id="1388d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1388d-129">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="1388d-129">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="1388d-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="1388d-130">Boolean</span></span>|<span data-ttu-id="1388d-131">True は、スタッフメンバーが office 365 ユーザーの場合、予約 API は、office 365 のスタッフメンバーの個人用予定表と**workingHours**プロパティを使用して、可用性を判断します。</span><span class="sxs-lookup"><span data-stu-id="1388d-131">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="1388d-132">colorIndex</span><span class="sxs-lookup"><span data-stu-id="1388d-132">colorIndex</span></span>|<span data-ttu-id="1388d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1388d-133">Int32</span></span>|<span data-ttu-id="1388d-134">スタッフメンバーを表す色を識別します。</span><span class="sxs-lookup"><span data-stu-id="1388d-134">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="1388d-135">この色は、予約アプリの [**スタッフの詳細**] ページのカラーパレットに対応しています。</span><span class="sxs-lookup"><span data-stu-id="1388d-135">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="1388d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1388d-136">displayName</span></span>|<span data-ttu-id="1388d-137">String</span><span class="sxs-lookup"><span data-stu-id="1388d-137">String</span></span>|<span data-ttu-id="1388d-138">スタッフメンバーの名前。顧客に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1388d-138">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="1388d-139">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1388d-139">emailAddress</span></span>|<span data-ttu-id="1388d-140">String</span><span class="sxs-lookup"><span data-stu-id="1388d-140">String</span></span>|<span data-ttu-id="1388d-141">スタッフメンバーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="1388d-141">The email address of the staff member.</span></span> <span data-ttu-id="1388d-142">これは、ビジネスと同じ Office 365 テナント内、または別の電子メールドメインに配置できます。</span><span class="sxs-lookup"><span data-stu-id="1388d-142">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="1388d-143">この電子メールアドレスは、ビジネスのスケジューリングポリシーで**sendConfirmationsToOwner**プロパティが true に設定されている場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="1388d-143">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="1388d-144">role</span><span class="sxs-lookup"><span data-stu-id="1388d-144">role</span></span>|<span data-ttu-id="1388d-145">string</span><span class="sxs-lookup"><span data-stu-id="1388d-145">string</span></span>| <span data-ttu-id="1388d-146">業務のスタッフメンバーの役割。</span><span class="sxs-lookup"><span data-stu-id="1388d-146">The role of the staff member in the business.</span></span> <span data-ttu-id="1388d-147">使用可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。</span><span class="sxs-lookup"><span data-stu-id="1388d-147">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="1388d-148">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="1388d-148">useBusinessHours</span></span>|<span data-ttu-id="1388d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="1388d-149">Boolean</span></span>|<span data-ttu-id="1388d-150">True は、スタッフメンバーの利用可能性がビジネスの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティによって決定されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1388d-150">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="1388d-151">False は、可用性がスタッフメンバーの**workingHouse**プロパティの設定によって決定されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1388d-151">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="1388d-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="1388d-152">workingHours</span></span>|<span data-ttu-id="1388d-153">[bookingwork hours](../resources/bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1388d-153">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="1388d-154">スタッフメンバーが予約に使用できる各曜日の時間の範囲。</span><span class="sxs-lookup"><span data-stu-id="1388d-154">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="1388d-155">応答</span><span class="sxs-lookup"><span data-stu-id="1388d-155">Response</span></span>
<span data-ttu-id="1388d-p107">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1388d-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1388d-158">例</span><span class="sxs-lookup"><span data-stu-id="1388d-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1388d-159">要求</span><span class="sxs-lookup"><span data-stu-id="1388d-159">Request</span></span>
<span data-ttu-id="1388d-160">次の例では、スタッフメンバーのスケジュールを変更して月曜日をオフにします。</span><span class="sxs-lookup"><span data-stu-id="1388d-160">The following example changes the staff member's schedule to have Mondays off.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

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
##### <a name="response"></a><span data-ttu-id="1388d-161">応答</span><span class="sxs-lookup"><span data-stu-id="1388d-161">Response</span></span>
<span data-ttu-id="1388d-162">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1388d-162">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
