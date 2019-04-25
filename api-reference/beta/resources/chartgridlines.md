---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 852b52fd70e619b8720ef56fb0e857fb499f0abf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543703"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="ec4e8-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ec4e8-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec4e8-104">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="ec4e8-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="ec4e8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ec4e8-105">Methods</span></span>

| <span data-ttu-id="ec4e8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ec4e8-106">Method</span></span>           | <span data-ttu-id="ec4e8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ec4e8-107">Return Type</span></span>    |<span data-ttu-id="ec4e8-108">説明</span><span class="sxs-lookup"><span data-stu-id="ec4e8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec4e8-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="ec4e8-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="ec4e8-110">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="ec4e8-110">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="ec4e8-111">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ec4e8-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="ec4e8-112">Update</span><span class="sxs-lookup"><span data-stu-id="ec4e8-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="ec4e8-113">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="ec4e8-113">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="ec4e8-114">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ec4e8-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec4e8-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec4e8-115">Properties</span></span>
| <span data-ttu-id="ec4e8-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec4e8-116">Property</span></span>     | <span data-ttu-id="ec4e8-117">型</span><span class="sxs-lookup"><span data-stu-id="ec4e8-117">Type</span></span>   |<span data-ttu-id="ec4e8-118">説明</span><span class="sxs-lookup"><span data-stu-id="ec4e8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec4e8-119">visible</span><span class="sxs-lookup"><span data-stu-id="ec4e8-119">visible</span></span>|<span data-ttu-id="ec4e8-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="ec4e8-120">boolean</span></span>|<span data-ttu-id="ec4e8-121">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="ec4e8-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec4e8-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ec4e8-122">Relationships</span></span>
| <span data-ttu-id="ec4e8-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ec4e8-123">Relationship</span></span> | <span data-ttu-id="ec4e8-124">型</span><span class="sxs-lookup"><span data-stu-id="ec4e8-124">Type</span></span>   |<span data-ttu-id="ec4e8-125">説明</span><span class="sxs-lookup"><span data-stu-id="ec4e8-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec4e8-126">format</span><span class="sxs-lookup"><span data-stu-id="ec4e8-126">format</span></span>|[<span data-ttu-id="ec4e8-127">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="ec4e8-127">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="ec4e8-p101">グラフの目盛線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ec4e8-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec4e8-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ec4e8-130">JSON representation</span></span>

<span data-ttu-id="ec4e8-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ec4e8-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
