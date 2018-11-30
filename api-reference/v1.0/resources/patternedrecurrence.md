---
title: patternedRecurrence リソースの種類
description: 繰り返しのパターンと範囲です。
ms.openlocfilehash: 10a90db032cd7461e28bc096fd6213df44f3ea45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021214"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="a7754-103">patternedRecurrence リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7754-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="a7754-104">繰り返しのパターンと範囲です。</span><span class="sxs-lookup"><span data-stu-id="a7754-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="a7754-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7754-105">Properties</span></span>
| <span data-ttu-id="a7754-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7754-106">Property</span></span>     | <span data-ttu-id="a7754-107">型</span><span class="sxs-lookup"><span data-stu-id="a7754-107">Type</span></span>   |<span data-ttu-id="a7754-108">説明</span><span class="sxs-lookup"><span data-stu-id="a7754-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7754-109">pattern</span><span class="sxs-lookup"><span data-stu-id="a7754-109">pattern</span></span>|[<span data-ttu-id="a7754-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="a7754-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="a7754-111">イベントの頻度。</span><span class="sxs-lookup"><span data-stu-id="a7754-111">The frequency of an event.</span></span>|
|<span data-ttu-id="a7754-112">range</span><span class="sxs-lookup"><span data-stu-id="a7754-112">range</span></span>|[<span data-ttu-id="a7754-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="a7754-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="a7754-114">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="a7754-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7754-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7754-115">JSON representation</span></span>

<span data-ttu-id="a7754-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a7754-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
