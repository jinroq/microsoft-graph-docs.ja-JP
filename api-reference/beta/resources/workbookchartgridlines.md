---
title: workbookChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bf2b481b3b60b7cf5893a1c7ab6e2f168c7cc1ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964023"
---
# <a name="workbookchartgridlines-resource-type"></a><span data-ttu-id="5aa6a-103">workbookChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5aa6a-103">workbookChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aa6a-104">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="5aa6a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5aa6a-105">Methods</span></span>

| <span data-ttu-id="5aa6a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5aa6a-106">Method</span></span>           | <span data-ttu-id="5aa6a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5aa6a-107">Return Type</span></span>    |<span data-ttu-id="5aa6a-108">説明</span><span class="sxs-lookup"><span data-stu-id="5aa6a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5aa6a-109">WorkbookChartGridlines を取得する</span><span class="sxs-lookup"><span data-stu-id="5aa6a-109">Get workbookChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="5aa6a-110">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="5aa6a-110">workbookChartGridlines</span></span>](workbookchartgridlines.md) |<span data-ttu-id="5aa6a-111">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="5aa6a-112">Update</span><span class="sxs-lookup"><span data-stu-id="5aa6a-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="5aa6a-113">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="5aa6a-113">workbookChartGridlines</span></span>](workbookchartgridlines.md)    |<span data-ttu-id="5aa6a-114">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5aa6a-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5aa6a-115">Properties</span></span>
| <span data-ttu-id="5aa6a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5aa6a-116">Property</span></span>     | <span data-ttu-id="5aa6a-117">型</span><span class="sxs-lookup"><span data-stu-id="5aa6a-117">Type</span></span>   |<span data-ttu-id="5aa6a-118">説明</span><span class="sxs-lookup"><span data-stu-id="5aa6a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5aa6a-119">visible</span><span class="sxs-lookup"><span data-stu-id="5aa6a-119">visible</span></span>|<span data-ttu-id="5aa6a-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="5aa6a-120">boolean</span></span>|<span data-ttu-id="5aa6a-121">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aa6a-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5aa6a-122">Relationships</span></span>
| <span data-ttu-id="5aa6a-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5aa6a-123">Relationship</span></span> | <span data-ttu-id="5aa6a-124">型</span><span class="sxs-lookup"><span data-stu-id="5aa6a-124">Type</span></span>   |<span data-ttu-id="5aa6a-125">説明</span><span class="sxs-lookup"><span data-stu-id="5aa6a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5aa6a-126">format</span><span class="sxs-lookup"><span data-stu-id="5aa6a-126">format</span></span>|[<span data-ttu-id="5aa6a-127">workbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="5aa6a-127">workbookChartGridlinesFormat</span></span>](workbookchartgridlinesformat.md)|<span data-ttu-id="5aa6a-128">グラフの目盛線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-128">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="5aa6a-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5aa6a-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5aa6a-130">JSON representation</span></span>

<span data-ttu-id="5aa6a-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5aa6a-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
