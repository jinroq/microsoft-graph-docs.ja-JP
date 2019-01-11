---
title: scheduleInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: e535f5c2b47e810fc767cb29d0b24f28ed3c7bf0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828708"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="ed41a-104">scheduleInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ed41a-104">scheduleInformation resource type</span></span>

 > <span data-ttu-id="ed41a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed41a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed41a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed41a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ed41a-107">指定された期間内のユーザー、配布リスト、またはリソースの可用性を表します。</span><span class="sxs-lookup"><span data-stu-id="ed41a-107">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="ed41a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed41a-108">Properties</span></span>
| <span data-ttu-id="ed41a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed41a-109">Property</span></span>     | <span data-ttu-id="ed41a-110">種類</span><span class="sxs-lookup"><span data-stu-id="ed41a-110">Type</span></span>   |<span data-ttu-id="ed41a-111">説明</span><span class="sxs-lookup"><span data-stu-id="ed41a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed41a-112">availabilityView</span><span class="sxs-lookup"><span data-stu-id="ed41a-112">availabilityView</span></span> |<span data-ttu-id="ed41a-113">String</span><span class="sxs-lookup"><span data-stu-id="ed41a-113">String</span></span> |<span data-ttu-id="ed41a-114">マージされたビュー内のすべての項目の数を表す`scheduleItems`。</span><span class="sxs-lookup"><span data-stu-id="ed41a-114">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="ed41a-115">ビューは、時間帯で構成されています。</span><span class="sxs-lookup"><span data-stu-id="ed41a-115">The view consists of time slots.</span></span> <span data-ttu-id="ed41a-116">各時間帯の可用性で示されます。:`0`無料 = `1`= 仮の予定、 `2`= ビジー状態か、`3`外出中 = `4`= の別の場所で作業します。</span><span class="sxs-lookup"><span data-stu-id="ed41a-116">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="ed41a-117">エラー</span><span class="sxs-lookup"><span data-stu-id="ed41a-117">error</span></span> |[<span data-ttu-id="ed41a-118">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="ed41a-118">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="ed41a-119">エラー情報が、ユーザー、配布リスト、またはリソースの可用性を取得しようとしていますから。</span><span class="sxs-lookup"><span data-stu-id="ed41a-119">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="ed41a-120">scheduleId</span><span class="sxs-lookup"><span data-stu-id="ed41a-120">scheduleId</span></span> |<span data-ttu-id="ed41a-121">String</span><span class="sxs-lookup"><span data-stu-id="ed41a-121">String</span></span> |<span data-ttu-id="ed41a-122">ユーザー、配布リスト、または**scheduleInformation**のインスタンスを識別する、リソースの SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="ed41a-122">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="ed41a-123">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="ed41a-123">scheduleItems</span></span> |<span data-ttu-id="ed41a-124">[scheduleItem](scheduleitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ed41a-124">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="ed41a-125">ユーザーまたはリソースの可用性を説明する項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed41a-125">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="ed41a-126">workingHours</span><span class="sxs-lookup"><span data-stu-id="ed41a-126">workingHours</span></span> |[<span data-ttu-id="ed41a-127">workingHours</span><span class="sxs-lookup"><span data-stu-id="ed41a-127">workingHours</span></span>](workinghours.md) |<span data-ttu-id="ed41a-128">ユーザーが働く曜日と、特定のタイムゾーンの時間。</span><span class="sxs-lookup"><span data-stu-id="ed41a-128">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="ed41a-129">これらは、ユーザーの[mailboxSettings](mailboxsettings.md)の一部として設定されています。</span><span class="sxs-lookup"><span data-stu-id="ed41a-129">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ed41a-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ed41a-130">JSON representation</span></span>

<span data-ttu-id="ed41a-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ed41a-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
