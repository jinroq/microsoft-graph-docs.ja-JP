---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトル オブジェクトを表します。
author: lumine2008
ms.openlocfilehash: b020cd28f889b2a4ee95f06794c1fc61a7dd5eb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337402"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="52e81-103">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52e81-103">ChartTitle resource type</span></span>

<span data-ttu-id="52e81-104">グラフのグラフ タイトル オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="52e81-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="52e81-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="52e81-105">Methods</span></span>

| <span data-ttu-id="52e81-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="52e81-106">Method</span></span>           | <span data-ttu-id="52e81-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="52e81-107">Return Type</span></span>    |<span data-ttu-id="52e81-108">説明</span><span class="sxs-lookup"><span data-stu-id="52e81-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52e81-109">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="52e81-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="52e81-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="52e81-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="52e81-111">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="52e81-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="52e81-112">Update</span><span class="sxs-lookup"><span data-stu-id="52e81-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="52e81-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="52e81-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="52e81-114">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="52e81-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52e81-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52e81-115">Properties</span></span>
| <span data-ttu-id="52e81-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52e81-116">Property</span></span>     | <span data-ttu-id="52e81-117">種類</span><span class="sxs-lookup"><span data-stu-id="52e81-117">Type</span></span>   |<span data-ttu-id="52e81-118">説明</span><span class="sxs-lookup"><span data-stu-id="52e81-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52e81-119">overlay</span><span class="sxs-lookup"><span data-stu-id="52e81-119">overlay</span></span>|<span data-ttu-id="52e81-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="52e81-120">boolean</span></span>|<span data-ttu-id="52e81-121">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="52e81-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="52e81-122">text</span><span class="sxs-lookup"><span data-stu-id="52e81-122">text</span></span>|<span data-ttu-id="52e81-123">文字列</span><span class="sxs-lookup"><span data-stu-id="52e81-123">string</span></span>|<span data-ttu-id="52e81-124">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="52e81-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="52e81-125">visible</span><span class="sxs-lookup"><span data-stu-id="52e81-125">visible</span></span>|<span data-ttu-id="52e81-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="52e81-126">boolean</span></span>|<span data-ttu-id="52e81-127">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="52e81-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52e81-128">関係</span><span class="sxs-lookup"><span data-stu-id="52e81-128">Relationships</span></span>
| <span data-ttu-id="52e81-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52e81-129">Relationship</span></span> | <span data-ttu-id="52e81-130">型</span><span class="sxs-lookup"><span data-stu-id="52e81-130">Type</span></span>   |<span data-ttu-id="52e81-131">説明</span><span class="sxs-lookup"><span data-stu-id="52e81-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52e81-132">format</span><span class="sxs-lookup"><span data-stu-id="52e81-132">format</span></span>|[<span data-ttu-id="52e81-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="52e81-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="52e81-p101">グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="52e81-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52e81-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52e81-136">JSON representation</span></span>

<span data-ttu-id="52e81-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52e81-137">Here is a JSON representation of the resource.</span></span>

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