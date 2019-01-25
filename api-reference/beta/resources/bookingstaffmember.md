---
title: bookingStaffMember リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520278"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="b96bb-104">bookingStaffMember リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b96bb-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b96bb-105">の[bookingBusiness](bookingbusiness.md)でサービスを提供できるスタッフ メンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="b96bb-106">スタッフ メンバーは、予約業務を構成すると、またはその他の電子メール プロバイダーからのメール サービスを使用することができます Office 355 テナントの一部にできます。</span><span class="sxs-lookup"><span data-stu-id="b96bb-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="b96bb-107">予定を予約するには、予約の API は、スタッフ メンバーの空き時間を決定するのには次の設定を考慮します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="b96bb-108">( [BookingBusiness](bookingbusiness.md)エンティティの**businessHours**プロパティ) のビジネスの操作の時間は、既定では、スタッフ メンバーの全般的な可用性を表します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="b96bb-109">**UseBusinessHours**が false の場合は、スタッフ メンバーの特定の作業時間 ( **bookingStaffmember**エンティティのプロパティを**workingHours** ) はそのメンバーの全般的な可用性を表します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="b96bb-110">**AvailabilityIsAffectedByPersonalCalendar**が true の場合は、予約 API は最初にによって決定される 1 または 2 のいずれか)、スタッフ メンバーの一般に利用可能な時間を見てし、スタッフ メンバーの個人に、その時間帯に可用性を検証します。予定表、予約をする前にします。</span><span class="sxs-lookup"><span data-stu-id="b96bb-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="b96bb-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="b96bb-111">Methods</span></span>

| <span data-ttu-id="b96bb-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="b96bb-112">Method</span></span>           | <span data-ttu-id="b96bb-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b96bb-113">Return Type</span></span>    |<span data-ttu-id="b96bb-114">説明</span><span class="sxs-lookup"><span data-stu-id="b96bb-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b96bb-115">スタッフ メンバーの一覧</span><span class="sxs-lookup"><span data-stu-id="b96bb-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="b96bb-116">[bookingStaffMember](bookingstaffmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b96bb-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="b96bb-117">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingStaffMember**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b96bb-118">BookingStaff を作成します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="b96bb-119">[bookingStaffMember](bookingstaffmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b96bb-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="b96bb-120">指定された[bookingbusiness](../resources/bookingbusiness.md)では、新しい**bookingStaffMember**を作成します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b96bb-121">BookingStaffMember を取得します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="b96bb-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b96bb-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="b96bb-123">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingStaffMember**の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b96bb-124">Update</span><span class="sxs-lookup"><span data-stu-id="b96bb-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="b96bb-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b96bb-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="b96bb-126">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingStaffMember**のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b96bb-127">Delete</span><span class="sxs-lookup"><span data-stu-id="b96bb-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="b96bb-128">なし</span><span class="sxs-lookup"><span data-stu-id="b96bb-128">None</span></span> |<span data-ttu-id="b96bb-129">指定された[bookingbusiness](../resources/bookingbusiness.md)のスタッフ メンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="b96bb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b96bb-130">Properties</span></span>
| <span data-ttu-id="b96bb-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b96bb-131">Property</span></span>     | <span data-ttu-id="b96bb-132">型</span><span class="sxs-lookup"><span data-stu-id="b96bb-132">Type</span></span>   |<span data-ttu-id="b96bb-133">説明</span><span class="sxs-lookup"><span data-stu-id="b96bb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b96bb-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="b96bb-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="b96bb-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="b96bb-135">Boolean</span></span>|<span data-ttu-id="b96bb-136">True では、あるスタッフ メンバーが、Office 365 ユーザーの場合は、予約 API はスタッフ メンバーの可用性を確認、Office 365 で、個人用の予定表で予約を行う前にことを意味します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="b96bb-137">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="b96bb-137">colorIndex</span></span>|<span data-ttu-id="b96bb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b96bb-138">Int32</span></span>|<span data-ttu-id="b96bb-139">スタッフ メンバーを表す色を識別します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="b96bb-140">予約アプリケーションでは、**スタッフの詳細**ページでカラー パレットに色が対応しています。</span><span class="sxs-lookup"><span data-stu-id="b96bb-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="b96bb-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b96bb-141">displayName</span></span>|<span data-ttu-id="b96bb-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b96bb-142">String</span></span>|<span data-ttu-id="b96bb-143">顧客に表示されるよう、スタッフ メンバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="b96bb-144">必須です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-144">Required.</span></span>|
|<span data-ttu-id="b96bb-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b96bb-145">emailAddress</span></span>|<span data-ttu-id="b96bb-146">String</span><span class="sxs-lookup"><span data-stu-id="b96bb-146">String</span></span>|<span data-ttu-id="b96bb-147">スタッフ メンバーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b96bb-147">The email address of the staff member.</span></span> <span data-ttu-id="b96bb-148">ビジネスとして同じ Office 365 テナントにまたは別の電子メール ドメインを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b96bb-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="b96bb-149">**SendConfirmationsToOwner**プロパティが設定されている場合、この e メール アドレスを使用することがビジネスのスケジュー リング ポリシーの場合は true です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="b96bb-150">必須です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-150">Required.</span></span>|
|<span data-ttu-id="b96bb-151">id</span><span class="sxs-lookup"><span data-stu-id="b96bb-151">id</span></span>|<span data-ttu-id="b96bb-152">文字列</span><span class="sxs-lookup"><span data-stu-id="b96bb-152">String</span></span>| <span data-ttu-id="b96bb-153">GUID 形式で、スタッフ メンバーの ID。</span><span class="sxs-lookup"><span data-stu-id="b96bb-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="b96bb-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-154">Read-only.</span></span>|
|<span data-ttu-id="b96bb-155">role</span><span class="sxs-lookup"><span data-stu-id="b96bb-155">role</span></span>|<span data-ttu-id="b96bb-156">string</span><span class="sxs-lookup"><span data-stu-id="b96bb-156">string</span></span>| <span data-ttu-id="b96bb-157">ビジネスのスタッフの役割です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-157">The role of the staff member in the business.</span></span> <span data-ttu-id="b96bb-158">可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="b96bb-159">必須です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-159">Required.</span></span>|
|<span data-ttu-id="b96bb-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="b96bb-160">useBusinessHours</span></span>|<span data-ttu-id="b96bb-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="b96bb-161">Boolean</span></span>|<span data-ttu-id="b96bb-162">真のスタッフ メンバーの可用性とは、ビジネスの**businessHours**プロパティで指定されています。</span><span class="sxs-lookup"><span data-stu-id="b96bb-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="b96bb-163">False は、利用可能時間は、スタッフ メンバーの**workingHours**プロパティの設定によって決定されますを意味します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="b96bb-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="b96bb-164">workingHours</span></span>|<span data-ttu-id="b96bb-165">[bookingWorkHours](bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b96bb-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="b96bb-166">スタッフ メンバーは、予約に使用される 1 週間の各日の時間の範囲です。</span><span class="sxs-lookup"><span data-stu-id="b96bb-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="b96bb-167">既定では、ビジネスの**businessHours**プロパティと同じにするのに初期化されます。</span><span class="sxs-lookup"><span data-stu-id="b96bb-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b96bb-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b96bb-168">Relationships</span></span>
<span data-ttu-id="b96bb-169">なし</span><span class="sxs-lookup"><span data-stu-id="b96bb-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b96bb-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b96bb-170">JSON representation</span></span>

<span data-ttu-id="b96bb-171">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b96bb-171">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
