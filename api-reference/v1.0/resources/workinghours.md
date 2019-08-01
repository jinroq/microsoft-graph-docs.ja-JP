---
title: workingHours リソースの種類
description: ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c3449e64f94a3e90bae443a23e7b941116df0291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033328"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="1f83a-103">workingHours リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f83a-103">workingHours resource type</span></span>

<span data-ttu-id="1f83a-104">ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。</span><span class="sxs-lookup"><span data-stu-id="1f83a-104">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="1f83a-105">アクティビティまたはリソースの計画に対処するシナリオでは、ユーザーの就業時間にアクセスできると便利です。</span><span class="sxs-lookup"><span data-stu-id="1f83a-105">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="1f83a-106">ユーザーの就業時間は、ユーザーの[メールボックス設定](mailboxsettings.md)の一部として[取得](../api/user-get-mailboxsettings.md#request-3)、[設定](../api/user-update-mailboxsettings.md#request-2)できます。</span><span class="sxs-lookup"><span data-stu-id="1f83a-106">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="1f83a-107">就業時間には、Outlook クライアントに設定したタイム ゾーンとは異なるタイム ゾーンを設定できます。</span><span class="sxs-lookup"><span data-stu-id="1f83a-107">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="1f83a-108">これは、通常の勤務地とは異なるタイム ゾーンに移動する場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1f83a-108">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="1f83a-109">Outlook クライアントを</span><span class="sxs-lookup"><span data-stu-id="1f83a-109">You can set the Outlook client</span></span>  
<span data-ttu-id="1f83a-110">移動先のタイム ゾーンに設定すると、現地にいる間、Outlook の時刻の値を現地時間で表示できます。</span><span class="sxs-lookup"><span data-stu-id="1f83a-110">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="1f83a-111">他のユーザーが通常の勤務地での時間で会議を要求するとしても、該当するタイム ゾーンでの就業時間が考慮されます。</span><span class="sxs-lookup"><span data-stu-id="1f83a-111">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="1f83a-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f83a-112">Properties</span></span>
| <span data-ttu-id="1f83a-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f83a-113">Property</span></span>     | <span data-ttu-id="1f83a-114">型</span><span class="sxs-lookup"><span data-stu-id="1f83a-114">Type</span></span>   |<span data-ttu-id="1f83a-115">説明</span><span class="sxs-lookup"><span data-stu-id="1f83a-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f83a-116">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="1f83a-116">daysOfWeek</span></span> | <span data-ttu-id="1f83a-117">dayOfWeek コレクション</span><span class="sxs-lookup"><span data-stu-id="1f83a-117">dayOfWeek collection</span></span> | <span data-ttu-id="1f83a-118">ユーザーが働く曜日。</span><span class="sxs-lookup"><span data-stu-id="1f83a-118">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="1f83a-119">startTime</span><span class="sxs-lookup"><span data-stu-id="1f83a-119">startTime</span></span> | <span data-ttu-id="1f83a-120">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1f83a-120">Edm.TimeOfDay</span></span> | <span data-ttu-id="1f83a-121">ユーザーの始業時間。</span><span class="sxs-lookup"><span data-stu-id="1f83a-121">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="1f83a-122">endTime</span><span class="sxs-lookup"><span data-stu-id="1f83a-122">endTime</span></span> | <span data-ttu-id="1f83a-123">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1f83a-123">Edm.TimeOfDay</span></span> | <span data-ttu-id="1f83a-124">ユーザーの終業時間。</span><span class="sxs-lookup"><span data-stu-id="1f83a-124">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="1f83a-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="1f83a-125">timeZone</span></span> | [<span data-ttu-id="1f83a-126">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="1f83a-126">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="1f83a-127">就業時間に適用するタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="1f83a-127">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1f83a-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f83a-128">JSON representation</span></span>

<span data-ttu-id="1f83a-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f83a-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "String (timeofday)",
  "endTime": "String (timeofday)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->
