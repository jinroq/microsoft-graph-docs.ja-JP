---
title: workingHours リソースの種類
description: ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。
ms.openlocfilehash: 915ec185931d3f7e77f010517a3ef0c3bff92204
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071906"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="b4def-103">workingHours リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4def-103">workingHours resource type</span></span>

> <span data-ttu-id="b4def-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4def-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4def-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4def-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4def-106">ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。</span><span class="sxs-lookup"><span data-stu-id="b4def-106">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="b4def-107">アクティビティまたはリソースの計画に対処するシナリオでは、ユーザーの就業時間にアクセスできると便利です。</span><span class="sxs-lookup"><span data-stu-id="b4def-107">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="b4def-108">ユーザーの就業時間は、ユーザーの[メールボックス設定](mailboxsettings.md)の一部として[取得](../api/user-get-mailboxsettings.md#request-3)、[設定](../api/user-update-mailboxsettings.md#request-2)できます。</span><span class="sxs-lookup"><span data-stu-id="b4def-108">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="b4def-109">就業時間には、Outlook クライアントに設定したタイム ゾーンとは異なるタイム ゾーンを設定できます。</span><span class="sxs-lookup"><span data-stu-id="b4def-109">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="b4def-110">これは、通常の勤務地とは異なるタイム ゾーンに移動する場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b4def-110">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="b4def-111">Outlook クライアントを</span><span class="sxs-lookup"><span data-stu-id="b4def-111">You can set the Outlook client</span></span>  
<span data-ttu-id="b4def-112">移動先のタイム ゾーンに設定すると、現地にいる間、Outlook の時刻の値を現地時間で表示できます。</span><span class="sxs-lookup"><span data-stu-id="b4def-112">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="b4def-113">他のユーザーが通常の勤務地での時間で会議を要求するとしても、該当するタイム ゾーンでの就業時間が考慮されます。</span><span class="sxs-lookup"><span data-stu-id="b4def-113">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="b4def-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4def-114">Properties</span></span>
| <span data-ttu-id="b4def-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4def-115">Property</span></span>     | <span data-ttu-id="b4def-116">型</span><span class="sxs-lookup"><span data-stu-id="b4def-116">Type</span></span>   |<span data-ttu-id="b4def-117">説明</span><span class="sxs-lookup"><span data-stu-id="b4def-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4def-118">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="b4def-118">daysOfWeek</span></span> | <span data-ttu-id="b4def-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b4def-119">String collection</span></span> | <span data-ttu-id="b4def-120">ユーザーが働く曜日。</span><span class="sxs-lookup"><span data-stu-id="b4def-120">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="b4def-121">startTime</span><span class="sxs-lookup"><span data-stu-id="b4def-121">startTime</span></span> | <span data-ttu-id="b4def-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b4def-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="b4def-123">ユーザーの始業時間。</span><span class="sxs-lookup"><span data-stu-id="b4def-123">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="b4def-124">endTime</span><span class="sxs-lookup"><span data-stu-id="b4def-124">endTime</span></span> | <span data-ttu-id="b4def-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b4def-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="b4def-126">ユーザーの終業時間。</span><span class="sxs-lookup"><span data-stu-id="b4def-126">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="b4def-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="b4def-127">timeZone</span></span> | [<span data-ttu-id="b4def-128">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="b4def-128">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="b4def-129">就業時間に適用するタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="b4def-129">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b4def-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4def-130">JSON representation</span></span>

<span data-ttu-id="b4def-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4def-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
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
  "tocPath": ""
}-->