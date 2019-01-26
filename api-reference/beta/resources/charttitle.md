---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトル オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0b669593bd9ca0768ad977ace8d54f5531301a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573096"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="7a578-103">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a578-103">ChartTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a578-104">グラフのグラフ タイトル オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7a578-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7a578-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a578-105">Methods</span></span>

| <span data-ttu-id="7a578-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a578-106">Method</span></span>           | <span data-ttu-id="7a578-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a578-107">Return Type</span></span>    |<span data-ttu-id="7a578-108">説明</span><span class="sxs-lookup"><span data-stu-id="7a578-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a578-109">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="7a578-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="7a578-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="7a578-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="7a578-111">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7a578-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="7a578-112">Update</span><span class="sxs-lookup"><span data-stu-id="7a578-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="7a578-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="7a578-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="7a578-114">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="7a578-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a578-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a578-115">Properties</span></span>
| <span data-ttu-id="7a578-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a578-116">Property</span></span>     | <span data-ttu-id="7a578-117">型</span><span class="sxs-lookup"><span data-stu-id="7a578-117">Type</span></span>   |<span data-ttu-id="7a578-118">説明</span><span class="sxs-lookup"><span data-stu-id="7a578-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a578-119">overlay</span><span class="sxs-lookup"><span data-stu-id="7a578-119">overlay</span></span>|<span data-ttu-id="7a578-120">boolean</span><span class="sxs-lookup"><span data-stu-id="7a578-120">boolean</span></span>|<span data-ttu-id="7a578-121">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7a578-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="7a578-122">text</span><span class="sxs-lookup"><span data-stu-id="7a578-122">text</span></span>|<span data-ttu-id="7a578-123">文字列</span><span class="sxs-lookup"><span data-stu-id="7a578-123">string</span></span>|<span data-ttu-id="7a578-124">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="7a578-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="7a578-125">visible</span><span class="sxs-lookup"><span data-stu-id="7a578-125">visible</span></span>|<span data-ttu-id="7a578-126">boolean</span><span class="sxs-lookup"><span data-stu-id="7a578-126">boolean</span></span>|<span data-ttu-id="7a578-127">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7a578-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a578-128">関係</span><span class="sxs-lookup"><span data-stu-id="7a578-128">Relationships</span></span>
| <span data-ttu-id="7a578-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a578-129">Relationship</span></span> | <span data-ttu-id="7a578-130">型</span><span class="sxs-lookup"><span data-stu-id="7a578-130">Type</span></span>   |<span data-ttu-id="7a578-131">説明</span><span class="sxs-lookup"><span data-stu-id="7a578-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a578-132">format</span><span class="sxs-lookup"><span data-stu-id="7a578-132">format</span></span>|[<span data-ttu-id="7a578-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="7a578-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="7a578-p101">グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7a578-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a578-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a578-136">JSON representation</span></span>

<span data-ttu-id="7a578-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a578-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
