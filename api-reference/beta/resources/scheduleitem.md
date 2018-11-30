---
title: scheduleItem のリソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071872"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="f85a9-104">scheduleItem のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f85a9-104">scheduleItem resource type</span></span>

 > <span data-ttu-id="f85a9-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f85a9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f85a9-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f85a9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f85a9-107">ユーザーの既定の予定表に、実際のイベントに対応するユーザーの可用性を説明する項目です。</span><span class="sxs-lookup"><span data-stu-id="f85a9-107">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="f85a9-108">リソースも同様にこの項目が適用されます。</span><span class="sxs-lookup"><span data-stu-id="f85a9-108">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="f85a9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f85a9-109">Properties</span></span>
| <span data-ttu-id="f85a9-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f85a9-110">Property</span></span>     | <span data-ttu-id="f85a9-111">型</span><span class="sxs-lookup"><span data-stu-id="f85a9-111">Type</span></span>   |<span data-ttu-id="f85a9-112">説明</span><span class="sxs-lookup"><span data-stu-id="f85a9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f85a9-113">end</span><span class="sxs-lookup"><span data-stu-id="f85a9-113">end</span></span> |[<span data-ttu-id="f85a9-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f85a9-114">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="f85a9-115">日付、時刻、およびタイム ゾーンに対応するイベントが終了します。</span><span class="sxs-lookup"><span data-stu-id="f85a9-115">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="f85a9-116">isPrivate</span><span class="sxs-lookup"><span data-stu-id="f85a9-116">isPrivate</span></span> |<span data-ttu-id="f85a9-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="f85a9-117">Boolean</span></span> |<span data-ttu-id="f85a9-118">対応するイベントの重大度。</span><span class="sxs-lookup"><span data-stu-id="f85a9-118">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="f85a9-119">イベントが設定されている場合は true。`private`は false、それ以外の場合。</span><span class="sxs-lookup"><span data-stu-id="f85a9-119">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="f85a9-120">location</span><span class="sxs-lookup"><span data-stu-id="f85a9-120">location</span></span> |<span data-ttu-id="f85a9-121">String</span><span class="sxs-lookup"><span data-stu-id="f85a9-121">String</span></span> | <span data-ttu-id="f85a9-122">場所の対応するイベントが保持されているから参加します。</span><span class="sxs-lookup"><span data-stu-id="f85a9-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="f85a9-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f85a9-123">Optional.</span></span>|
|<span data-ttu-id="f85a9-124">start</span><span class="sxs-lookup"><span data-stu-id="f85a9-124">start</span></span> |[<span data-ttu-id="f85a9-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f85a9-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="f85a9-126">日付、時刻、およびタイム ゾーンに対応するイベントが開始します。</span><span class="sxs-lookup"><span data-stu-id="f85a9-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="f85a9-127">status</span><span class="sxs-lookup"><span data-stu-id="f85a9-127">status</span></span> |<span data-ttu-id="f85a9-128">String</span><span class="sxs-lookup"><span data-stu-id="f85a9-128">String</span></span> | <span data-ttu-id="f85a9-129">ユーザーまたは対応するイベントの中にリソースの可用性の状態です。</span><span class="sxs-lookup"><span data-stu-id="f85a9-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="f85a9-130">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="f85a9-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="f85a9-131">subject</span><span class="sxs-lookup"><span data-stu-id="f85a9-131">subject</span></span> |<span data-ttu-id="f85a9-132">String</span><span class="sxs-lookup"><span data-stu-id="f85a9-132">String</span></span> | <span data-ttu-id="f85a9-133">対応するイベントの件名の行です。</span><span class="sxs-lookup"><span data-stu-id="f85a9-133">The corresponding event's subject line.</span></span> <span data-ttu-id="f85a9-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f85a9-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f85a9-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f85a9-135">JSON representation</span></span>

<span data-ttu-id="f85a9-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f85a9-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->