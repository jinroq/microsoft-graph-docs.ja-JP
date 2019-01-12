---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914639"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="b3a3f-104">bookingSchedulingPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3a3f-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="b3a3f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3a3f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b3a3f-107">Microsoft 予約カレンダーで予定を作成する方法を決定するポリシーのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="b3a3f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3a3f-108">Properties</span></span>
| <span data-ttu-id="b3a3f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3a3f-109">Property</span></span>     | <span data-ttu-id="b3a3f-110">型</span><span class="sxs-lookup"><span data-stu-id="b3a3f-110">Type</span></span>   |<span data-ttu-id="b3a3f-111">説明</span><span class="sxs-lookup"><span data-stu-id="b3a3f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3a3f-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="b3a3f-112">allowStaffSelection</span></span>|<span data-ttu-id="b3a3f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a3f-113">Boolean</span></span>|<span data-ttu-id="b3a3f-114">顧客が予約の特定の人を選択できるようにする場合は true です。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="b3a3f-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="b3a3f-115">maximumAdvance</span></span>|<span data-ttu-id="b3a3f-116">Duration</span><span class="sxs-lookup"><span data-stu-id="b3a3f-116">Duration</span></span>|<span data-ttu-id="b3a3f-117">日の事前に、予約が可能な最大数です。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="b3a3f-118">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="b3a3f-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="b3a3f-119">minimumLeadTime</span></span>|<span data-ttu-id="b3a3f-120">Duration</span><span class="sxs-lookup"><span data-stu-id="b3a3f-120">Duration</span></span>|<span data-ttu-id="b3a3f-121">最小限の時間の前にある予約とキャンセル行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="b3a3f-122">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="b3a3f-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="b3a3f-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="b3a3f-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a3f-124">Boolean</span></span>| <span data-ttu-id="b3a3f-125">予約を作成または変更されたときに電子メール経由でビジネスを通知する場合は true です。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="b3a3f-126">ビジネスの**bookingBusiness**エンティティの**email**プロパティで指定された電子メール アドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="b3a3f-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="b3a3f-127">timeSlotInterval</span></span>|<span data-ttu-id="b3a3f-128">Duration</span><span class="sxs-lookup"><span data-stu-id="b3a3f-128">Duration</span></span>|<span data-ttu-id="b3a3f-129">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、各時間帯の期間です。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3a3f-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3a3f-130">JSON representation</span></span>

<span data-ttu-id="b3a3f-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b3a3f-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
