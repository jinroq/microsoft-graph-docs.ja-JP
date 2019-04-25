---
title: bookingSchedulingPolicy リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543754"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="8102b-104">bookingSchedulingPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8102b-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="8102b-105">Microsoft の予約予定表で予定を作成する方法を決定する一連のポリシーを表します。</span><span class="sxs-lookup"><span data-stu-id="8102b-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="8102b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8102b-106">Properties</span></span>
| <span data-ttu-id="8102b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8102b-107">Property</span></span>     | <span data-ttu-id="8102b-108">型</span><span class="sxs-lookup"><span data-stu-id="8102b-108">Type</span></span>   |<span data-ttu-id="8102b-109">説明</span><span class="sxs-lookup"><span data-stu-id="8102b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8102b-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="8102b-110">allowStaffSelection</span></span>|<span data-ttu-id="8102b-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="8102b-111">Boolean</span></span>|<span data-ttu-id="8102b-112">True の場合、ユーザーは予約の特定のユーザーを選択することができます。</span><span class="sxs-lookup"><span data-stu-id="8102b-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="8102b-113">maximumadvance</span><span class="sxs-lookup"><span data-stu-id="8102b-113">maximumAdvance</span></span>|<span data-ttu-id="8102b-114">期間</span><span class="sxs-lookup"><span data-stu-id="8102b-114">Duration</span></span>|<span data-ttu-id="8102b-115">予約を事前に作成できる最大日数。</span><span class="sxs-lookup"><span data-stu-id="8102b-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="8102b-116">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に従います。</span><span class="sxs-lookup"><span data-stu-id="8102b-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="8102b-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="8102b-117">minimumLeadTime</span></span>|<span data-ttu-id="8102b-118">期間</span><span class="sxs-lookup"><span data-stu-id="8102b-118">Duration</span></span>|<span data-ttu-id="8102b-119">予約と取り消しを行う必要のある最小時間。</span><span class="sxs-lookup"><span data-stu-id="8102b-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="8102b-120">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式に従います。</span><span class="sxs-lookup"><span data-stu-id="8102b-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="8102b-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="8102b-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="8102b-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="8102b-122">Boolean</span></span>| <span data-ttu-id="8102b-123">True は、予約が作成または変更されたときに電子メールでビジネスに通知します。</span><span class="sxs-lookup"><span data-stu-id="8102b-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="8102b-124">会社の**bookingbusiness**エンティティの**email**プロパティで指定された電子メールアドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="8102b-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="8102b-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="8102b-125">timeSlotInterval</span></span>|<span data-ttu-id="8102b-126">期間</span><span class="sxs-lookup"><span data-stu-id="8102b-126">Duration</span></span>|<span data-ttu-id="8102b-127">各時間帯の期間は、 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で示されます。</span><span class="sxs-lookup"><span data-stu-id="8102b-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8102b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8102b-128">JSON representation</span></span>

<span data-ttu-id="8102b-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8102b-129">The following is a JSON representation of the resource.</span></span>

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
