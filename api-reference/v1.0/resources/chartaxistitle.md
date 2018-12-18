---
title: ChartAxisTitle リソースの種類
description: グラフ軸のタイトルを表します。
author: lumine2008
ms.openlocfilehash: 785caa4d48cf32c5892d05238b4137691fd0f5c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317263"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="2b375-103">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b375-103">ChartAxisTitle resource type</span></span>

<span data-ttu-id="2b375-104">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="2b375-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="2b375-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b375-105">Methods</span></span>

| <span data-ttu-id="2b375-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b375-106">Method</span></span>           | <span data-ttu-id="2b375-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2b375-107">Return Type</span></span>    |<span data-ttu-id="2b375-108">説明</span><span class="sxs-lookup"><span data-stu-id="2b375-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b375-109">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="2b375-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="2b375-110">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="2b375-110">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="2b375-111">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2b375-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="2b375-112">Update</span><span class="sxs-lookup"><span data-stu-id="2b375-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="2b375-113">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="2b375-113">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="2b375-114">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2b375-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2b375-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b375-115">Properties</span></span>
| <span data-ttu-id="2b375-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b375-116">Property</span></span>     | <span data-ttu-id="2b375-117">種類</span><span class="sxs-lookup"><span data-stu-id="2b375-117">Type</span></span>   |<span data-ttu-id="2b375-118">説明</span><span class="sxs-lookup"><span data-stu-id="2b375-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b375-119">text</span><span class="sxs-lookup"><span data-stu-id="2b375-119">text</span></span>|<span data-ttu-id="2b375-120">文字列</span><span class="sxs-lookup"><span data-stu-id="2b375-120">string</span></span>|<span data-ttu-id="2b375-121">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="2b375-121">Represents the axis title.</span></span>|
|<span data-ttu-id="2b375-122">visible</span><span class="sxs-lookup"><span data-stu-id="2b375-122">visible</span></span>|<span data-ttu-id="2b375-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="2b375-123">boolean</span></span>|<span data-ttu-id="2b375-124">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="2b375-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b375-125">関係</span><span class="sxs-lookup"><span data-stu-id="2b375-125">Relationships</span></span>
| <span data-ttu-id="2b375-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b375-126">Relationship</span></span> | <span data-ttu-id="2b375-127">型</span><span class="sxs-lookup"><span data-stu-id="2b375-127">Type</span></span>   |<span data-ttu-id="2b375-128">説明</span><span class="sxs-lookup"><span data-stu-id="2b375-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b375-129">format</span><span class="sxs-lookup"><span data-stu-id="2b375-129">format</span></span>|[<span data-ttu-id="2b375-130">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="2b375-130">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="2b375-p101">グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2b375-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b375-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b375-133">JSON representation</span></span>

<span data-ttu-id="2b375-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b375-134">Here is a JSON representation of the resource.</span></span>

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