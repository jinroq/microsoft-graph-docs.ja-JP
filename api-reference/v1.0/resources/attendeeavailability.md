---
title: attendeeAvailability リソースの種類
description: 出席者の種類と空き時間情報。
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021033"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="876e5-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="876e5-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="876e5-104">出席者の種類と空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="876e5-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="876e5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="876e5-105">JSON representation</span></span>

<span data-ttu-id="876e5-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="876e5-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="876e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="876e5-107">Properties</span></span>
| <span data-ttu-id="876e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="876e5-108">Property</span></span>     | <span data-ttu-id="876e5-109">型</span><span class="sxs-lookup"><span data-stu-id="876e5-109">Type</span></span>   |<span data-ttu-id="876e5-110">説明</span><span class="sxs-lookup"><span data-stu-id="876e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="876e5-111">attendee</span><span class="sxs-lookup"><span data-stu-id="876e5-111">attendee</span></span>|[<span data-ttu-id="876e5-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="876e5-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="876e5-113">出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。</span><span class="sxs-lookup"><span data-stu-id="876e5-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="876e5-114">availability</span><span class="sxs-lookup"><span data-stu-id="876e5-114">availability</span></span>|<span data-ttu-id="876e5-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="876e5-115">freeBusyStatus</span></span>| <span data-ttu-id="876e5-116">出席者の空き時間の状態。</span><span class="sxs-lookup"><span data-stu-id="876e5-116">The availability status of the attendee.</span></span> <span data-ttu-id="876e5-117">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="876e5-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
