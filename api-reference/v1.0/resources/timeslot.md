---
title: timeSlot リソースの種類
description: 期間です。
ms.openlocfilehash: 43ce20e006f2a6946877a4ffd2bf730d45d6d1c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022220"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="63f75-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63f75-103">timeSlot resource type</span></span>

<span data-ttu-id="63f75-104">期間です。</span><span class="sxs-lookup"><span data-stu-id="63f75-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63f75-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63f75-105">JSON representation</span></span>

<span data-ttu-id="63f75-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="63f75-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="63f75-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63f75-107">Properties</span></span>
| <span data-ttu-id="63f75-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63f75-108">Property</span></span>     | <span data-ttu-id="63f75-109">型</span><span class="sxs-lookup"><span data-stu-id="63f75-109">Type</span></span>   |<span data-ttu-id="63f75-110">説明</span><span class="sxs-lookup"><span data-stu-id="63f75-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f75-111">end</span><span class="sxs-lookup"><span data-stu-id="63f75-111">end</span></span>|[<span data-ttu-id="63f75-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="63f75-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="63f75-113">期間の開始時間。</span><span class="sxs-lookup"><span data-stu-id="63f75-113">The time a period begins.</span></span>|
|<span data-ttu-id="63f75-114">start</span><span class="sxs-lookup"><span data-stu-id="63f75-114">start</span></span>|[<span data-ttu-id="63f75-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="63f75-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="63f75-116">期間の終了時間。</span><span class="sxs-lookup"><span data-stu-id="63f75-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->