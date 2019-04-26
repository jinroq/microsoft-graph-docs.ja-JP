---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5ca085d009f38a2879074d7ee95a78acddf0f4a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572935"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="b9673-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9673-103">rgbColor resource type</span></span>

> <span data-ttu-id="b9673-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9673-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9673-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9673-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9673-106">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="b9673-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="b9673-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9673-107">Properties</span></span>
|<span data-ttu-id="b9673-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9673-108">Property</span></span>|<span data-ttu-id="b9673-109">型</span><span class="sxs-lookup"><span data-stu-id="b9673-109">Type</span></span>|<span data-ttu-id="b9673-110">説明</span><span class="sxs-lookup"><span data-stu-id="b9673-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9673-111">r</span><span class="sxs-lookup"><span data-stu-id="b9673-111">r</span></span>|<span data-ttu-id="b9673-112">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="b9673-112">Byte</span></span>|<span data-ttu-id="b9673-113">赤の値</span><span class="sxs-lookup"><span data-stu-id="b9673-113">Red value</span></span>|
|<span data-ttu-id="b9673-114">g</span><span class="sxs-lookup"><span data-stu-id="b9673-114">g</span></span>|<span data-ttu-id="b9673-115">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="b9673-115">Byte</span></span>|<span data-ttu-id="b9673-116">緑の値</span><span class="sxs-lookup"><span data-stu-id="b9673-116">Green value</span></span>|
|<span data-ttu-id="b9673-117">b</span><span class="sxs-lookup"><span data-stu-id="b9673-117">b</span></span>|<span data-ttu-id="b9673-118">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="b9673-118">Byte</span></span>|<span data-ttu-id="b9673-119">青の値</span><span class="sxs-lookup"><span data-stu-id="b9673-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9673-120">関係</span><span class="sxs-lookup"><span data-stu-id="b9673-120">Relationships</span></span>
<span data-ttu-id="b9673-121">なし</span><span class="sxs-lookup"><span data-stu-id="b9673-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9673-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9673-122">JSON Representation</span></span>
<span data-ttu-id="b9673-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9673-123">Here is a JSON representation of the resource.</span></span>
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





