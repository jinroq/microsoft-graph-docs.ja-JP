---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b0afb706a71ef8e0e3d4877fa7d0df822fe1d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788122"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="5df60-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5df60-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="5df60-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5df60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5df60-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5df60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5df60-106">オペレーティングシステムのバージョンの範囲。</span><span class="sxs-lookup"><span data-stu-id="5df60-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="5df60-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5df60-107">Properties</span></span>
|<span data-ttu-id="5df60-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5df60-108">Property</span></span>|<span data-ttu-id="5df60-109">型</span><span class="sxs-lookup"><span data-stu-id="5df60-109">Type</span></span>|<span data-ttu-id="5df60-110">説明</span><span class="sxs-lookup"><span data-stu-id="5df60-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df60-111">description</span><span class="sxs-lookup"><span data-stu-id="5df60-111">description</span></span>|<span data-ttu-id="5df60-112">String</span><span class="sxs-lookup"><span data-stu-id="5df60-112">String</span></span>|<span data-ttu-id="5df60-113">この範囲の説明 (例: 有効な1702ビルド)</span><span class="sxs-lookup"><span data-stu-id="5df60-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="5df60-114">lowestversion</span><span class="sxs-lookup"><span data-stu-id="5df60-114">lowestVersion</span></span>|<span data-ttu-id="5df60-115">文字列</span><span class="sxs-lookup"><span data-stu-id="5df60-115">String</span></span>|<span data-ttu-id="5df60-116">この範囲に含まれている最小の包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="5df60-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="5df60-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="5df60-117">highestVersion</span></span>|<span data-ttu-id="5df60-118">文字列</span><span class="sxs-lookup"><span data-stu-id="5df60-118">String</span></span>|<span data-ttu-id="5df60-119">この範囲に含まれている最も高い包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="5df60-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df60-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5df60-120">Relationships</span></span>
<span data-ttu-id="5df60-121">なし</span><span class="sxs-lookup"><span data-stu-id="5df60-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5df60-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5df60-122">JSON Representation</span></span>
<span data-ttu-id="5df60-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5df60-123">Here is a JSON representation of the resource.</span></span>
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





