---
title: workbookIcon リソースの種類
description: セルのアイコンを表します。
localization_priority: Normal
ms.openlocfilehash: dae8d9c050dfa8e5ce9c27b7c3d1933a733239e4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348896"
---
# <a name="workbookicon-resource-type"></a><span data-ttu-id="318b7-103">workbookIcon リソースの種類</span><span class="sxs-lookup"><span data-stu-id="318b7-103">workbookIcon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="318b7-104">セルのアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="318b7-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="318b7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="318b7-105">Methods</span></span>

| <span data-ttu-id="318b7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="318b7-106">Method</span></span>           | <span data-ttu-id="318b7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="318b7-107">Return Type</span></span>    |<span data-ttu-id="318b7-108">説明</span><span class="sxs-lookup"><span data-stu-id="318b7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="318b7-109">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="318b7-109">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="318b7-110">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="318b7-110">workbookIcon</span></span>](workbookicon.md) |<span data-ttu-id="318b7-111">アイコン オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="318b7-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="318b7-112">Update</span><span class="sxs-lookup"><span data-stu-id="318b7-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="318b7-113">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="318b7-113">workbookIcon</span></span>](workbookicon.md)  |<span data-ttu-id="318b7-114">アイコン オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="318b7-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="318b7-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="318b7-115">Properties</span></span>
| <span data-ttu-id="318b7-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="318b7-116">Property</span></span>     | <span data-ttu-id="318b7-117">型</span><span class="sxs-lookup"><span data-stu-id="318b7-117">Type</span></span>   |<span data-ttu-id="318b7-118">説明</span><span class="sxs-lookup"><span data-stu-id="318b7-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="318b7-119">index</span><span class="sxs-lookup"><span data-stu-id="318b7-119">index</span></span>|<span data-ttu-id="318b7-120">int</span><span class="sxs-lookup"><span data-stu-id="318b7-120">int</span></span>|<span data-ttu-id="318b7-121">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="318b7-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="318b7-122">set</span><span class="sxs-lookup"><span data-stu-id="318b7-122">set</span></span>|<span data-ttu-id="318b7-123">string</span><span class="sxs-lookup"><span data-stu-id="318b7-123">string</span></span>|<span data-ttu-id="318b7-p101">アイコンがその一部であるセットを表します。可能な値は、`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes` です。</span><span class="sxs-lookup"><span data-stu-id="318b7-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="318b7-126">関係</span><span class="sxs-lookup"><span data-stu-id="318b7-126">Relationships</span></span>
<span data-ttu-id="318b7-127">なし</span><span class="sxs-lookup"><span data-stu-id="318b7-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="318b7-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="318b7-128">JSON representation</span></span>

<span data-ttu-id="318b7-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="318b7-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
