---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398528"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="eeeea-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eeeea-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="eeeea-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eeeea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eeeea-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeeea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eeeea-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eeeea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeeea-107">オペレーティング システムのバージョンの範囲です。</span><span class="sxs-lookup"><span data-stu-id="eeeea-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="eeeea-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eeeea-108">Properties</span></span>
|<span data-ttu-id="eeeea-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eeeea-109">Property</span></span>|<span data-ttu-id="eeeea-110">型</span><span class="sxs-lookup"><span data-stu-id="eeeea-110">Type</span></span>|<span data-ttu-id="eeeea-111">説明</span><span class="sxs-lookup"><span data-stu-id="eeeea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeeea-112">説明</span><span class="sxs-lookup"><span data-stu-id="eeeea-112">description</span></span>|<span data-ttu-id="eeeea-113">String</span><span class="sxs-lookup"><span data-stu-id="eeeea-113">String</span></span>|<span data-ttu-id="eeeea-114">この範囲 (有効 1702 のビルドなど) の説明</span><span class="sxs-lookup"><span data-stu-id="eeeea-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="eeeea-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="eeeea-115">lowestVersion</span></span>|<span data-ttu-id="eeeea-116">String</span><span class="sxs-lookup"><span data-stu-id="eeeea-116">String</span></span>|<span data-ttu-id="eeeea-117">最小包括的なバージョンをこの範囲に含まれています。</span><span class="sxs-lookup"><span data-stu-id="eeeea-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="eeeea-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="eeeea-118">highestVersion</span></span>|<span data-ttu-id="eeeea-119">String</span><span class="sxs-lookup"><span data-stu-id="eeeea-119">String</span></span>|<span data-ttu-id="eeeea-120">この範囲に含まれている最高の包括的なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="eeeea-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeeea-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eeeea-121">Relationships</span></span>
<span data-ttu-id="eeeea-122">なし</span><span class="sxs-lookup"><span data-stu-id="eeeea-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eeeea-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eeeea-123">JSON Representation</span></span>
<span data-ttu-id="eeeea-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eeeea-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```




