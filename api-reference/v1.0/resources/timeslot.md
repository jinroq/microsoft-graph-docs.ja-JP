---
title: timeSlot リソースの種類
description: 期間です。
localization_priority: Normal
ms.openlocfilehash: e01b8d0f34a21eb18bc92e8bcc4e1b8365541d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860565"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="29327-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29327-103">timeSlot resource type</span></span>

<span data-ttu-id="29327-104">期間です。</span><span class="sxs-lookup"><span data-stu-id="29327-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29327-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29327-105">JSON representation</span></span>

<span data-ttu-id="29327-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="29327-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="29327-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29327-107">Properties</span></span>
| <span data-ttu-id="29327-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29327-108">Property</span></span>     | <span data-ttu-id="29327-109">種類</span><span class="sxs-lookup"><span data-stu-id="29327-109">Type</span></span>   |<span data-ttu-id="29327-110">説明</span><span class="sxs-lookup"><span data-stu-id="29327-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29327-111">end</span><span class="sxs-lookup"><span data-stu-id="29327-111">end</span></span>|[<span data-ttu-id="29327-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="29327-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="29327-113">期間の開始時間。</span><span class="sxs-lookup"><span data-stu-id="29327-113">The time a period begins.</span></span>|
|<span data-ttu-id="29327-114">start</span><span class="sxs-lookup"><span data-stu-id="29327-114">start</span></span>|[<span data-ttu-id="29327-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="29327-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="29327-116">期間の終了時間。</span><span class="sxs-lookup"><span data-stu-id="29327-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
