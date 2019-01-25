---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523450"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="dc689-104">bookingSchedulingPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc689-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="dc689-105">Microsoft 予約カレンダーで予定を作成する方法を決定するポリシーのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="dc689-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="dc689-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc689-106">Properties</span></span>
| <span data-ttu-id="dc689-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc689-107">Property</span></span>     | <span data-ttu-id="dc689-108">型</span><span class="sxs-lookup"><span data-stu-id="dc689-108">Type</span></span>   |<span data-ttu-id="dc689-109">説明</span><span class="sxs-lookup"><span data-stu-id="dc689-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc689-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="dc689-110">allowStaffSelection</span></span>|<span data-ttu-id="dc689-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="dc689-111">Boolean</span></span>|<span data-ttu-id="dc689-112">顧客が予約の特定の人を選択できるようにする場合は true です。</span><span class="sxs-lookup"><span data-stu-id="dc689-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="dc689-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="dc689-113">maximumAdvance</span></span>|<span data-ttu-id="dc689-114">Duration</span><span class="sxs-lookup"><span data-stu-id="dc689-114">Duration</span></span>|<span data-ttu-id="dc689-115">日の事前に、予約が可能な最大数です。</span><span class="sxs-lookup"><span data-stu-id="dc689-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="dc689-116">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。</span><span class="sxs-lookup"><span data-stu-id="dc689-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="dc689-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="dc689-117">minimumLeadTime</span></span>|<span data-ttu-id="dc689-118">Duration</span><span class="sxs-lookup"><span data-stu-id="dc689-118">Duration</span></span>|<span data-ttu-id="dc689-119">最小限の時間の前にある予約とキャンセル行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc689-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="dc689-120">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に依存します。</span><span class="sxs-lookup"><span data-stu-id="dc689-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="dc689-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="dc689-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="dc689-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="dc689-122">Boolean</span></span>| <span data-ttu-id="dc689-123">予約を作成または変更されたときに電子メール経由でビジネスを通知する場合は true です。</span><span class="sxs-lookup"><span data-stu-id="dc689-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="dc689-124">ビジネスの**bookingBusiness**エンティティの**email**プロパティで指定された電子メール アドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="dc689-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="dc689-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="dc689-125">timeSlotInterval</span></span>|<span data-ttu-id="dc689-126">Duration</span><span class="sxs-lookup"><span data-stu-id="dc689-126">Duration</span></span>|<span data-ttu-id="dc689-127">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、各時間帯の期間です。</span><span class="sxs-lookup"><span data-stu-id="dc689-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc689-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc689-128">JSON representation</span></span>

<span data-ttu-id="dc689-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc689-129">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
