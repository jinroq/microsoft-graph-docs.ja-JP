---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e58d4dfe1e75b4b37333e29858ce93d1383f75a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155679"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="dca58-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dca58-103">rgbColor resource type</span></span>

> <span data-ttu-id="dca58-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dca58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dca58-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dca58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca58-106">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="dca58-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="dca58-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca58-107">Properties</span></span>
|<span data-ttu-id="dca58-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca58-108">Property</span></span>|<span data-ttu-id="dca58-109">型</span><span class="sxs-lookup"><span data-stu-id="dca58-109">Type</span></span>|<span data-ttu-id="dca58-110">説明</span><span class="sxs-lookup"><span data-stu-id="dca58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca58-111">r</span><span class="sxs-lookup"><span data-stu-id="dca58-111">r</span></span>|<span data-ttu-id="dca58-112">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="dca58-112">Byte</span></span>|<span data-ttu-id="dca58-113">赤の値</span><span class="sxs-lookup"><span data-stu-id="dca58-113">Red value</span></span>|
|<span data-ttu-id="dca58-114">g</span><span class="sxs-lookup"><span data-stu-id="dca58-114">g</span></span>|<span data-ttu-id="dca58-115">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="dca58-115">Byte</span></span>|<span data-ttu-id="dca58-116">緑の値</span><span class="sxs-lookup"><span data-stu-id="dca58-116">Green value</span></span>|
|<span data-ttu-id="dca58-117">b</span><span class="sxs-lookup"><span data-stu-id="dca58-117">b</span></span>|<span data-ttu-id="dca58-118">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="dca58-118">Byte</span></span>|<span data-ttu-id="dca58-119">青の値</span><span class="sxs-lookup"><span data-stu-id="dca58-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca58-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dca58-120">Relationships</span></span>
<span data-ttu-id="dca58-121">なし</span><span class="sxs-lookup"><span data-stu-id="dca58-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dca58-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dca58-122">JSON Representation</span></span>
<span data-ttu-id="dca58-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dca58-123">Here is a JSON representation of the resource.</span></span>
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




