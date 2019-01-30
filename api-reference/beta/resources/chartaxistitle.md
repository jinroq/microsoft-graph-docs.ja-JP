---
title: ChartAxisTitle リソースの種類
description: グラフ軸のタイトルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 25a5daf571f7533bd1682974adecad1cfd984894
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644085"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="e6f30-103">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6f30-103">ChartAxisTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f30-104">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="e6f30-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="e6f30-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6f30-105">Methods</span></span>

| <span data-ttu-id="e6f30-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6f30-106">Method</span></span>           | <span data-ttu-id="e6f30-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6f30-107">Return Type</span></span>    |<span data-ttu-id="e6f30-108">説明</span><span class="sxs-lookup"><span data-stu-id="e6f30-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6f30-109">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="e6f30-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="e6f30-110">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="e6f30-110">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="e6f30-111">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e6f30-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="e6f30-112">更新する</span><span class="sxs-lookup"><span data-stu-id="e6f30-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="e6f30-113">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="e6f30-113">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="e6f30-114">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e6f30-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6f30-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6f30-115">Properties</span></span>
| <span data-ttu-id="e6f30-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6f30-116">Property</span></span>     | <span data-ttu-id="e6f30-117">型</span><span class="sxs-lookup"><span data-stu-id="e6f30-117">Type</span></span>   |<span data-ttu-id="e6f30-118">説明</span><span class="sxs-lookup"><span data-stu-id="e6f30-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f30-119">text</span><span class="sxs-lookup"><span data-stu-id="e6f30-119">text</span></span>|<span data-ttu-id="e6f30-120">文字列</span><span class="sxs-lookup"><span data-stu-id="e6f30-120">string</span></span>|<span data-ttu-id="e6f30-121">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="e6f30-121">Represents the axis title.</span></span>|
|<span data-ttu-id="e6f30-122">visible</span><span class="sxs-lookup"><span data-stu-id="e6f30-122">visible</span></span>|<span data-ttu-id="e6f30-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="e6f30-123">boolean</span></span>|<span data-ttu-id="e6f30-124">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="e6f30-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6f30-125">関係</span><span class="sxs-lookup"><span data-stu-id="e6f30-125">Relationships</span></span>
| <span data-ttu-id="e6f30-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6f30-126">Relationship</span></span> | <span data-ttu-id="e6f30-127">型</span><span class="sxs-lookup"><span data-stu-id="e6f30-127">Type</span></span>   |<span data-ttu-id="e6f30-128">説明</span><span class="sxs-lookup"><span data-stu-id="e6f30-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f30-129">format</span><span class="sxs-lookup"><span data-stu-id="e6f30-129">format</span></span>|[<span data-ttu-id="e6f30-130">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="e6f30-130">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="e6f30-p101">グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e6f30-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6f30-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6f30-133">JSON representation</span></span>

<span data-ttu-id="e6f30-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6f30-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
