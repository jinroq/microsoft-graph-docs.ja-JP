---
title: timeoffitem リソースの種類
description: timeoff のバージョンを表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3b5b819b9179d266064d7ddf0f6636b9027591af
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345503"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="31965-103">timeoffitem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31965-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31965-104">[timeoff](timeoff.md)のバージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="31965-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="31965-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31965-105">Properties</span></span>
| <span data-ttu-id="31965-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31965-106">Property</span></span>                         | <span data-ttu-id="31965-107">型</span><span class="sxs-lookup"><span data-stu-id="31965-107">Type</span></span>                    | <span data-ttu-id="31965-108">説明</span><span class="sxs-lookup"><span data-stu-id="31965-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="31965-109">timeoff理由 id</span><span class="sxs-lookup"><span data-stu-id="31965-109">timeOffReasonId</span></span>               | <span data-ttu-id="31965-110">string</span><span class="sxs-lookup"><span data-stu-id="31965-110">string</span></span>                  | <span data-ttu-id="31965-111">`timeOffReason`のの ID `timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="31965-111">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="31965-112">必須です。</span><span class="sxs-lookup"><span data-stu-id="31965-112">Required.</span></span>     |
| <span data-ttu-id="31965-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31965-113">startDateTime</span></span>               | <span data-ttu-id="31965-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31965-114">DateTimeOffset</span></span>                  | <span data-ttu-id="31965-115">の開始日時`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="31965-115">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="31965-116">必須です。</span><span class="sxs-lookup"><span data-stu-id="31965-116">Required.</span></span> <span data-ttu-id="31965-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="31965-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31965-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="31965-118">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="31965-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="31965-119">endDateTime</span></span>               | <span data-ttu-id="31965-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31965-120">DateTimeOffset</span></span>                  | <span data-ttu-id="31965-121">の終了日時`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="31965-121">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="31965-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="31965-122">Required.</span></span> <span data-ttu-id="31965-123">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="31965-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31965-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="31965-124">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="31965-125">theme</span><span class="sxs-lookup"><span data-stu-id="31965-125">theme</span></span> | <span data-ttu-id="31965-126">scheduleentitytheme</span><span class="sxs-lookup"><span data-stu-id="31965-126">scheduleEntityTheme</span></span>   | <span data-ttu-id="31965-127">サポートされている色: 白。水色緑青紫色ピンクイエロー灰色darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="31965-127">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31965-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31965-128">JSON representation</span></span>

<span data-ttu-id="31965-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31965-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
