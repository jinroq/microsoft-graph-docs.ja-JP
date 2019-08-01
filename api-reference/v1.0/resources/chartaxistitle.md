---
title: ChartAxisTitle リソースの種類
description: グラフ軸のタイトルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5c89b3e90cce7dcc064dfd7186eafcc26a37dd0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033027"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="ead37-103">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ead37-103">ChartAxisTitle resource type</span></span>

<span data-ttu-id="ead37-104">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="ead37-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="ead37-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ead37-105">Methods</span></span>

| <span data-ttu-id="ead37-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ead37-106">Method</span></span>           | <span data-ttu-id="ead37-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ead37-107">Return Type</span></span>    |<span data-ttu-id="ead37-108">説明</span><span class="sxs-lookup"><span data-stu-id="ead37-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ead37-109">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="ead37-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="ead37-110">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="ead37-110">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="ead37-111">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ead37-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="ead37-112">Update</span><span class="sxs-lookup"><span data-stu-id="ead37-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="ead37-113">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="ead37-113">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="ead37-114">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ead37-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ead37-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ead37-115">Properties</span></span>
| <span data-ttu-id="ead37-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ead37-116">Property</span></span>     | <span data-ttu-id="ead37-117">型</span><span class="sxs-lookup"><span data-stu-id="ead37-117">Type</span></span>   |<span data-ttu-id="ead37-118">説明</span><span class="sxs-lookup"><span data-stu-id="ead37-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ead37-119">text</span><span class="sxs-lookup"><span data-stu-id="ead37-119">text</span></span>|<span data-ttu-id="ead37-120">string</span><span class="sxs-lookup"><span data-stu-id="ead37-120">string</span></span>|<span data-ttu-id="ead37-121">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="ead37-121">Represents the axis title.</span></span>|
|<span data-ttu-id="ead37-122">visible</span><span class="sxs-lookup"><span data-stu-id="ead37-122">visible</span></span>|<span data-ttu-id="ead37-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="ead37-123">boolean</span></span>|<span data-ttu-id="ead37-124">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="ead37-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ead37-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ead37-125">Relationships</span></span>
| <span data-ttu-id="ead37-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ead37-126">Relationship</span></span> | <span data-ttu-id="ead37-127">型</span><span class="sxs-lookup"><span data-stu-id="ead37-127">Type</span></span>   |<span data-ttu-id="ead37-128">説明</span><span class="sxs-lookup"><span data-stu-id="ead37-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ead37-129">format</span><span class="sxs-lookup"><span data-stu-id="ead37-129">format</span></span>|[<span data-ttu-id="ead37-130">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="ead37-130">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="ead37-131">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="ead37-131">Represents the formatting of chart axis title.</span></span> <span data-ttu-id="ead37-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ead37-132">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ead37-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ead37-133">JSON representation</span></span>

<span data-ttu-id="ead37-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ead37-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
