---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトル オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db0b95e0e01fcbf1c962689a1615066692700992
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977564"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="85d62-103">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85d62-103">ChartTitle resource type</span></span>

> <span data-ttu-id="85d62-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="85d62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85d62-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85d62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85d62-106">グラフのグラフ タイトル オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="85d62-106">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="85d62-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="85d62-107">Methods</span></span>

| <span data-ttu-id="85d62-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="85d62-108">Method</span></span>           | <span data-ttu-id="85d62-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="85d62-109">Return Type</span></span>    |<span data-ttu-id="85d62-110">説明</span><span class="sxs-lookup"><span data-stu-id="85d62-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85d62-111">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="85d62-111">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="85d62-112">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="85d62-112">ChartTitle</span></span>](charttitle.md) |<span data-ttu-id="85d62-113">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="85d62-113">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="85d62-114">Update</span><span class="sxs-lookup"><span data-stu-id="85d62-114">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="85d62-115">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="85d62-115">ChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="85d62-116">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="85d62-116">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="85d62-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85d62-117">Properties</span></span>
| <span data-ttu-id="85d62-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85d62-118">Property</span></span>     | <span data-ttu-id="85d62-119">型</span><span class="sxs-lookup"><span data-stu-id="85d62-119">Type</span></span>   |<span data-ttu-id="85d62-120">説明</span><span class="sxs-lookup"><span data-stu-id="85d62-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85d62-121">overlay</span><span class="sxs-lookup"><span data-stu-id="85d62-121">overlay</span></span>|<span data-ttu-id="85d62-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="85d62-122">boolean</span></span>|<span data-ttu-id="85d62-123">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="85d62-123">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="85d62-124">text</span><span class="sxs-lookup"><span data-stu-id="85d62-124">text</span></span>|<span data-ttu-id="85d62-125">文字列</span><span class="sxs-lookup"><span data-stu-id="85d62-125">string</span></span>|<span data-ttu-id="85d62-126">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="85d62-126">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="85d62-127">visible</span><span class="sxs-lookup"><span data-stu-id="85d62-127">visible</span></span>|<span data-ttu-id="85d62-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="85d62-128">boolean</span></span>|<span data-ttu-id="85d62-129">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="85d62-129">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85d62-130">関係</span><span class="sxs-lookup"><span data-stu-id="85d62-130">Relationships</span></span>
| <span data-ttu-id="85d62-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85d62-131">Relationship</span></span> | <span data-ttu-id="85d62-132">型</span><span class="sxs-lookup"><span data-stu-id="85d62-132">Type</span></span>   |<span data-ttu-id="85d62-133">説明</span><span class="sxs-lookup"><span data-stu-id="85d62-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85d62-134">format</span><span class="sxs-lookup"><span data-stu-id="85d62-134">format</span></span>|[<span data-ttu-id="85d62-135">ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="85d62-135">ChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="85d62-p102">グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="85d62-p102">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85d62-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85d62-138">JSON representation</span></span>

<span data-ttu-id="85d62-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="85d62-139">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
