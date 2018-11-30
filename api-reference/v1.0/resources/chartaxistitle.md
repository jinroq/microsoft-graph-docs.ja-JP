---
title: ChartAxisTitle リソースの種類
description: グラフ軸のタイトルを表します。
ms.openlocfilehash: ede660e2ba5d0ab34e8b985574e3077ca06b32b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021604"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="084ac-103">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="084ac-103">ChartAxisTitle resource type</span></span>

<span data-ttu-id="084ac-104">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="084ac-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="084ac-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="084ac-105">Methods</span></span>

| <span data-ttu-id="084ac-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="084ac-106">Method</span></span>           | <span data-ttu-id="084ac-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="084ac-107">Return Type</span></span>    |<span data-ttu-id="084ac-108">説明</span><span class="sxs-lookup"><span data-stu-id="084ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="084ac-109">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="084ac-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="084ac-110">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="084ac-110">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="084ac-111">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="084ac-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="084ac-112">Update</span><span class="sxs-lookup"><span data-stu-id="084ac-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="084ac-113">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="084ac-113">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="084ac-114">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="084ac-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="084ac-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="084ac-115">Properties</span></span>
| <span data-ttu-id="084ac-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="084ac-116">Property</span></span>     | <span data-ttu-id="084ac-117">型</span><span class="sxs-lookup"><span data-stu-id="084ac-117">Type</span></span>   |<span data-ttu-id="084ac-118">説明</span><span class="sxs-lookup"><span data-stu-id="084ac-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="084ac-119">text</span><span class="sxs-lookup"><span data-stu-id="084ac-119">text</span></span>|<span data-ttu-id="084ac-120">文字列</span><span class="sxs-lookup"><span data-stu-id="084ac-120">string</span></span>|<span data-ttu-id="084ac-121">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="084ac-121">Represents the axis title.</span></span>|
|<span data-ttu-id="084ac-122">visible</span><span class="sxs-lookup"><span data-stu-id="084ac-122">visible</span></span>|<span data-ttu-id="084ac-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="084ac-123">boolean</span></span>|<span data-ttu-id="084ac-124">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="084ac-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="084ac-125">関係</span><span class="sxs-lookup"><span data-stu-id="084ac-125">Relationships</span></span>
| <span data-ttu-id="084ac-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="084ac-126">Relationship</span></span> | <span data-ttu-id="084ac-127">型</span><span class="sxs-lookup"><span data-stu-id="084ac-127">Type</span></span>   |<span data-ttu-id="084ac-128">説明</span><span class="sxs-lookup"><span data-stu-id="084ac-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="084ac-129">format</span><span class="sxs-lookup"><span data-stu-id="084ac-129">format</span></span>|[<span data-ttu-id="084ac-130">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="084ac-130">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="084ac-p101">グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="084ac-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="084ac-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="084ac-133">JSON representation</span></span>

<span data-ttu-id="084ac-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="084ac-134">Here is a JSON representation of the resource.</span></span>

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