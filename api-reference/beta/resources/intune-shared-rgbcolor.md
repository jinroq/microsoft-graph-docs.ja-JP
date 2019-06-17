---
title: rgbColor リソースの種類
description: RGB 色。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b515627dab47d05915ddc167c62d367723a46ce
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986285"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="79768-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79768-103">rgbColor resource type</span></span>

> <span data-ttu-id="79768-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79768-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79768-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79768-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79768-106">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="79768-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="79768-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79768-107">Properties</span></span>
|<span data-ttu-id="79768-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79768-108">Property</span></span>|<span data-ttu-id="79768-109">型</span><span class="sxs-lookup"><span data-stu-id="79768-109">Type</span></span>|<span data-ttu-id="79768-110">説明</span><span class="sxs-lookup"><span data-stu-id="79768-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79768-111">r</span><span class="sxs-lookup"><span data-stu-id="79768-111">r</span></span>|<span data-ttu-id="79768-112">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="79768-112">Byte</span></span>|<span data-ttu-id="79768-113">赤の値</span><span class="sxs-lookup"><span data-stu-id="79768-113">Red value</span></span>|
|<span data-ttu-id="79768-114">g</span><span class="sxs-lookup"><span data-stu-id="79768-114">g</span></span>|<span data-ttu-id="79768-115">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="79768-115">Byte</span></span>|<span data-ttu-id="79768-116">緑の値</span><span class="sxs-lookup"><span data-stu-id="79768-116">Green value</span></span>|
|<span data-ttu-id="79768-117">b</span><span class="sxs-lookup"><span data-stu-id="79768-117">b</span></span>|<span data-ttu-id="79768-118">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="79768-118">Byte</span></span>|<span data-ttu-id="79768-119">青の値</span><span class="sxs-lookup"><span data-stu-id="79768-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="79768-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79768-120">Relationships</span></span>
<span data-ttu-id="79768-121">なし</span><span class="sxs-lookup"><span data-stu-id="79768-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79768-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79768-122">JSON Representation</span></span>
<span data-ttu-id="79768-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79768-123">Here is a JSON representation of the resource.</span></span>
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





