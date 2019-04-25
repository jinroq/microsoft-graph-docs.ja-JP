---
title: アイコン リソースの種類
description: セルのアイコンを表します。
localization_priority: Normal
ms.openlocfilehash: 833fa4cb4061a96b01077c3adeb7dcaed49e0a02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567810"
---
# <a name="icon-resource-type"></a><span data-ttu-id="bdb1b-103">アイコン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdb1b-103">Icon resource type</span></span>

<span data-ttu-id="bdb1b-104">セルのアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="bdb1b-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="bdb1b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bdb1b-105">Methods</span></span>

| <span data-ttu-id="bdb1b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bdb1b-106">Method</span></span>           | <span data-ttu-id="bdb1b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bdb1b-107">Return Type</span></span>    |<span data-ttu-id="bdb1b-108">説明</span><span class="sxs-lookup"><span data-stu-id="bdb1b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdb1b-109">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="bdb1b-109">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="bdb1b-110">Icon</span><span class="sxs-lookup"><span data-stu-id="bdb1b-110">Icon</span></span>](icon.md) |<span data-ttu-id="bdb1b-111">アイコン オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bdb1b-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="bdb1b-112">Update</span><span class="sxs-lookup"><span data-stu-id="bdb1b-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="bdb1b-113">Icon</span><span class="sxs-lookup"><span data-stu-id="bdb1b-113">Icon</span></span>](icon.md)  |<span data-ttu-id="bdb1b-114">アイコン オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bdb1b-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bdb1b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdb1b-115">Properties</span></span>
| <span data-ttu-id="bdb1b-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdb1b-116">Property</span></span>     | <span data-ttu-id="bdb1b-117">型</span><span class="sxs-lookup"><span data-stu-id="bdb1b-117">Type</span></span>   |<span data-ttu-id="bdb1b-118">説明</span><span class="sxs-lookup"><span data-stu-id="bdb1b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdb1b-119">index</span><span class="sxs-lookup"><span data-stu-id="bdb1b-119">index</span></span>|<span data-ttu-id="bdb1b-120">int</span><span class="sxs-lookup"><span data-stu-id="bdb1b-120">int</span></span>|<span data-ttu-id="bdb1b-121">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="bdb1b-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="bdb1b-122">set</span><span class="sxs-lookup"><span data-stu-id="bdb1b-122">set</span></span>|<span data-ttu-id="bdb1b-123">string</span><span class="sxs-lookup"><span data-stu-id="bdb1b-123">string</span></span>|<span data-ttu-id="bdb1b-124">アイコンがその一部であるセットを表します。</span><span class="sxs-lookup"><span data-stu-id="bdb1b-124">Represents the set that the icon is part of.</span></span> <span data-ttu-id="bdb1b-125">使用可能な値は`Invalid`次`ThreeArrows`の`ThreeArrowsGray`とおり`ThreeFlags`です`ThreeTrafficLights1`。 `ThreeTrafficLights2`、 `ThreeSigns` `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` `FourTrafficLights` `FiveQuarters`、、、、、、、、、、、、 `ThreeStars` `FiveArrows` `FiveArrowsGray` `FiveRating`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="bdb1b-125">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdb1b-126">関係</span><span class="sxs-lookup"><span data-stu-id="bdb1b-126">Relationships</span></span>
<span data-ttu-id="bdb1b-127">なし</span><span class="sxs-lookup"><span data-stu-id="bdb1b-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bdb1b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdb1b-128">JSON representation</span></span>

<span data-ttu-id="bdb1b-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bdb1b-129">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
