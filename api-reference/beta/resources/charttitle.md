---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトルのオブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a71aed2da93c2121492f1eb29826470b797768ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460990"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="52058-103">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52058-103">ChartTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52058-104">グラフのグラフ タイトルのオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="52058-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="52058-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="52058-105">Methods</span></span>

| <span data-ttu-id="52058-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="52058-106">Method</span></span>           | <span data-ttu-id="52058-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="52058-107">Return Type</span></span>    |<span data-ttu-id="52058-108">説明</span><span class="sxs-lookup"><span data-stu-id="52058-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52058-109">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="52058-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="52058-110">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="52058-110">ChartTitle</span></span>](charttitle.md) |<span data-ttu-id="52058-111">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="52058-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="52058-112">Update</span><span class="sxs-lookup"><span data-stu-id="52058-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="52058-113">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="52058-113">ChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="52058-114">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="52058-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52058-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52058-115">Properties</span></span>
| <span data-ttu-id="52058-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52058-116">Property</span></span>     | <span data-ttu-id="52058-117">型</span><span class="sxs-lookup"><span data-stu-id="52058-117">Type</span></span>   |<span data-ttu-id="52058-118">説明</span><span class="sxs-lookup"><span data-stu-id="52058-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52058-119">overlay</span><span class="sxs-lookup"><span data-stu-id="52058-119">overlay</span></span>|<span data-ttu-id="52058-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="52058-120">boolean</span></span>|<span data-ttu-id="52058-121">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="52058-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="52058-122">text</span><span class="sxs-lookup"><span data-stu-id="52058-122">text</span></span>|<span data-ttu-id="52058-123">string</span><span class="sxs-lookup"><span data-stu-id="52058-123">string</span></span>|<span data-ttu-id="52058-124">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="52058-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="52058-125">visible</span><span class="sxs-lookup"><span data-stu-id="52058-125">visible</span></span>|<span data-ttu-id="52058-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="52058-126">boolean</span></span>|<span data-ttu-id="52058-127">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="52058-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52058-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52058-128">Relationships</span></span>
| <span data-ttu-id="52058-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52058-129">Relationship</span></span> | <span data-ttu-id="52058-130">型</span><span class="sxs-lookup"><span data-stu-id="52058-130">Type</span></span>   |<span data-ttu-id="52058-131">説明</span><span class="sxs-lookup"><span data-stu-id="52058-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52058-132">format</span><span class="sxs-lookup"><span data-stu-id="52058-132">format</span></span>|[<span data-ttu-id="52058-133">ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="52058-133">ChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="52058-p101">グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="52058-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52058-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52058-136">JSON representation</span></span>

<span data-ttu-id="52058-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52058-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
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
