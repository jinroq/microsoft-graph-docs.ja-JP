---
title: attendeeAvailability リソースの種類
description: 出席者の種類と空き時間情報。
ms.openlocfilehash: ddea2be21f2dd9290637536e2a428e25fc03fcca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066802"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="9e38e-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e38e-103">attendeeAvailability resource type</span></span>

> <span data-ttu-id="9e38e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e38e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e38e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e38e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e38e-106">出席者の種類と空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="9e38e-106">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e38e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e38e-107">JSON representation</span></span>

<span data-ttu-id="9e38e-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9e38e-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9e38e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e38e-109">Properties</span></span>
| <span data-ttu-id="9e38e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e38e-110">Property</span></span>     | <span data-ttu-id="9e38e-111">型</span><span class="sxs-lookup"><span data-stu-id="9e38e-111">Type</span></span>   |<span data-ttu-id="9e38e-112">説明</span><span class="sxs-lookup"><span data-stu-id="9e38e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e38e-113">attendee</span><span class="sxs-lookup"><span data-stu-id="9e38e-113">attendee</span></span>|[<span data-ttu-id="9e38e-114">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="9e38e-114">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="9e38e-115">出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。</span><span class="sxs-lookup"><span data-stu-id="9e38e-115">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="9e38e-116">availability</span><span class="sxs-lookup"><span data-stu-id="9e38e-116">availability</span></span>|<span data-ttu-id="9e38e-117">String</span><span class="sxs-lookup"><span data-stu-id="9e38e-117">String</span></span>| <span data-ttu-id="9e38e-p102">出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9e38e-p102">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->