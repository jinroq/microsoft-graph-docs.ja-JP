---
title: アイコン リソースの種類
description: セルのアイコンを表します。
localization_priority: Normal
ms.openlocfilehash: e1b31632884c757d40be4a7c9639933439028382
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861692"
---
# <a name="icon-resource-type"></a><span data-ttu-id="268bb-103">アイコン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="268bb-103">Icon resource type</span></span>

> <span data-ttu-id="268bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="268bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="268bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="268bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="268bb-106">セルのアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="268bb-106">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="268bb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="268bb-107">Methods</span></span>

| <span data-ttu-id="268bb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="268bb-108">Method</span></span>           | <span data-ttu-id="268bb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="268bb-109">Return Type</span></span>    |<span data-ttu-id="268bb-110">説明</span><span class="sxs-lookup"><span data-stu-id="268bb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="268bb-111">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="268bb-111">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="268bb-112">Icon</span><span class="sxs-lookup"><span data-stu-id="268bb-112">Icon</span></span>](icon.md) |<span data-ttu-id="268bb-113">アイコン オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="268bb-113">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="268bb-114">Update</span><span class="sxs-lookup"><span data-stu-id="268bb-114">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="268bb-115">Icon</span><span class="sxs-lookup"><span data-stu-id="268bb-115">Icon</span></span>](icon.md)  |<span data-ttu-id="268bb-116">アイコン オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="268bb-116">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="268bb-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="268bb-117">Properties</span></span>
| <span data-ttu-id="268bb-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="268bb-118">Property</span></span>     | <span data-ttu-id="268bb-119">種類</span><span class="sxs-lookup"><span data-stu-id="268bb-119">Type</span></span>   |<span data-ttu-id="268bb-120">説明</span><span class="sxs-lookup"><span data-stu-id="268bb-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="268bb-121">index</span><span class="sxs-lookup"><span data-stu-id="268bb-121">index</span></span>|<span data-ttu-id="268bb-122">int</span><span class="sxs-lookup"><span data-stu-id="268bb-122">int</span></span>|<span data-ttu-id="268bb-123">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="268bb-123">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="268bb-124">set</span><span class="sxs-lookup"><span data-stu-id="268bb-124">set</span></span>|<span data-ttu-id="268bb-125">文字列</span><span class="sxs-lookup"><span data-stu-id="268bb-125">string</span></span>|<span data-ttu-id="268bb-p102">アイコンがその一部であるセットを表します。可能な値は、`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes` です。</span><span class="sxs-lookup"><span data-stu-id="268bb-p102">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="268bb-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="268bb-128">Relationships</span></span>
<span data-ttu-id="268bb-129">なし</span><span class="sxs-lookup"><span data-stu-id="268bb-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="268bb-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="268bb-130">JSON representation</span></span>

<span data-ttu-id="268bb-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="268bb-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.icon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
