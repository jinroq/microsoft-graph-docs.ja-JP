---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2222d7142ea033a8db2c2ce263da04c3b33153
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524555"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="f0f88-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0f88-103">rgbColor resource type</span></span>

> <span data-ttu-id="f0f88-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0f88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0f88-105">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="f0f88-105">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="f0f88-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0f88-106">Properties</span></span>
|<span data-ttu-id="f0f88-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0f88-107">Property</span></span>|<span data-ttu-id="f0f88-108">型</span><span class="sxs-lookup"><span data-stu-id="f0f88-108">Type</span></span>|<span data-ttu-id="f0f88-109">説明</span><span class="sxs-lookup"><span data-stu-id="f0f88-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f88-110">r</span><span class="sxs-lookup"><span data-stu-id="f0f88-110">r</span></span>|<span data-ttu-id="f0f88-111">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="f0f88-111">Byte</span></span>|<span data-ttu-id="f0f88-112">赤の値</span><span class="sxs-lookup"><span data-stu-id="f0f88-112">Red value</span></span>|
|<span data-ttu-id="f0f88-113">g</span><span class="sxs-lookup"><span data-stu-id="f0f88-113">g</span></span>|<span data-ttu-id="f0f88-114">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="f0f88-114">Byte</span></span>|<span data-ttu-id="f0f88-115">緑の値</span><span class="sxs-lookup"><span data-stu-id="f0f88-115">Green value</span></span>|
|<span data-ttu-id="f0f88-116">b</span><span class="sxs-lookup"><span data-stu-id="f0f88-116">b</span></span>|<span data-ttu-id="f0f88-117">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="f0f88-117">Byte</span></span>|<span data-ttu-id="f0f88-118">青の値</span><span class="sxs-lookup"><span data-stu-id="f0f88-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0f88-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0f88-119">Relationships</span></span>
<span data-ttu-id="f0f88-120">なし</span><span class="sxs-lookup"><span data-stu-id="f0f88-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0f88-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0f88-121">JSON Representation</span></span>
<span data-ttu-id="f0f88-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0f88-122">Here is a JSON representation of the resource.</span></span>
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



