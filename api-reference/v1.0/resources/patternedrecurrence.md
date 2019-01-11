---
title: patternedRecurrence リソースの種類
description: 繰り返しのパターンと範囲です。
localization_priority: Normal
ms.openlocfilehash: 8a9581150e3b7790f32268eb34f35b22abcb3642
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840797"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="86a74-103">patternedRecurrence リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86a74-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="86a74-104">繰り返しのパターンと範囲です。</span><span class="sxs-lookup"><span data-stu-id="86a74-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="86a74-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86a74-105">Properties</span></span>
| <span data-ttu-id="86a74-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86a74-106">Property</span></span>     | <span data-ttu-id="86a74-107">種類</span><span class="sxs-lookup"><span data-stu-id="86a74-107">Type</span></span>   |<span data-ttu-id="86a74-108">説明</span><span class="sxs-lookup"><span data-stu-id="86a74-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86a74-109">pattern</span><span class="sxs-lookup"><span data-stu-id="86a74-109">pattern</span></span>|[<span data-ttu-id="86a74-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="86a74-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="86a74-111">イベントの頻度。</span><span class="sxs-lookup"><span data-stu-id="86a74-111">The frequency of an event.</span></span>|
|<span data-ttu-id="86a74-112">range</span><span class="sxs-lookup"><span data-stu-id="86a74-112">range</span></span>|[<span data-ttu-id="86a74-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="86a74-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="86a74-114">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="86a74-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86a74-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86a74-115">JSON representation</span></span>

<span data-ttu-id="86a74-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="86a74-116">Here is a JSON representation of the resource</span></span>

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
