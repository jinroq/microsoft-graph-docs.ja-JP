---
title: ChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
ms.openlocfilehash: be9d0d3f30deb608aee9873866442e0478c0056a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352186"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="bf4f7-103">ChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf4f7-103">ChartLineFormat resource type</span></span>

> <span data-ttu-id="bf4f7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf4f7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf4f7-106">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-106">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="bf4f7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf4f7-107">Methods</span></span>

| <span data-ttu-id="bf4f7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf4f7-108">Method</span></span>           | <span data-ttu-id="bf4f7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bf4f7-109">Return Type</span></span>    |<span data-ttu-id="bf4f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf4f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf4f7-111">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bf4f7-111">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="bf4f7-112">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bf4f7-112">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="bf4f7-113">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-113">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="bf4f7-114">Update</span><span class="sxs-lookup"><span data-stu-id="bf4f7-114">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="bf4f7-115">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bf4f7-115">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="bf4f7-116">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-116">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="bf4f7-117">Clear</span><span class="sxs-lookup"><span data-stu-id="bf4f7-117">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="bf4f7-118">なし</span><span class="sxs-lookup"><span data-stu-id="bf4f7-118">None</span></span>|<span data-ttu-id="bf4f7-119">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-119">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf4f7-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf4f7-120">Properties</span></span>
| <span data-ttu-id="bf4f7-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf4f7-121">Property</span></span>     | <span data-ttu-id="bf4f7-122">種類</span><span class="sxs-lookup"><span data-stu-id="bf4f7-122">Type</span></span>   |<span data-ttu-id="bf4f7-123">説明</span><span class="sxs-lookup"><span data-stu-id="bf4f7-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf4f7-124">color</span><span class="sxs-lookup"><span data-stu-id="bf4f7-124">color</span></span>|<span data-ttu-id="bf4f7-125">文字列</span><span class="sxs-lookup"><span data-stu-id="bf4f7-125">string</span></span>|<span data-ttu-id="bf4f7-126">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-126">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf4f7-127">関係</span><span class="sxs-lookup"><span data-stu-id="bf4f7-127">Relationships</span></span>
<span data-ttu-id="bf4f7-128">なし</span><span class="sxs-lookup"><span data-stu-id="bf4f7-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bf4f7-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf4f7-129">JSON representation</span></span>

<span data-ttu-id="bf4f7-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf4f7-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->