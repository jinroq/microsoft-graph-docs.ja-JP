---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7fe455bc0e934e08b858a084009ac5c8364a673
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950964"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="382e4-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="382e4-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="382e4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="382e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="382e4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="382e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="382e4-106">オペレーティングシステムのバージョンの範囲。</span><span class="sxs-lookup"><span data-stu-id="382e4-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="382e4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="382e4-107">Properties</span></span>
|<span data-ttu-id="382e4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="382e4-108">Property</span></span>|<span data-ttu-id="382e4-109">型</span><span class="sxs-lookup"><span data-stu-id="382e4-109">Type</span></span>|<span data-ttu-id="382e4-110">説明</span><span class="sxs-lookup"><span data-stu-id="382e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="382e4-111">description</span><span class="sxs-lookup"><span data-stu-id="382e4-111">description</span></span>|<span data-ttu-id="382e4-112">String</span><span class="sxs-lookup"><span data-stu-id="382e4-112">String</span></span>|<span data-ttu-id="382e4-113">この範囲の説明 (例: 有効な1702ビルド)</span><span class="sxs-lookup"><span data-stu-id="382e4-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="382e4-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="382e4-114">lowestVersion</span></span>|<span data-ttu-id="382e4-115">String</span><span class="sxs-lookup"><span data-stu-id="382e4-115">String</span></span>|<span data-ttu-id="382e4-116">この範囲に含まれている最小の包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="382e4-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="382e4-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="382e4-117">highestVersion</span></span>|<span data-ttu-id="382e4-118">String</span><span class="sxs-lookup"><span data-stu-id="382e4-118">String</span></span>|<span data-ttu-id="382e4-119">この範囲に含まれている最も高い包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="382e4-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="382e4-120">関係</span><span class="sxs-lookup"><span data-stu-id="382e4-120">Relationships</span></span>
<span data-ttu-id="382e4-121">なし</span><span class="sxs-lookup"><span data-stu-id="382e4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="382e4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="382e4-122">JSON Representation</span></span>
<span data-ttu-id="382e4-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="382e4-123">Here is a JSON representation of the resource.</span></span>
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




