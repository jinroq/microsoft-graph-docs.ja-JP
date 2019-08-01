---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc5d2feb61c731e9b8e80d7b28fec539319f5a9b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037269"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="63dfa-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63dfa-103">rgbColor resource type</span></span>

> <span data-ttu-id="63dfa-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63dfa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63dfa-105">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="63dfa-105">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="63dfa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63dfa-106">Properties</span></span>
|<span data-ttu-id="63dfa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63dfa-107">Property</span></span>|<span data-ttu-id="63dfa-108">型</span><span class="sxs-lookup"><span data-stu-id="63dfa-108">Type</span></span>|<span data-ttu-id="63dfa-109">説明</span><span class="sxs-lookup"><span data-stu-id="63dfa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dfa-110">r</span><span class="sxs-lookup"><span data-stu-id="63dfa-110">r</span></span>|<span data-ttu-id="63dfa-111">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="63dfa-111">Byte</span></span>|<span data-ttu-id="63dfa-112">赤の値</span><span class="sxs-lookup"><span data-stu-id="63dfa-112">Red value</span></span>|
|<span data-ttu-id="63dfa-113">g</span><span class="sxs-lookup"><span data-stu-id="63dfa-113">g</span></span>|<span data-ttu-id="63dfa-114">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="63dfa-114">Byte</span></span>|<span data-ttu-id="63dfa-115">緑の値</span><span class="sxs-lookup"><span data-stu-id="63dfa-115">Green value</span></span>|
|<span data-ttu-id="63dfa-116">b</span><span class="sxs-lookup"><span data-stu-id="63dfa-116">b</span></span>|<span data-ttu-id="63dfa-117">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="63dfa-117">Byte</span></span>|<span data-ttu-id="63dfa-118">青の値</span><span class="sxs-lookup"><span data-stu-id="63dfa-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="63dfa-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="63dfa-119">Relationships</span></span>
<span data-ttu-id="63dfa-120">なし</span><span class="sxs-lookup"><span data-stu-id="63dfa-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63dfa-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63dfa-121">JSON Representation</span></span>
<span data-ttu-id="63dfa-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="63dfa-122">Here is a JSON representation of the resource.</span></span>
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



