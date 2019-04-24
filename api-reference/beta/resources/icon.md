---
title: アイコン リソースの種類
description: セルのアイコンを表します。
localization_priority: Normal
ms.openlocfilehash: c15ee02d1c6830cbb5246826665d0353b7e999b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506412"
---
# <a name="icon-resource-type"></a><span data-ttu-id="990d8-103">アイコン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="990d8-103">Icon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="990d8-104">セルのアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="990d8-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="990d8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="990d8-105">Methods</span></span>

| <span data-ttu-id="990d8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="990d8-106">Method</span></span>           | <span data-ttu-id="990d8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="990d8-107">Return Type</span></span>    |<span data-ttu-id="990d8-108">説明</span><span class="sxs-lookup"><span data-stu-id="990d8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="990d8-109">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="990d8-109">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="990d8-110">Icon</span><span class="sxs-lookup"><span data-stu-id="990d8-110">Icon</span></span>](icon.md) |<span data-ttu-id="990d8-111">アイコン オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="990d8-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="990d8-112">Update</span><span class="sxs-lookup"><span data-stu-id="990d8-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="990d8-113">Icon</span><span class="sxs-lookup"><span data-stu-id="990d8-113">Icon</span></span>](icon.md)  |<span data-ttu-id="990d8-114">アイコン オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="990d8-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="990d8-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="990d8-115">Properties</span></span>
| <span data-ttu-id="990d8-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="990d8-116">Property</span></span>     | <span data-ttu-id="990d8-117">型</span><span class="sxs-lookup"><span data-stu-id="990d8-117">Type</span></span>   |<span data-ttu-id="990d8-118">説明</span><span class="sxs-lookup"><span data-stu-id="990d8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="990d8-119">index</span><span class="sxs-lookup"><span data-stu-id="990d8-119">index</span></span>|<span data-ttu-id="990d8-120">int</span><span class="sxs-lookup"><span data-stu-id="990d8-120">int</span></span>|<span data-ttu-id="990d8-121">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="990d8-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="990d8-122">set</span><span class="sxs-lookup"><span data-stu-id="990d8-122">set</span></span>|<span data-ttu-id="990d8-123">string</span><span class="sxs-lookup"><span data-stu-id="990d8-123">string</span></span>|<span data-ttu-id="990d8-p101">アイコンがその一部であるセットを表します。可能な値は、`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes` です。</span><span class="sxs-lookup"><span data-stu-id="990d8-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="990d8-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="990d8-126">Relationships</span></span>
<span data-ttu-id="990d8-127">なし</span><span class="sxs-lookup"><span data-stu-id="990d8-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="990d8-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="990d8-128">JSON representation</span></span>

<span data-ttu-id="990d8-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="990d8-129">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/icon.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
