---
title: アイコン リソースの種類
description: セルのアイコンを表します。
ms.openlocfilehash: fd3e0682a7eb73dd4e3286e11d9f9680755db265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068504"
---
# <a name="icon-resource-type"></a><span data-ttu-id="8b7e7-103">アイコン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b7e7-103">Icon resource type</span></span>

> <span data-ttu-id="8b7e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b7e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b7e7-106">セルのアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-106">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="8b7e7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8b7e7-107">Methods</span></span>

| <span data-ttu-id="8b7e7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8b7e7-108">Method</span></span>           | <span data-ttu-id="8b7e7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8b7e7-109">Return Type</span></span>    |<span data-ttu-id="8b7e7-110">説明</span><span class="sxs-lookup"><span data-stu-id="8b7e7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b7e7-111">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="8b7e7-111">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="8b7e7-112">Icon</span><span class="sxs-lookup"><span data-stu-id="8b7e7-112">Icon</span></span>](icon.md) |<span data-ttu-id="8b7e7-113">アイコン オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-113">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="8b7e7-114">Update</span><span class="sxs-lookup"><span data-stu-id="8b7e7-114">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="8b7e7-115">Icon</span><span class="sxs-lookup"><span data-stu-id="8b7e7-115">Icon</span></span>](icon.md)  |<span data-ttu-id="8b7e7-116">アイコン オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-116">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8b7e7-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b7e7-117">Properties</span></span>
| <span data-ttu-id="8b7e7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b7e7-118">Property</span></span>     | <span data-ttu-id="8b7e7-119">型</span><span class="sxs-lookup"><span data-stu-id="8b7e7-119">Type</span></span>   |<span data-ttu-id="8b7e7-120">説明</span><span class="sxs-lookup"><span data-stu-id="8b7e7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b7e7-121">index</span><span class="sxs-lookup"><span data-stu-id="8b7e7-121">index</span></span>|<span data-ttu-id="8b7e7-122">int</span><span class="sxs-lookup"><span data-stu-id="8b7e7-122">int</span></span>|<span data-ttu-id="8b7e7-123">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-123">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="8b7e7-124">set</span><span class="sxs-lookup"><span data-stu-id="8b7e7-124">set</span></span>|<span data-ttu-id="8b7e7-125">文字列</span><span class="sxs-lookup"><span data-stu-id="8b7e7-125">string</span></span>|<span data-ttu-id="8b7e7-p102">アイコンがその一部であるセットを表します。可能な値は、`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes` です。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-p102">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b7e7-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b7e7-128">Relationships</span></span>
<span data-ttu-id="8b7e7-129">なし</span><span class="sxs-lookup"><span data-stu-id="8b7e7-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b7e7-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b7e7-130">JSON representation</span></span>

<span data-ttu-id="8b7e7-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b7e7-131">Here is a JSON representation of the resource.</span></span>

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