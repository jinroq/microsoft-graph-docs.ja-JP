---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトルのオブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f6c843e24839b51da67bda5ed3484a32c868ae54
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584992"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="f4962-103">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4962-103">ChartTitle resource type</span></span>

<span data-ttu-id="f4962-104">グラフのグラフ タイトルのオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="f4962-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f4962-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4962-105">Methods</span></span>

| <span data-ttu-id="f4962-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4962-106">Method</span></span>           | <span data-ttu-id="f4962-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f4962-107">Return Type</span></span>    |<span data-ttu-id="f4962-108">説明</span><span class="sxs-lookup"><span data-stu-id="f4962-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4962-109">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="f4962-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="f4962-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="f4962-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="f4962-111">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4962-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="f4962-112">Update</span><span class="sxs-lookup"><span data-stu-id="f4962-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="f4962-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="f4962-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="f4962-114">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4962-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4962-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4962-115">Properties</span></span>
| <span data-ttu-id="f4962-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4962-116">Property</span></span>     | <span data-ttu-id="f4962-117">型</span><span class="sxs-lookup"><span data-stu-id="f4962-117">Type</span></span>   |<span data-ttu-id="f4962-118">説明</span><span class="sxs-lookup"><span data-stu-id="f4962-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4962-119">overlay</span><span class="sxs-lookup"><span data-stu-id="f4962-119">overlay</span></span>|<span data-ttu-id="f4962-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="f4962-120">boolean</span></span>|<span data-ttu-id="f4962-121">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="f4962-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="f4962-122">text</span><span class="sxs-lookup"><span data-stu-id="f4962-122">text</span></span>|<span data-ttu-id="f4962-123">string</span><span class="sxs-lookup"><span data-stu-id="f4962-123">string</span></span>|<span data-ttu-id="f4962-124">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="f4962-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="f4962-125">visible</span><span class="sxs-lookup"><span data-stu-id="f4962-125">visible</span></span>|<span data-ttu-id="f4962-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="f4962-126">boolean</span></span>|<span data-ttu-id="f4962-127">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="f4962-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4962-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4962-128">Relationships</span></span>
| <span data-ttu-id="f4962-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4962-129">Relationship</span></span> | <span data-ttu-id="f4962-130">型</span><span class="sxs-lookup"><span data-stu-id="f4962-130">Type</span></span>   |<span data-ttu-id="f4962-131">説明</span><span class="sxs-lookup"><span data-stu-id="f4962-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4962-132">format</span><span class="sxs-lookup"><span data-stu-id="f4962-132">format</span></span>|[<span data-ttu-id="f4962-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="f4962-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="f4962-134">塗りつぶしとフォントの書式設定を含む、グラフタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="f4962-134">Represents the formatting of a chart title, which includes fill and font formatting.</span></span> <span data-ttu-id="f4962-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f4962-135">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4962-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4962-136">JSON representation</span></span>

<span data-ttu-id="f4962-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4962-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
