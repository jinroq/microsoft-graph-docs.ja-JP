---
title: "\"佐々木 ftitem\" リソースの種類"
description: "\"佐々木 ftitem\" は、シフトのバージョンを表します。"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd5b3d224e60fc3f21b4d484952c7a2643b02407
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343039"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="b6254-103">"佐々木 ftitem" リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6254-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6254-104">[シフト](shift.md)のバージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="b6254-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b6254-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6254-105">Properties</span></span>
| <span data-ttu-id="b6254-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6254-106">Property</span></span>                         | <span data-ttu-id="b6254-107">型</span><span class="sxs-lookup"><span data-stu-id="b6254-107">Type</span></span>                    | <span data-ttu-id="b6254-108">説明</span><span class="sxs-lookup"><span data-stu-id="b6254-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="b6254-109">notes</span><span class="sxs-lookup"><span data-stu-id="b6254-109">notes</span></span>               | <span data-ttu-id="b6254-110">string</span><span class="sxs-lookup"><span data-stu-id="b6254-110">string</span></span>                  | <span data-ttu-id="b6254-111">のメモ`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="b6254-111">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="b6254-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b6254-112">displayName</span></span>               | <span data-ttu-id="b6254-113">string</span><span class="sxs-lookup"><span data-stu-id="b6254-113">string</span></span>                  | <span data-ttu-id="b6254-114">の名前`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="b6254-114">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="b6254-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b6254-115">startDateTime</span></span>               | <span data-ttu-id="b6254-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6254-116">DateTimeOffset</span></span>                  | <span data-ttu-id="b6254-117">の開始日時`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="b6254-117">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="b6254-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="b6254-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6254-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="b6254-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b6254-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="b6254-120">Required.</span></span> |
| <span data-ttu-id="b6254-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b6254-121">endDateTime</span></span>               | <span data-ttu-id="b6254-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6254-122">DateTimeOffset</span></span>                 | <span data-ttu-id="b6254-123">の終了日時`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="b6254-123">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="b6254-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="b6254-124">Required.</span></span> <span data-ttu-id="b6254-125">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="b6254-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6254-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="b6254-126">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b6254-127">theme</span><span class="sxs-lookup"><span data-stu-id="b6254-127">theme</span></span> | <span data-ttu-id="b6254-128">scheduleentitytheme</span><span class="sxs-lookup"><span data-stu-id="b6254-128">scheduleEntityTheme</span></span>   |  <span data-ttu-id="b6254-129">サポートされている色: 白。水色緑青紫色ピンクイエロー灰色darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="b6254-129">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="b6254-130">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="b6254-130">activities</span></span>    | <span data-ttu-id="b6254-131">[shiftActivity](shiftactivity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6254-131">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="b6254-132">従業員がいつ、どのような時間帯に勤務しているかを詳細に説明できる、シフトの増分部分。</span><span class="sxs-lookup"><span data-stu-id="b6254-132">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="b6254-133">たとえば、割り当て、またはスケジュールされた休憩またはランチ。</span><span class="sxs-lookup"><span data-stu-id="b6254-133">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="b6254-134">必須。</span><span class="sxs-lookup"><span data-stu-id="b6254-134">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6254-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6254-135">JSON representation</span></span>

<span data-ttu-id="b6254-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b6254-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
