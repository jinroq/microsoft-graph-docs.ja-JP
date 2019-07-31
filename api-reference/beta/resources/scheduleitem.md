---
title: scheduleItem リソースの種類
description: ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソースにも適用されます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008643"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="e8f5b-104">scheduleItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8f5b-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e8f5b-105">ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="e8f5b-106">この項目は、リソース (会議室または備品) にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="e8f5b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8f5b-107">Properties</span></span>
| <span data-ttu-id="e8f5b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8f5b-108">Property</span></span>     | <span data-ttu-id="e8f5b-109">型</span><span class="sxs-lookup"><span data-stu-id="e8f5b-109">Type</span></span>   |<span data-ttu-id="e8f5b-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8f5b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8f5b-111">end</span><span class="sxs-lookup"><span data-stu-id="e8f5b-111">end</span></span> |[<span data-ttu-id="e8f5b-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e8f5b-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="e8f5b-113">対応するイベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="e8f5b-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="e8f5b-114">isPrivate</span></span> |<span data-ttu-id="e8f5b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8f5b-115">Boolean</span></span> |<span data-ttu-id="e8f5b-116">対応するイベントの感度。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="e8f5b-117">イベントがマーク`private`されている場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="e8f5b-118">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-118">Optional.</span></span> |
|<span data-ttu-id="e8f5b-119">location</span><span class="sxs-lookup"><span data-stu-id="e8f5b-119">location</span></span> |<span data-ttu-id="e8f5b-120">String</span><span class="sxs-lookup"><span data-stu-id="e8f5b-120">String</span></span> | <span data-ttu-id="e8f5b-121">対応するイベントが保持または参加している場所。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="e8f5b-122">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-122">Optional.</span></span>|
|<span data-ttu-id="e8f5b-123">開始</span><span class="sxs-lookup"><span data-stu-id="e8f5b-123">start</span></span> |[<span data-ttu-id="e8f5b-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e8f5b-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="e8f5b-125">対応するイベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="e8f5b-126">status</span><span class="sxs-lookup"><span data-stu-id="e8f5b-126">status</span></span> |<span data-ttu-id="e8f5b-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="e8f5b-127">freeBusyStatus</span></span> | <span data-ttu-id="e8f5b-128">対応するイベント中のユーザーまたはリソースの空き時間状態。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="e8f5b-129">使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="e8f5b-130">subject</span><span class="sxs-lookup"><span data-stu-id="e8f5b-130">subject</span></span> |<span data-ttu-id="e8f5b-131">String</span><span class="sxs-lookup"><span data-stu-id="e8f5b-131">String</span></span> | <span data-ttu-id="e8f5b-132">対応するイベントの件名行。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-132">The corresponding event's subject line.</span></span> <span data-ttu-id="e8f5b-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e8f5b-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8f5b-134">JSON representation</span></span>

<span data-ttu-id="e8f5b-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8f5b-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
