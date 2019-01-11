---
title: Bookingstaffmember を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 4ba2ea126f916b6bd91b83bdd81e24d30fae8ac4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824984"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="5910c-104">Bookingstaffmember を更新します。</span><span class="sxs-lookup"><span data-stu-id="5910c-104">Update bookingstaffmember</span></span>

 > <span data-ttu-id="5910c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5910c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5910c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5910c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="5910c-107">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 [bookingStaffMember](../resources/bookingstaffmember.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5910c-107">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5910c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5910c-108">Permissions</span></span>
<span data-ttu-id="5910c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5910c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5910c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5910c-111">Permission type</span></span>      | <span data-ttu-id="5910c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5910c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5910c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5910c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="5910c-114">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5910c-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5910c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5910c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5910c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5910c-116">Not supported.</span></span>   |
|<span data-ttu-id="5910c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5910c-117">Application</span></span> | <span data-ttu-id="5910c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5910c-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5910c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5910c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5910c-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5910c-120">Optional request headers</span></span>
| <span data-ttu-id="5910c-121">名前</span><span class="sxs-lookup"><span data-stu-id="5910c-121">Name</span></span>       | <span data-ttu-id="5910c-122">説明</span><span class="sxs-lookup"><span data-stu-id="5910c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5910c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5910c-123">Authorization</span></span>  | <span data-ttu-id="5910c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5910c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5910c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5910c-125">Request body</span></span>
<span data-ttu-id="5910c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5910c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5910c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5910c-129">Property</span></span>     | <span data-ttu-id="5910c-130">種類</span><span class="sxs-lookup"><span data-stu-id="5910c-130">Type</span></span>   |<span data-ttu-id="5910c-131">説明</span><span class="sxs-lookup"><span data-stu-id="5910c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5910c-132">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="5910c-132">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="5910c-133">ブール型</span><span class="sxs-lookup"><span data-stu-id="5910c-133">Boolean</span></span>|<span data-ttu-id="5910c-134">True は、スタッフ メンバーが、Office 365 ユーザーの場合は、予約 API は**workingHours**プロパティと同様に Office 365 で、スタッフ メンバーの個人用予定表の可用性を決定します。</span><span class="sxs-lookup"><span data-stu-id="5910c-134">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="5910c-135">colorIndex</span><span class="sxs-lookup"><span data-stu-id="5910c-135">colorIndex</span></span>|<span data-ttu-id="5910c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5910c-136">Int32</span></span>|<span data-ttu-id="5910c-137">スタッフ メンバーを表す色を識別します。</span><span class="sxs-lookup"><span data-stu-id="5910c-137">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="5910c-138">予約アプリケーションでは、**スタッフの詳細**ページでカラー パレットに色が対応しています。</span><span class="sxs-lookup"><span data-stu-id="5910c-138">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="5910c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5910c-139">displayName</span></span>|<span data-ttu-id="5910c-140">String</span><span class="sxs-lookup"><span data-stu-id="5910c-140">String</span></span>|<span data-ttu-id="5910c-141">顧客に表示されるよう、スタッフ メンバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="5910c-141">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="5910c-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5910c-142">emailAddress</span></span>|<span data-ttu-id="5910c-143">String</span><span class="sxs-lookup"><span data-stu-id="5910c-143">String</span></span>|<span data-ttu-id="5910c-144">スタッフ メンバーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="5910c-144">The email address of the staff member.</span></span> <span data-ttu-id="5910c-145">ビジネスとして同じ Office 365 テナントにまたは別の電子メール ドメインを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5910c-145">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="5910c-146">**SendConfirmationsToOwner**プロパティが設定されている場合、この電子メール アドレスが使用されるビジネスのスケジュー リング ポリシーの場合は true です。</span><span class="sxs-lookup"><span data-stu-id="5910c-146">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="5910c-147">role</span><span class="sxs-lookup"><span data-stu-id="5910c-147">role</span></span>|<span data-ttu-id="5910c-148">文字列</span><span class="sxs-lookup"><span data-stu-id="5910c-148">string</span></span>| <span data-ttu-id="5910c-149">ビジネスのスタッフの役割です。</span><span class="sxs-lookup"><span data-stu-id="5910c-149">The role of the staff member in the business.</span></span> <span data-ttu-id="5910c-150">可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。</span><span class="sxs-lookup"><span data-stu-id="5910c-150">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="5910c-151">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="5910c-151">useBusinessHours</span></span>|<span data-ttu-id="5910c-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="5910c-152">Boolean</span></span>|<span data-ttu-id="5910c-153">True では、スタッフ メンバーの可用性は、ビジネスの**businessHours**プロパティによって決定されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="5910c-153">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="5910c-154">False は、利用可能時間は、スタッフ メンバーの**workingHouse**プロパティの設定によって決定されますを意味します。</span><span class="sxs-lookup"><span data-stu-id="5910c-154">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="5910c-155">workingHours</span><span class="sxs-lookup"><span data-stu-id="5910c-155">workingHours</span></span>|<span data-ttu-id="5910c-156">[bookingWorkHours](../resources/bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5910c-156">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="5910c-157">スタッフ メンバーは、予約に使用される 1 週間の各日の時間の範囲です。</span><span class="sxs-lookup"><span data-stu-id="5910c-157">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="5910c-158">応答</span><span class="sxs-lookup"><span data-stu-id="5910c-158">Response</span></span>
<span data-ttu-id="5910c-p109">成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5910c-p109">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5910c-161">例</span><span class="sxs-lookup"><span data-stu-id="5910c-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5910c-162">要求</span><span class="sxs-lookup"><span data-stu-id="5910c-162">Request</span></span>
<span data-ttu-id="5910c-163">次の使用例では、毎週月曜日にのスタッフ メンバーのスケジュールを変更します。</span><span class="sxs-lookup"><span data-stu-id="5910c-163">The following example changes the staff member's schedule to have Mondays off.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5910c-164">応答</span><span class="sxs-lookup"><span data-stu-id="5910c-164">Response</span></span>
<span data-ttu-id="5910c-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5910c-165">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
