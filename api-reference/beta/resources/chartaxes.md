---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
ms.openlocfilehash: a4fc9cf19cbf1f8cc8bf535c21689990bf92fc08
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352760"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="cd721-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd721-103">ChartAxes resource type</span></span>

> <span data-ttu-id="cd721-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd721-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd721-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd721-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd721-106">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="cd721-106">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="cd721-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd721-107">Methods</span></span>
<span data-ttu-id="cd721-108">なし</span><span class="sxs-lookup"><span data-stu-id="cd721-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="cd721-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd721-109">Properties</span></span>
<span data-ttu-id="cd721-110">なし</span><span class="sxs-lookup"><span data-stu-id="cd721-110">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cd721-111">関係</span><span class="sxs-lookup"><span data-stu-id="cd721-111">Relationships</span></span>
| <span data-ttu-id="cd721-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cd721-112">Relationship</span></span> | <span data-ttu-id="cd721-113">型</span><span class="sxs-lookup"><span data-stu-id="cd721-113">Type</span></span>   |<span data-ttu-id="cd721-114">説明</span><span class="sxs-lookup"><span data-stu-id="cd721-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd721-115">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="cd721-115">categoryAxis</span></span>|[<span data-ttu-id="cd721-116">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="cd721-116">ChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="cd721-p102">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cd721-p102">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="cd721-119">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="cd721-119">seriesAxis</span></span>|[<span data-ttu-id="cd721-120">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="cd721-120">ChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="cd721-p103">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cd721-p103">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="cd721-123">valueAxis</span><span class="sxs-lookup"><span data-stu-id="cd721-123">valueAxis</span></span>|[<span data-ttu-id="cd721-124">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="cd721-124">ChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="cd721-p104">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cd721-p104">Represents the value axis in an axis. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->