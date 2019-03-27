---
title: scheduleitem リソースの種類
description: ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソースにも適用されます。
localization_priority: Normal
ms.openlocfilehash: a39f45598ab3c427a741659aa93615317c3c57a7
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869310"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="5415a-104">scheduleitem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5415a-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="5415a-105">ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。</span><span class="sxs-lookup"><span data-stu-id="5415a-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="5415a-106">この項目は、リソース (会議室または備品) にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="5415a-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="5415a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5415a-107">Properties</span></span>
| <span data-ttu-id="5415a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5415a-108">Property</span></span>     | <span data-ttu-id="5415a-109">型</span><span class="sxs-lookup"><span data-stu-id="5415a-109">Type</span></span>   |<span data-ttu-id="5415a-110">説明</span><span class="sxs-lookup"><span data-stu-id="5415a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5415a-111">end</span><span class="sxs-lookup"><span data-stu-id="5415a-111">end</span></span> |[<span data-ttu-id="5415a-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5415a-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="5415a-113">対応するイベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="5415a-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="5415a-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="5415a-114">isPrivate</span></span> |<span data-ttu-id="5415a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5415a-115">Boolean</span></span> |<span data-ttu-id="5415a-116">対応するイベントの感度。</span><span class="sxs-lookup"><span data-stu-id="5415a-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="5415a-117">イベントがマーク`private`されている場合は True、それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="5415a-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="5415a-118">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5415a-118">Optional.</span></span> |
|<span data-ttu-id="5415a-119">location</span><span class="sxs-lookup"><span data-stu-id="5415a-119">location</span></span> |<span data-ttu-id="5415a-120">String</span><span class="sxs-lookup"><span data-stu-id="5415a-120">String</span></span> | <span data-ttu-id="5415a-121">対応するイベントが保持または参加している場所。</span><span class="sxs-lookup"><span data-stu-id="5415a-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="5415a-122">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5415a-122">Optional.</span></span>|
|<span data-ttu-id="5415a-123">start</span><span class="sxs-lookup"><span data-stu-id="5415a-123">start</span></span> |[<span data-ttu-id="5415a-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5415a-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="5415a-125">対応するイベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="5415a-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="5415a-126">status</span><span class="sxs-lookup"><span data-stu-id="5415a-126">status</span></span> |<span data-ttu-id="5415a-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5415a-127">freeBusyStatus</span></span> | <span data-ttu-id="5415a-128">対応するイベント中のユーザーまたはリソースの空き時間状態。</span><span class="sxs-lookup"><span data-stu-id="5415a-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="5415a-129">使用可能な値は`free`、 `tentative`、 `busy` `oof` `workingElsewhere`、、、 `unknown`、です。</span><span class="sxs-lookup"><span data-stu-id="5415a-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="5415a-130">subject</span><span class="sxs-lookup"><span data-stu-id="5415a-130">subject</span></span> |<span data-ttu-id="5415a-131">String</span><span class="sxs-lookup"><span data-stu-id="5415a-131">String</span></span> | <span data-ttu-id="5415a-132">対応するイベントの件名行。</span><span class="sxs-lookup"><span data-stu-id="5415a-132">The corresponding event's subject line.</span></span> <span data-ttu-id="5415a-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5415a-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5415a-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5415a-134">JSON representation</span></span>

<span data-ttu-id="5415a-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5415a-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
