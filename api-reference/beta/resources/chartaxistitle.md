---
title: ChartAxisTitle リソースの種類
description: グラフ軸のタイトルを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a78219e5833f7f85cde571dc984959b642ebe4d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894181"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="d0dd0-103">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0dd0-103">ChartAxisTitle resource type</span></span>

> <span data-ttu-id="d0dd0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0dd0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0dd0-106">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-106">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="d0dd0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0dd0-107">Methods</span></span>

| <span data-ttu-id="d0dd0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0dd0-108">Method</span></span>           | <span data-ttu-id="d0dd0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d0dd0-109">Return Type</span></span>    |<span data-ttu-id="d0dd0-110">説明</span><span class="sxs-lookup"><span data-stu-id="d0dd0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0dd0-111">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="d0dd0-111">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="d0dd0-112">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="d0dd0-112">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="d0dd0-113">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-113">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="d0dd0-114">Update</span><span class="sxs-lookup"><span data-stu-id="d0dd0-114">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="d0dd0-115">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="d0dd0-115">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="d0dd0-116">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-116">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0dd0-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0dd0-117">Properties</span></span>
| <span data-ttu-id="d0dd0-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0dd0-118">Property</span></span>     | <span data-ttu-id="d0dd0-119">種類</span><span class="sxs-lookup"><span data-stu-id="d0dd0-119">Type</span></span>   |<span data-ttu-id="d0dd0-120">説明</span><span class="sxs-lookup"><span data-stu-id="d0dd0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0dd0-121">text</span><span class="sxs-lookup"><span data-stu-id="d0dd0-121">text</span></span>|<span data-ttu-id="d0dd0-122">文字列</span><span class="sxs-lookup"><span data-stu-id="d0dd0-122">string</span></span>|<span data-ttu-id="d0dd0-123">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-123">Represents the axis title.</span></span>|
|<span data-ttu-id="d0dd0-124">visible</span><span class="sxs-lookup"><span data-stu-id="d0dd0-124">visible</span></span>|<span data-ttu-id="d0dd0-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="d0dd0-125">boolean</span></span>|<span data-ttu-id="d0dd0-126">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-126">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0dd0-127">関係</span><span class="sxs-lookup"><span data-stu-id="d0dd0-127">Relationships</span></span>
| <span data-ttu-id="d0dd0-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0dd0-128">Relationship</span></span> | <span data-ttu-id="d0dd0-129">型</span><span class="sxs-lookup"><span data-stu-id="d0dd0-129">Type</span></span>   |<span data-ttu-id="d0dd0-130">説明</span><span class="sxs-lookup"><span data-stu-id="d0dd0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0dd0-131">format</span><span class="sxs-lookup"><span data-stu-id="d0dd0-131">format</span></span>|[<span data-ttu-id="d0dd0-132">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="d0dd0-132">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="d0dd0-p102">グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-p102">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0dd0-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0dd0-135">JSON representation</span></span>

<span data-ttu-id="d0dd0-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0dd0-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
