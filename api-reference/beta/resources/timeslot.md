---
title: timeSlot リソースの種類
description: 期間です。
localization_priority: Normal
ms.openlocfilehash: 1f383a7feafbb3816ef838d8f0667eebdd42443f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877932"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="48b8d-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48b8d-103">timeSlot resource type</span></span>

> <span data-ttu-id="48b8d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="48b8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48b8d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48b8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48b8d-106">期間です。</span><span class="sxs-lookup"><span data-stu-id="48b8d-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48b8d-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48b8d-107">JSON representation</span></span>

<span data-ttu-id="48b8d-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="48b8d-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="48b8d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48b8d-109">Properties</span></span>
| <span data-ttu-id="48b8d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48b8d-110">Property</span></span>     | <span data-ttu-id="48b8d-111">種類</span><span class="sxs-lookup"><span data-stu-id="48b8d-111">Type</span></span>   |<span data-ttu-id="48b8d-112">説明</span><span class="sxs-lookup"><span data-stu-id="48b8d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48b8d-113">end</span><span class="sxs-lookup"><span data-stu-id="48b8d-113">end</span></span>|[<span data-ttu-id="48b8d-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="48b8d-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="48b8d-115">期間の開始時間。</span><span class="sxs-lookup"><span data-stu-id="48b8d-115">The time a period begins.</span></span>|
|<span data-ttu-id="48b8d-116">start</span><span class="sxs-lookup"><span data-stu-id="48b8d-116">start</span></span>|[<span data-ttu-id="48b8d-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="48b8d-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="48b8d-118">期間の終了時間。</span><span class="sxs-lookup"><span data-stu-id="48b8d-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
