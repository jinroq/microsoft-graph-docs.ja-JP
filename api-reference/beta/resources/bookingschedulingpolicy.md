---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 7a16e9a2ec4e64978dd3c20f7510cfd42d76e826
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069900"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="8cd4c-104">bookingSchedulingPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cd4c-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="8cd4c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cd4c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="8cd4c-107">Microsoft 予約カレンダーで予定を作成する方法を決定するポリシーのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="8cd4c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cd4c-108">Properties</span></span>
| <span data-ttu-id="8cd4c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cd4c-109">Property</span></span>     | <span data-ttu-id="8cd4c-110">型</span><span class="sxs-lookup"><span data-stu-id="8cd4c-110">Type</span></span>   |<span data-ttu-id="8cd4c-111">説明</span><span class="sxs-lookup"><span data-stu-id="8cd4c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cd4c-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="8cd4c-112">allowStaffSelection</span></span>|<span data-ttu-id="8cd4c-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="8cd4c-113">Boolean</span></span>|<span data-ttu-id="8cd4c-114">顧客が予約の特定の人を選択できるようにする場合は true です。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="8cd4c-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="8cd4c-115">maximumAdvance</span></span>|<span data-ttu-id="8cd4c-116">Duration</span><span class="sxs-lookup"><span data-stu-id="8cd4c-116">Duration</span></span>|<span data-ttu-id="8cd4c-117">日の事前に、予約が可能な最大数です。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="8cd4c-118">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="8cd4c-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="8cd4c-119">minimumLeadTime</span></span>|<span data-ttu-id="8cd4c-120">Duration</span><span class="sxs-lookup"><span data-stu-id="8cd4c-120">Duration</span></span>|<span data-ttu-id="8cd4c-121">最小限の時間の前にある予約とキャンセル行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="8cd4c-122">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="8cd4c-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="8cd4c-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="8cd4c-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="8cd4c-124">Boolean</span></span>| <span data-ttu-id="8cd4c-125">予約を作成または変更されたときに電子メール経由でビジネスを通知する場合は true です。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="8cd4c-126">ビジネスの**bookingBusiness**エンティティの**email**プロパティで指定された電子メール アドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="8cd4c-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="8cd4c-127">timeSlotInterval</span></span>|<span data-ttu-id="8cd4c-128">Duration</span><span class="sxs-lookup"><span data-stu-id="8cd4c-128">Duration</span></span>|<span data-ttu-id="8cd4c-129">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、各時間帯の期間です。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cd4c-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cd4c-130">JSON representation</span></span>

<span data-ttu-id="8cd4c-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8cd4c-131">The following is a JSON representation of the resource.</span></span>

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