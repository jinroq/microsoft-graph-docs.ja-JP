---
title: attendeeAvailability リソースの種類
description: 出席者の種類と空き時間情報。
localization_priority: Normal
ms.openlocfilehash: a00fe38e678c6a51cd252b823a7d2651e531d20a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820469"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="75e65-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75e65-103">attendeeAvailability resource type</span></span>

> <span data-ttu-id="75e65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75e65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75e65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75e65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75e65-106">出席者の種類と空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="75e65-106">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75e65-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75e65-107">JSON representation</span></span>

<span data-ttu-id="75e65-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="75e65-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="75e65-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75e65-109">Properties</span></span>
| <span data-ttu-id="75e65-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75e65-110">Property</span></span>     | <span data-ttu-id="75e65-111">種類</span><span class="sxs-lookup"><span data-stu-id="75e65-111">Type</span></span>   |<span data-ttu-id="75e65-112">説明</span><span class="sxs-lookup"><span data-stu-id="75e65-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75e65-113">attendee</span><span class="sxs-lookup"><span data-stu-id="75e65-113">attendee</span></span>|[<span data-ttu-id="75e65-114">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="75e65-114">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="75e65-115">出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。</span><span class="sxs-lookup"><span data-stu-id="75e65-115">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="75e65-116">availability</span><span class="sxs-lookup"><span data-stu-id="75e65-116">availability</span></span>|<span data-ttu-id="75e65-117">String</span><span class="sxs-lookup"><span data-stu-id="75e65-117">String</span></span>| <span data-ttu-id="75e65-p102">出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="75e65-p102">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
