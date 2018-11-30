---
title: bookingStaffMember リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: ad8af6ead37bff4b60c5c4d5ef39ae7628cf100e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066504"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="cde60-104">bookingStaffMember リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cde60-104">bookingStaffMember resource type</span></span>

 > <span data-ttu-id="cde60-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cde60-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cde60-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cde60-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="cde60-107">の[bookingBusiness](bookingbusiness.md)でサービスを提供できるスタッフ メンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="cde60-107">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="cde60-108">スタッフ メンバーは、予約業務を構成すると、またはその他の電子メール プロバイダーからのメール サービスを使用することができます Office 355 テナントの一部にできます。</span><span class="sxs-lookup"><span data-stu-id="cde60-108">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="cde60-109">予定を予約するには、予約の API は、スタッフ メンバーの空き時間を決定するのには次の設定を考慮します。</span><span class="sxs-lookup"><span data-stu-id="cde60-109">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="cde60-110">( [BookingBusiness](bookingbusiness.md)エンティティの**businessHours**プロパティ) のビジネスの操作の時間は、既定では、スタッフ メンバーの全般的な可用性を表します。</span><span class="sxs-lookup"><span data-stu-id="cde60-110">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="cde60-111">**UseBusinessHours**が false の場合は、スタッフ メンバーの特定の作業時間 ( **bookingStaffmember**エンティティのプロパティを**workingHours** ) はそのメンバーの全般的な可用性を表します。</span><span class="sxs-lookup"><span data-stu-id="cde60-111">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="cde60-112">**AvailabilityIsAffectedByPersonalCalendar**が true の場合は、予約 API は最初にによって決定される 1 または 2 のいずれか)、スタッフ メンバーの一般に利用可能な時間を見てし、スタッフ メンバーの個人に、その時間帯に可用性を検証します。予定表、予約をする前にします。</span><span class="sxs-lookup"><span data-stu-id="cde60-112">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="cde60-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="cde60-113">Methods</span></span>

| <span data-ttu-id="cde60-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="cde60-114">Method</span></span>           | <span data-ttu-id="cde60-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cde60-115">Return Type</span></span>    |<span data-ttu-id="cde60-116">説明</span><span class="sxs-lookup"><span data-stu-id="cde60-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cde60-117">スタッフ メンバーの一覧</span><span class="sxs-lookup"><span data-stu-id="cde60-117">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="cde60-118">[bookingStaffMember](bookingstaffmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cde60-118">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="cde60-119">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingStaffMember**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cde60-119">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="cde60-120">BookingStaff を作成します。</span><span class="sxs-lookup"><span data-stu-id="cde60-120">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="cde60-121">[bookingStaffMember](bookingstaffmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cde60-121">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="cde60-122">指定された[bookingbusiness](../resources/bookingbusiness.md)では、新しい**bookingStaffMember**を作成します。</span><span class="sxs-lookup"><span data-stu-id="cde60-122">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="cde60-123">BookingStaffMember を取得します。</span><span class="sxs-lookup"><span data-stu-id="cde60-123">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="cde60-124">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="cde60-124">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="cde60-125">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingStaffMember**の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="cde60-125">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="cde60-126">Update</span><span class="sxs-lookup"><span data-stu-id="cde60-126">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="cde60-127">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="cde60-127">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="cde60-128">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingStaffMember**のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cde60-128">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="cde60-129">削除</span><span class="sxs-lookup"><span data-stu-id="cde60-129">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="cde60-130">なし</span><span class="sxs-lookup"><span data-stu-id="cde60-130">None</span></span> |<span data-ttu-id="cde60-131">指定された[bookingbusiness](../resources/bookingbusiness.md)のスタッフ メンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="cde60-131">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="cde60-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cde60-132">Properties</span></span>
| <span data-ttu-id="cde60-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cde60-133">Property</span></span>     | <span data-ttu-id="cde60-134">型</span><span class="sxs-lookup"><span data-stu-id="cde60-134">Type</span></span>   |<span data-ttu-id="cde60-135">説明</span><span class="sxs-lookup"><span data-stu-id="cde60-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cde60-136">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="cde60-136">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="cde60-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="cde60-137">Boolean</span></span>|<span data-ttu-id="cde60-138">True では、あるスタッフ メンバーが、Office 365 ユーザーの場合は、予約 API はスタッフ メンバーの可用性を確認、Office 365 で、個人用の予定表で予約を行う前にことを意味します。</span><span class="sxs-lookup"><span data-stu-id="cde60-138">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="cde60-139">colorIndex</span><span class="sxs-lookup"><span data-stu-id="cde60-139">colorIndex</span></span>|<span data-ttu-id="cde60-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cde60-140">Int32</span></span>|<span data-ttu-id="cde60-141">スタッフ メンバーを表す色を識別します。</span><span class="sxs-lookup"><span data-stu-id="cde60-141">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="cde60-142">予約アプリケーションでは、**スタッフの詳細**ページでカラー パレットに色が対応しています。</span><span class="sxs-lookup"><span data-stu-id="cde60-142">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="cde60-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cde60-143">displayName</span></span>|<span data-ttu-id="cde60-144">String</span><span class="sxs-lookup"><span data-stu-id="cde60-144">String</span></span>|<span data-ttu-id="cde60-145">顧客に表示されるよう、スタッフ メンバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="cde60-145">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="cde60-146">必須。</span><span class="sxs-lookup"><span data-stu-id="cde60-146">Required.</span></span>|
|<span data-ttu-id="cde60-147">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cde60-147">emailAddress</span></span>|<span data-ttu-id="cde60-148">String</span><span class="sxs-lookup"><span data-stu-id="cde60-148">String</span></span>|<span data-ttu-id="cde60-149">スタッフ メンバーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="cde60-149">The email address of the staff member.</span></span> <span data-ttu-id="cde60-150">ビジネスとして同じ Office 365 テナントにまたは別の電子メール ドメインを指定できます。</span><span class="sxs-lookup"><span data-stu-id="cde60-150">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="cde60-151">**SendConfirmationsToOwner**プロパティが設定されている場合、この e メール アドレスを使用することがビジネスのスケジュー リング ポリシーの場合は true です。</span><span class="sxs-lookup"><span data-stu-id="cde60-151">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="cde60-152">必須。</span><span class="sxs-lookup"><span data-stu-id="cde60-152">Required.</span></span>|
|<span data-ttu-id="cde60-153">id</span><span class="sxs-lookup"><span data-stu-id="cde60-153">id</span></span>|<span data-ttu-id="cde60-154">String</span><span class="sxs-lookup"><span data-stu-id="cde60-154">String</span></span>| <span data-ttu-id="cde60-155">GUID 形式で、スタッフ メンバーの ID。</span><span class="sxs-lookup"><span data-stu-id="cde60-155">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="cde60-156">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cde60-156">Read-only.</span></span>|
|<span data-ttu-id="cde60-157">role</span><span class="sxs-lookup"><span data-stu-id="cde60-157">role</span></span>|<span data-ttu-id="cde60-158">文字列</span><span class="sxs-lookup"><span data-stu-id="cde60-158">string</span></span>| <span data-ttu-id="cde60-159">ビジネスのスタッフの役割です。</span><span class="sxs-lookup"><span data-stu-id="cde60-159">The role of the staff member in the business.</span></span> <span data-ttu-id="cde60-160">可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。</span><span class="sxs-lookup"><span data-stu-id="cde60-160">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="cde60-161">必須。</span><span class="sxs-lookup"><span data-stu-id="cde60-161">Required.</span></span>|
|<span data-ttu-id="cde60-162">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="cde60-162">useBusinessHours</span></span>|<span data-ttu-id="cde60-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="cde60-163">Boolean</span></span>|<span data-ttu-id="cde60-164">真のスタッフ メンバーの可用性とは、ビジネスの**businessHours**プロパティで指定されています。</span><span class="sxs-lookup"><span data-stu-id="cde60-164">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="cde60-165">False は、利用可能時間は、スタッフ メンバーの**workingHours**プロパティの設定によって決定されますを意味します。</span><span class="sxs-lookup"><span data-stu-id="cde60-165">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="cde60-166">workingHours</span><span class="sxs-lookup"><span data-stu-id="cde60-166">workingHours</span></span>|<span data-ttu-id="cde60-167">[bookingWorkHours](bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cde60-167">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="cde60-168">スタッフ メンバーは、予約に使用される 1 週間の各日の時間の範囲です。</span><span class="sxs-lookup"><span data-stu-id="cde60-168">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="cde60-169">既定では、ビジネスの**businessHours**プロパティと同じにするのに初期化されます。</span><span class="sxs-lookup"><span data-stu-id="cde60-169">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cde60-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cde60-170">Relationships</span></span>
<span data-ttu-id="cde60-171">なし</span><span class="sxs-lookup"><span data-stu-id="cde60-171">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cde60-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cde60-172">JSON representation</span></span>

<span data-ttu-id="cde60-173">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cde60-173">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->