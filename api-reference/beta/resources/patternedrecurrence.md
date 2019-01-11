---
title: patternedRecurrence リソースの種類
description: 繰り返しのパターンと範囲です。
localization_priority: Normal
ms.openlocfilehash: 2c2d68046c69ed702738318121a0289eb6a347a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825245"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="46e61-103">patternedRecurrence リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46e61-103">patternedRecurrence resource type</span></span>

> <span data-ttu-id="46e61-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46e61-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46e61-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46e61-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46e61-106">繰り返しのパターンと範囲です。</span><span class="sxs-lookup"><span data-stu-id="46e61-106">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="46e61-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46e61-107">Properties</span></span>
| <span data-ttu-id="46e61-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46e61-108">Property</span></span>     | <span data-ttu-id="46e61-109">種類</span><span class="sxs-lookup"><span data-stu-id="46e61-109">Type</span></span>   |<span data-ttu-id="46e61-110">説明</span><span class="sxs-lookup"><span data-stu-id="46e61-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46e61-111">pattern</span><span class="sxs-lookup"><span data-stu-id="46e61-111">pattern</span></span>|[<span data-ttu-id="46e61-112">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="46e61-112">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="46e61-113">イベントの頻度。</span><span class="sxs-lookup"><span data-stu-id="46e61-113">The frequency of an event.</span></span>|
|<span data-ttu-id="46e61-114">range</span><span class="sxs-lookup"><span data-stu-id="46e61-114">range</span></span>|[<span data-ttu-id="46e61-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="46e61-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="46e61-116">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="46e61-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46e61-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46e61-117">JSON representation</span></span>

<span data-ttu-id="46e61-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="46e61-118">Here is a JSON representation of the resource</span></span>

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
