---
title: patternedRecurrence リソースの種類
description: 繰り返しのパターンと範囲です。
localization_priority: Normal
ms.openlocfilehash: 063df70dfeeb1d37cfc5e23710108dd4cfc9ae57
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344934"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="e9f7b-103">patternedRecurrence リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9f7b-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f7b-104">繰り返しのパターンと範囲です。</span><span class="sxs-lookup"><span data-stu-id="e9f7b-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="e9f7b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9f7b-105">Properties</span></span>
| <span data-ttu-id="e9f7b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9f7b-106">Property</span></span>     | <span data-ttu-id="e9f7b-107">型</span><span class="sxs-lookup"><span data-stu-id="e9f7b-107">Type</span></span>   |<span data-ttu-id="e9f7b-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9f7b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9f7b-109">pattern</span><span class="sxs-lookup"><span data-stu-id="e9f7b-109">pattern</span></span>|[<span data-ttu-id="e9f7b-110">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="e9f7b-110">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="e9f7b-111">イベントの頻度。</span><span class="sxs-lookup"><span data-stu-id="e9f7b-111">The frequency of an event.</span></span>|
|<span data-ttu-id="e9f7b-112">range</span><span class="sxs-lookup"><span data-stu-id="e9f7b-112">range</span></span>|[<span data-ttu-id="e9f7b-113">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="e9f7b-113">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="e9f7b-114">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="e9f7b-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9f7b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9f7b-115">JSON representation</span></span>

<span data-ttu-id="e9f7b-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e9f7b-116">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
