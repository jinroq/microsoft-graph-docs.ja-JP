---
title: rgbColor リソースの種類
description: RGB 色。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 505383227d1014f779cb558d43c18da29d3989aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395518"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="ee4d3-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee4d3-103">rgbColor resource type</span></span>

> <span data-ttu-id="ee4d3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee4d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee4d3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee4d3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee4d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee4d3-107">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="ee4d3-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="ee4d3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee4d3-108">Properties</span></span>
|<span data-ttu-id="ee4d3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee4d3-109">Property</span></span>|<span data-ttu-id="ee4d3-110">型</span><span class="sxs-lookup"><span data-stu-id="ee4d3-110">Type</span></span>|<span data-ttu-id="ee4d3-111">説明</span><span class="sxs-lookup"><span data-stu-id="ee4d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee4d3-112">r</span><span class="sxs-lookup"><span data-stu-id="ee4d3-112">r</span></span>|<span data-ttu-id="ee4d3-113">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="ee4d3-113">Byte</span></span>|<span data-ttu-id="ee4d3-114">赤の値</span><span class="sxs-lookup"><span data-stu-id="ee4d3-114">Red value</span></span>|
|<span data-ttu-id="ee4d3-115">g</span><span class="sxs-lookup"><span data-stu-id="ee4d3-115">g</span></span>|<span data-ttu-id="ee4d3-116">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="ee4d3-116">Byte</span></span>|<span data-ttu-id="ee4d3-117">緑の値</span><span class="sxs-lookup"><span data-stu-id="ee4d3-117">Green value</span></span>|
|<span data-ttu-id="ee4d3-118">b</span><span class="sxs-lookup"><span data-stu-id="ee4d3-118">b</span></span>|<span data-ttu-id="ee4d3-119">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="ee4d3-119">Byte</span></span>|<span data-ttu-id="ee4d3-120">青の値</span><span class="sxs-lookup"><span data-stu-id="ee4d3-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee4d3-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee4d3-121">Relationships</span></span>
<span data-ttu-id="ee4d3-122">なし</span><span class="sxs-lookup"><span data-stu-id="ee4d3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee4d3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee4d3-123">JSON Representation</span></span>
<span data-ttu-id="ee4d3-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee4d3-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```




