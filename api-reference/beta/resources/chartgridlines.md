---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
ms.openlocfilehash: c09580b2c669710d8aabf60e31c3c36965bfaa6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066520"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="9d2f3-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d2f3-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="9d2f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d2f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d2f3-106">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="9d2f3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d2f3-107">Methods</span></span>

| <span data-ttu-id="9d2f3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d2f3-108">Method</span></span>           | <span data-ttu-id="9d2f3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9d2f3-109">Return Type</span></span>    |<span data-ttu-id="9d2f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="9d2f3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d2f3-111">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9d2f3-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="9d2f3-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9d2f3-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="9d2f3-113">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="9d2f3-114">Update</span><span class="sxs-lookup"><span data-stu-id="9d2f3-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="9d2f3-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9d2f3-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="9d2f3-116">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d2f3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d2f3-117">Properties</span></span>
| <span data-ttu-id="9d2f3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d2f3-118">Property</span></span>     | <span data-ttu-id="9d2f3-119">型</span><span class="sxs-lookup"><span data-stu-id="9d2f3-119">Type</span></span>   |<span data-ttu-id="9d2f3-120">説明</span><span class="sxs-lookup"><span data-stu-id="9d2f3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d2f3-121">visible</span><span class="sxs-lookup"><span data-stu-id="9d2f3-121">visible</span></span>|<span data-ttu-id="9d2f3-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="9d2f3-122">boolean</span></span>|<span data-ttu-id="9d2f3-123">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d2f3-124">関係</span><span class="sxs-lookup"><span data-stu-id="9d2f3-124">Relationships</span></span>
| <span data-ttu-id="9d2f3-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9d2f3-125">Relationship</span></span> | <span data-ttu-id="9d2f3-126">型</span><span class="sxs-lookup"><span data-stu-id="9d2f3-126">Type</span></span>   |<span data-ttu-id="9d2f3-127">説明</span><span class="sxs-lookup"><span data-stu-id="9d2f3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d2f3-128">format</span><span class="sxs-lookup"><span data-stu-id="9d2f3-128">format</span></span>|[<span data-ttu-id="9d2f3-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="9d2f3-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="9d2f3-p102">グラフの目盛線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d2f3-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d2f3-132">JSON representation</span></span>

<span data-ttu-id="9d2f3-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->