---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
ms.openlocfilehash: 964133a103d59b699613c4c378295e1d9693e7a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070478"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="81fbe-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81fbe-103">ChartAxes resource type</span></span>

> <span data-ttu-id="81fbe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81fbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81fbe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81fbe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81fbe-106">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="81fbe-106">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="81fbe-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="81fbe-107">Methods</span></span>
<span data-ttu-id="81fbe-108">なし</span><span class="sxs-lookup"><span data-stu-id="81fbe-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="81fbe-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81fbe-109">Properties</span></span>
<span data-ttu-id="81fbe-110">なし</span><span class="sxs-lookup"><span data-stu-id="81fbe-110">None</span></span>

## <a name="relationships"></a><span data-ttu-id="81fbe-111">関係</span><span class="sxs-lookup"><span data-stu-id="81fbe-111">Relationships</span></span>
| <span data-ttu-id="81fbe-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81fbe-112">Relationship</span></span> | <span data-ttu-id="81fbe-113">型</span><span class="sxs-lookup"><span data-stu-id="81fbe-113">Type</span></span>   |<span data-ttu-id="81fbe-114">説明</span><span class="sxs-lookup"><span data-stu-id="81fbe-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81fbe-115">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="81fbe-115">categoryAxis</span></span>|[<span data-ttu-id="81fbe-116">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="81fbe-116">ChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="81fbe-p102">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="81fbe-p102">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="81fbe-119">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="81fbe-119">seriesAxis</span></span>|[<span data-ttu-id="81fbe-120">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="81fbe-120">ChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="81fbe-p103">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="81fbe-p103">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="81fbe-123">valueAxis</span><span class="sxs-lookup"><span data-stu-id="81fbe-123">valueAxis</span></span>|[<span data-ttu-id="81fbe-124">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="81fbe-124">ChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="81fbe-p104">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="81fbe-p104">Represents the value axis in an axis. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->