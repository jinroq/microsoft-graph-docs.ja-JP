---
title: attendeeAvailability リソースの種類
description: 出席者の種類と空き時間情報。
localization_priority: Normal
ms.openlocfilehash: f831a88a14fc6ec970332208389e15a5adc49377
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508938"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="4edff-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4edff-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4edff-104">出席者の種類と空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="4edff-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4edff-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4edff-105">JSON representation</span></span>

<span data-ttu-id="4edff-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4edff-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4edff-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4edff-107">Properties</span></span>
| <span data-ttu-id="4edff-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4edff-108">Property</span></span>     | <span data-ttu-id="4edff-109">型</span><span class="sxs-lookup"><span data-stu-id="4edff-109">Type</span></span>   |<span data-ttu-id="4edff-110">説明</span><span class="sxs-lookup"><span data-stu-id="4edff-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4edff-111">attendee</span><span class="sxs-lookup"><span data-stu-id="4edff-111">attendee</span></span>|[<span data-ttu-id="4edff-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="4edff-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="4edff-113">出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。</span><span class="sxs-lookup"><span data-stu-id="4edff-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="4edff-114">availability</span><span class="sxs-lookup"><span data-stu-id="4edff-114">availability</span></span>|<span data-ttu-id="4edff-115">String</span><span class="sxs-lookup"><span data-stu-id="4edff-115">String</span></span>| <span data-ttu-id="4edff-p101">出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="4edff-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
