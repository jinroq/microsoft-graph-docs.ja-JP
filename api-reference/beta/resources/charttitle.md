---
title: ChartTitle リソースの種類
description: グラフのグラフ タイトル オブジェクトを表します。
author: lumine2008
ms.openlocfilehash: b3d685c68b14ebe3f49eb3dd9186838c977c1cac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338102"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="bdffe-103">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdffe-103">ChartTitle resource type</span></span>

> <span data-ttu-id="bdffe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bdffe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdffe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdffe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdffe-106">グラフのグラフ タイトル オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="bdffe-106">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="bdffe-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bdffe-107">Methods</span></span>

| <span data-ttu-id="bdffe-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bdffe-108">Method</span></span>           | <span data-ttu-id="bdffe-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bdffe-109">Return Type</span></span>    |<span data-ttu-id="bdffe-110">説明</span><span class="sxs-lookup"><span data-stu-id="bdffe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdffe-111">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="bdffe-111">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="bdffe-112">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="bdffe-112">ChartTitle</span></span>](charttitle.md) |<span data-ttu-id="bdffe-113">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bdffe-113">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="bdffe-114">Update</span><span class="sxs-lookup"><span data-stu-id="bdffe-114">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="bdffe-115">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="bdffe-115">ChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="bdffe-116">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bdffe-116">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bdffe-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdffe-117">Properties</span></span>
| <span data-ttu-id="bdffe-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdffe-118">Property</span></span>     | <span data-ttu-id="bdffe-119">種類</span><span class="sxs-lookup"><span data-stu-id="bdffe-119">Type</span></span>   |<span data-ttu-id="bdffe-120">説明</span><span class="sxs-lookup"><span data-stu-id="bdffe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdffe-121">overlay</span><span class="sxs-lookup"><span data-stu-id="bdffe-121">overlay</span></span>|<span data-ttu-id="bdffe-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="bdffe-122">boolean</span></span>|<span data-ttu-id="bdffe-123">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="bdffe-123">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="bdffe-124">text</span><span class="sxs-lookup"><span data-stu-id="bdffe-124">text</span></span>|<span data-ttu-id="bdffe-125">文字列</span><span class="sxs-lookup"><span data-stu-id="bdffe-125">string</span></span>|<span data-ttu-id="bdffe-126">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="bdffe-126">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="bdffe-127">visible</span><span class="sxs-lookup"><span data-stu-id="bdffe-127">visible</span></span>|<span data-ttu-id="bdffe-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="bdffe-128">boolean</span></span>|<span data-ttu-id="bdffe-129">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="bdffe-129">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdffe-130">関係</span><span class="sxs-lookup"><span data-stu-id="bdffe-130">Relationships</span></span>
| <span data-ttu-id="bdffe-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bdffe-131">Relationship</span></span> | <span data-ttu-id="bdffe-132">型</span><span class="sxs-lookup"><span data-stu-id="bdffe-132">Type</span></span>   |<span data-ttu-id="bdffe-133">説明</span><span class="sxs-lookup"><span data-stu-id="bdffe-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdffe-134">format</span><span class="sxs-lookup"><span data-stu-id="bdffe-134">format</span></span>|[<span data-ttu-id="bdffe-135">ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="bdffe-135">ChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="bdffe-p102">グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="bdffe-p102">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdffe-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdffe-138">JSON representation</span></span>

<span data-ttu-id="bdffe-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bdffe-139">Here is a JSON representation of the resource.</span></span>

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