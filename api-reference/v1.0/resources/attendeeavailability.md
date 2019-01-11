---
title: attendeeAvailability リソースの種類
description: 出席者の種類と空き時間情報。
localization_priority: Normal
ms.openlocfilehash: a6dee994fc5eb3786fc1a432adcb9333bdb56ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834749"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="8c76e-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c76e-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="8c76e-104">出席者の種類と空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="8c76e-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c76e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c76e-105">JSON representation</span></span>

<span data-ttu-id="8c76e-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8c76e-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="8c76e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c76e-107">Properties</span></span>
| <span data-ttu-id="8c76e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c76e-108">Property</span></span>     | <span data-ttu-id="8c76e-109">種類</span><span class="sxs-lookup"><span data-stu-id="8c76e-109">Type</span></span>   |<span data-ttu-id="8c76e-110">説明</span><span class="sxs-lookup"><span data-stu-id="8c76e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c76e-111">attendee</span><span class="sxs-lookup"><span data-stu-id="8c76e-111">attendee</span></span>|[<span data-ttu-id="8c76e-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="8c76e-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="8c76e-113">出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。</span><span class="sxs-lookup"><span data-stu-id="8c76e-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="8c76e-114">availability</span><span class="sxs-lookup"><span data-stu-id="8c76e-114">availability</span></span>|<span data-ttu-id="8c76e-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="8c76e-115">freeBusyStatus</span></span>| <span data-ttu-id="8c76e-116">出席者の空き時間の状態。</span><span class="sxs-lookup"><span data-stu-id="8c76e-116">The availability status of the attendee.</span></span> <span data-ttu-id="8c76e-117">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="8c76e-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
