---
title: bookingStaffMember リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1de32728aff808975efd3121c9fd99fd0819b06c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013088"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="d1722-104">bookingStaffMember リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1722-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d1722-105">[Bookingbusiness](bookingbusiness.md)でサービスを提供するスタッフメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d1722-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="d1722-106">スタッフメンバーは、予約ビジネスが構成されている Office 355 テナントの一部として、または他の電子メールプロバイダーの電子メールサービスを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d1722-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="d1722-107">予約時に予約 API は、次の設定を考慮してスタッフメンバーの可用性を判断します。</span><span class="sxs-lookup"><span data-stu-id="d1722-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="d1722-108">既定では、ビジネスの運用時間 ( [Bookingbusiness](bookingbusiness.md)エンティティの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティ) は、スタッフメンバーの一般利用可能性を表します。</span><span class="sxs-lookup"><span data-stu-id="d1722-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="d1722-109">**UseBusinessHours**が false の場合、スタッフメンバーの特定の勤務時間 ( **BookingStaffmember**エンティティの**workingHours**プロパティ) は、そのメンバーの一般的な利用可能時間を表します。</span><span class="sxs-lookup"><span data-stu-id="d1722-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="d1722-110">**AvailabilityIsAffectedByPersonalCalendar**が true の場合、予約 API は最初にスタッフメンバーの使用可能な時間 (#1 または #2 のどちらかによって決まります) を調べて、スタッフメンバーの個人の時間帯に空き時間情報を確認します。予約する前に、予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="d1722-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="d1722-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1722-111">Methods</span></span>

| <span data-ttu-id="d1722-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1722-112">Method</span></span>           | <span data-ttu-id="d1722-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d1722-113">Return Type</span></span>    |<span data-ttu-id="d1722-114">説明</span><span class="sxs-lookup"><span data-stu-id="d1722-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1722-115">スタッフメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1722-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="d1722-116">[bookingStaffMember](bookingstaffmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d1722-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="d1722-117">指定した[bookingbusiness](../resources/bookingbusiness.md)の**bookingStaffMember**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1722-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="d1722-118">BookingStaff を作成する</span><span class="sxs-lookup"><span data-stu-id="d1722-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="d1722-119">[bookingStaffMember](bookingstaffmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d1722-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="d1722-120">指定した[bookingbusiness](../resources/bookingbusiness.md)で新しい**bookingStaffMember**を作成します。</span><span class="sxs-lookup"><span data-stu-id="d1722-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="d1722-121">BookingStaffMember を取得する</span><span class="sxs-lookup"><span data-stu-id="d1722-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="d1722-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="d1722-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="d1722-123">指定した[bookingbusiness](../resources/bookingbusiness.md)の**bookingStaffMember**のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1722-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="d1722-124">Update</span><span class="sxs-lookup"><span data-stu-id="d1722-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="d1722-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="d1722-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="d1722-126">指定した[bookingbusiness](../resources/bookingbusiness.md)の**bookingStaffMember**のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1722-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="d1722-127">Delete</span><span class="sxs-lookup"><span data-stu-id="d1722-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="d1722-128">None</span><span class="sxs-lookup"><span data-stu-id="d1722-128">None</span></span> |<span data-ttu-id="d1722-129">指定した[bookingbusiness](../resources/bookingbusiness.md)のスタッフメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="d1722-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="d1722-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1722-130">Properties</span></span>
| <span data-ttu-id="d1722-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1722-131">Property</span></span>     | <span data-ttu-id="d1722-132">型</span><span class="sxs-lookup"><span data-stu-id="d1722-132">Type</span></span>   |<span data-ttu-id="d1722-133">説明</span><span class="sxs-lookup"><span data-stu-id="d1722-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1722-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="d1722-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="d1722-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1722-135">Boolean</span></span>|<span data-ttu-id="d1722-136">True は、スタッフメンバーが Office 365 ユーザーの場合、予約 API は、予約を行う前に Office 365 の個人用予定表でスタッフメンバーの利用可能性を確認します。</span><span class="sxs-lookup"><span data-stu-id="d1722-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="d1722-137">colorIndex</span><span class="sxs-lookup"><span data-stu-id="d1722-137">colorIndex</span></span>|<span data-ttu-id="d1722-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d1722-138">Int32</span></span>|<span data-ttu-id="d1722-139">スタッフメンバーを表す色を識別します。</span><span class="sxs-lookup"><span data-stu-id="d1722-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="d1722-140">この色は、予約アプリの [**スタッフの詳細**] ページのカラーパレットに対応しています。</span><span class="sxs-lookup"><span data-stu-id="d1722-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="d1722-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d1722-141">displayName</span></span>|<span data-ttu-id="d1722-142">String</span><span class="sxs-lookup"><span data-stu-id="d1722-142">String</span></span>|<span data-ttu-id="d1722-143">スタッフメンバーの名前。顧客に表示されます。</span><span class="sxs-lookup"><span data-stu-id="d1722-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="d1722-144">必須です。</span><span class="sxs-lookup"><span data-stu-id="d1722-144">Required.</span></span>|
|<span data-ttu-id="d1722-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d1722-145">emailAddress</span></span>|<span data-ttu-id="d1722-146">String</span><span class="sxs-lookup"><span data-stu-id="d1722-146">String</span></span>|<span data-ttu-id="d1722-147">スタッフメンバーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="d1722-147">The email address of the staff member.</span></span> <span data-ttu-id="d1722-148">これは、ビジネスと同じ Office 365 テナント内、または別の電子メールドメインに配置できます。</span><span class="sxs-lookup"><span data-stu-id="d1722-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="d1722-149">この電子メールアドレスは、ビジネスのスケジューリングポリシーで**sendConfirmationsToOwner**プロパティが true に設定されている場合に使用できます。</span><span class="sxs-lookup"><span data-stu-id="d1722-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="d1722-150">必須。</span><span class="sxs-lookup"><span data-stu-id="d1722-150">Required.</span></span>|
|<span data-ttu-id="d1722-151">id</span><span class="sxs-lookup"><span data-stu-id="d1722-151">id</span></span>|<span data-ttu-id="d1722-152">文字列</span><span class="sxs-lookup"><span data-stu-id="d1722-152">String</span></span>| <span data-ttu-id="d1722-153">GUID 形式のスタッフメンバーの ID。</span><span class="sxs-lookup"><span data-stu-id="d1722-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="d1722-154">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d1722-154">Read-only.</span></span>|
|<span data-ttu-id="d1722-155">role</span><span class="sxs-lookup"><span data-stu-id="d1722-155">role</span></span>|<span data-ttu-id="d1722-156">string</span><span class="sxs-lookup"><span data-stu-id="d1722-156">string</span></span>| <span data-ttu-id="d1722-157">業務のスタッフメンバーの役割。</span><span class="sxs-lookup"><span data-stu-id="d1722-157">The role of the staff member in the business.</span></span> <span data-ttu-id="d1722-158">使用可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。</span><span class="sxs-lookup"><span data-stu-id="d1722-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="d1722-159">必須です。</span><span class="sxs-lookup"><span data-stu-id="d1722-159">Required.</span></span>|
|<span data-ttu-id="d1722-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="d1722-160">useBusinessHours</span></span>|<span data-ttu-id="d1722-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1722-161">Boolean</span></span>|<span data-ttu-id="d1722-162">True は、スタッフメンバーの可用性が、ビジネスの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティで指定されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="d1722-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="d1722-163">False は、可用性がスタッフメンバーの**workingHours**プロパティの設定によって決定されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="d1722-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="d1722-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="d1722-164">workingHours</span></span>|<span data-ttu-id="d1722-165">[Bookingwork hours](bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d1722-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="d1722-166">スタッフメンバーが予約に使用できる各曜日の時間の範囲。</span><span class="sxs-lookup"><span data-stu-id="d1722-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="d1722-167">既定では、ビジネスの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティと同じになるように初期化されます。</span><span class="sxs-lookup"><span data-stu-id="d1722-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1722-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1722-168">Relationships</span></span>
<span data-ttu-id="d1722-169">なし</span><span class="sxs-lookup"><span data-stu-id="d1722-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d1722-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1722-170">JSON representation</span></span>

<span data-ttu-id="d1722-171">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1722-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
