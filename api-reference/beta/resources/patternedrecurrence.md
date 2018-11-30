---
title: patternedRecurrence リソースの種類
description: 繰り返しのパターンと範囲です。
ms.openlocfilehash: 205c563d8b4cecc0a817dd1893a6c4f002eb4e06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074323"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="dc2de-103">patternedRecurrence リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc2de-103">patternedRecurrence resource type</span></span>

> <span data-ttu-id="dc2de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc2de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc2de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc2de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc2de-106">繰り返しのパターンと範囲です。</span><span class="sxs-lookup"><span data-stu-id="dc2de-106">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="dc2de-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc2de-107">Properties</span></span>
| <span data-ttu-id="dc2de-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc2de-108">Property</span></span>     | <span data-ttu-id="dc2de-109">型</span><span class="sxs-lookup"><span data-stu-id="dc2de-109">Type</span></span>   |<span data-ttu-id="dc2de-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc2de-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc2de-111">pattern</span><span class="sxs-lookup"><span data-stu-id="dc2de-111">pattern</span></span>|[<span data-ttu-id="dc2de-112">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="dc2de-112">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="dc2de-113">イベントの頻度。</span><span class="sxs-lookup"><span data-stu-id="dc2de-113">The frequency of an event.</span></span>|
|<span data-ttu-id="dc2de-114">range</span><span class="sxs-lookup"><span data-stu-id="dc2de-114">range</span></span>|[<span data-ttu-id="dc2de-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="dc2de-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="dc2de-116">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="dc2de-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc2de-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc2de-117">JSON representation</span></span>

<span data-ttu-id="dc2de-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dc2de-118">Here is a JSON representation of the resource</span></span>

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
