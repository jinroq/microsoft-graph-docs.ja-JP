---
title: scheduleItem リソースの種類
description: ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソース (会議室または備品) にも適用されます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fb544041948d5e46c1ae8c3f6f887f595ddb82e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034634"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="1067d-104">scheduleItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1067d-104">scheduleItem resource type</span></span>

<span data-ttu-id="1067d-105">ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。</span><span class="sxs-lookup"><span data-stu-id="1067d-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="1067d-106">この項目は、リソース (会議室または備品) にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="1067d-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="1067d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1067d-107">Properties</span></span>
| <span data-ttu-id="1067d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1067d-108">Property</span></span>     | <span data-ttu-id="1067d-109">型</span><span class="sxs-lookup"><span data-stu-id="1067d-109">Type</span></span>   |<span data-ttu-id="1067d-110">説明</span><span class="sxs-lookup"><span data-stu-id="1067d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1067d-111">end</span><span class="sxs-lookup"><span data-stu-id="1067d-111">end</span></span> |[<span data-ttu-id="1067d-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1067d-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="1067d-113">対応するイベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1067d-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="1067d-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="1067d-114">isPrivate</span></span> |<span data-ttu-id="1067d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="1067d-115">Boolean</span></span> |<span data-ttu-id="1067d-116">対応するイベントの感度。</span><span class="sxs-lookup"><span data-stu-id="1067d-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="1067d-117">イベントがマーク`private`されている場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="1067d-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="1067d-118">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1067d-118">Optional.</span></span>|
|<span data-ttu-id="1067d-119">location</span><span class="sxs-lookup"><span data-stu-id="1067d-119">location</span></span> |<span data-ttu-id="1067d-120">String</span><span class="sxs-lookup"><span data-stu-id="1067d-120">String</span></span> | <span data-ttu-id="1067d-121">対応するイベントが保持または参加している場所。</span><span class="sxs-lookup"><span data-stu-id="1067d-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="1067d-122">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1067d-122">Optional.</span></span>|
|<span data-ttu-id="1067d-123">開始</span><span class="sxs-lookup"><span data-stu-id="1067d-123">start</span></span> |[<span data-ttu-id="1067d-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1067d-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="1067d-125">対応するイベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="1067d-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="1067d-126">status</span><span class="sxs-lookup"><span data-stu-id="1067d-126">status</span></span> |<span data-ttu-id="1067d-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="1067d-127">freeBusyStatus</span></span> | <span data-ttu-id="1067d-128">対応するイベント中のユーザーまたはリソースの空き時間状態。</span><span class="sxs-lookup"><span data-stu-id="1067d-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="1067d-129">使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="1067d-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="1067d-130">subject</span><span class="sxs-lookup"><span data-stu-id="1067d-130">subject</span></span> |<span data-ttu-id="1067d-131">String</span><span class="sxs-lookup"><span data-stu-id="1067d-131">String</span></span> | <span data-ttu-id="1067d-132">対応するイベントの件名行。</span><span class="sxs-lookup"><span data-stu-id="1067d-132">The corresponding event's subject line.</span></span> <span data-ttu-id="1067d-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1067d-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1067d-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1067d-134">JSON representation</span></span>

<span data-ttu-id="1067d-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1067d-135">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": ""
}
-->
