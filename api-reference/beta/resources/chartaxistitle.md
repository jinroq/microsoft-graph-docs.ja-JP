---
title: ChartAxisTitle リソースの種類
description: グラフ軸のタイトルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 25a5daf571f7533bd1682974adecad1cfd984894
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513124"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="77add-103">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77add-103">ChartAxisTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77add-104">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="77add-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="77add-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="77add-105">Methods</span></span>

| <span data-ttu-id="77add-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="77add-106">Method</span></span>           | <span data-ttu-id="77add-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="77add-107">Return Type</span></span>    |<span data-ttu-id="77add-108">説明</span><span class="sxs-lookup"><span data-stu-id="77add-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77add-109">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="77add-109">[Get ChartAxisTitle](../api/chartaxistitle-get.md)</span></span> | [<span data-ttu-id="77add-110">chartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="77add-110">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="77add-111">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="77add-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="77add-112">Update</span><span class="sxs-lookup"><span data-stu-id="77add-112">Update</span></span>](../api/chartaxistitle-update.md) | <span data-ttu-id="77add-113">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="77add-113">[ChartAxisTitle](chartaxistitle.md)</span></span>    |<span data-ttu-id="77add-114">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="77add-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77add-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77add-115">Properties</span></span>
| <span data-ttu-id="77add-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77add-116">Property</span></span>     | <span data-ttu-id="77add-117">型</span><span class="sxs-lookup"><span data-stu-id="77add-117">Type</span></span>   |<span data-ttu-id="77add-118">説明</span><span class="sxs-lookup"><span data-stu-id="77add-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77add-119">text</span><span class="sxs-lookup"><span data-stu-id="77add-119">text</span></span>|<span data-ttu-id="77add-120">文字列</span><span class="sxs-lookup"><span data-stu-id="77add-120">string</span></span>|<span data-ttu-id="77add-121">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="77add-121">Represents the axis title.</span></span>|
|<span data-ttu-id="77add-122">visible</span><span class="sxs-lookup"><span data-stu-id="77add-122">visible</span></span>|<span data-ttu-id="77add-123">boolean</span><span class="sxs-lookup"><span data-stu-id="77add-123">boolean</span></span>|<span data-ttu-id="77add-124">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="77add-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77add-125">関係</span><span class="sxs-lookup"><span data-stu-id="77add-125">Relationships</span></span>
| <span data-ttu-id="77add-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="77add-126">Relationship</span></span> | <span data-ttu-id="77add-127">型</span><span class="sxs-lookup"><span data-stu-id="77add-127">Type</span></span>   |<span data-ttu-id="77add-128">説明</span><span class="sxs-lookup"><span data-stu-id="77add-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77add-129">format</span><span class="sxs-lookup"><span data-stu-id="77add-129">format</span></span>|[<span data-ttu-id="77add-130">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="77add-130">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="77add-p101">グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="77add-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77add-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77add-133">JSON representation</span></span>

<span data-ttu-id="77add-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="77add-134">Here is a JSON representation of the resource.</span></span>

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
