---
title: timeSlot リソースの種類
description: 期間です。
ms.openlocfilehash: c1df6ea458bf6742dc20149e62d9760a8a6510e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073139"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="fa6da-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa6da-103">timeSlot resource type</span></span>

> <span data-ttu-id="fa6da-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa6da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa6da-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa6da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa6da-106">期間です。</span><span class="sxs-lookup"><span data-stu-id="fa6da-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa6da-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa6da-107">JSON representation</span></span>

<span data-ttu-id="fa6da-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fa6da-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fa6da-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa6da-109">Properties</span></span>
| <span data-ttu-id="fa6da-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa6da-110">Property</span></span>     | <span data-ttu-id="fa6da-111">型</span><span class="sxs-lookup"><span data-stu-id="fa6da-111">Type</span></span>   |<span data-ttu-id="fa6da-112">説明</span><span class="sxs-lookup"><span data-stu-id="fa6da-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa6da-113">end</span><span class="sxs-lookup"><span data-stu-id="fa6da-113">end</span></span>|[<span data-ttu-id="fa6da-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fa6da-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="fa6da-115">期間の開始時間。</span><span class="sxs-lookup"><span data-stu-id="fa6da-115">The time a period begins.</span></span>|
|<span data-ttu-id="fa6da-116">start</span><span class="sxs-lookup"><span data-stu-id="fa6da-116">start</span></span>|[<span data-ttu-id="fa6da-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fa6da-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="fa6da-118">期間の終了時間。</span><span class="sxs-lookup"><span data-stu-id="fa6da-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->