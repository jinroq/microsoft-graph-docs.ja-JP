---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521f7d0b0ec4ddab728ed3b95c27acf21695b0d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148609"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="348ed-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="348ed-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="348ed-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="348ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="348ed-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="348ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="348ed-106">オペレーティングシステムのバージョンの範囲。</span><span class="sxs-lookup"><span data-stu-id="348ed-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="348ed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="348ed-107">Properties</span></span>
|<span data-ttu-id="348ed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="348ed-108">Property</span></span>|<span data-ttu-id="348ed-109">型</span><span class="sxs-lookup"><span data-stu-id="348ed-109">Type</span></span>|<span data-ttu-id="348ed-110">説明</span><span class="sxs-lookup"><span data-stu-id="348ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="348ed-111">説明</span><span class="sxs-lookup"><span data-stu-id="348ed-111">description</span></span>|<span data-ttu-id="348ed-112">String</span><span class="sxs-lookup"><span data-stu-id="348ed-112">String</span></span>|<span data-ttu-id="348ed-113">この範囲の説明 (例: 有効な1702ビルド)</span><span class="sxs-lookup"><span data-stu-id="348ed-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="348ed-114">lowestversion</span><span class="sxs-lookup"><span data-stu-id="348ed-114">lowestVersion</span></span>|<span data-ttu-id="348ed-115">String</span><span class="sxs-lookup"><span data-stu-id="348ed-115">String</span></span>|<span data-ttu-id="348ed-116">この範囲に含まれている最小の包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="348ed-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="348ed-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="348ed-117">highestVersion</span></span>|<span data-ttu-id="348ed-118">String</span><span class="sxs-lookup"><span data-stu-id="348ed-118">String</span></span>|<span data-ttu-id="348ed-119">この範囲に含まれている最も高い包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="348ed-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="348ed-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="348ed-120">Relationships</span></span>
<span data-ttu-id="348ed-121">なし</span><span class="sxs-lookup"><span data-stu-id="348ed-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="348ed-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="348ed-122">JSON Representation</span></span>
<span data-ttu-id="348ed-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="348ed-123">Here is a JSON representation of the resource.</span></span>
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




