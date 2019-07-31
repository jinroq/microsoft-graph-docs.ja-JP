---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d94d120fcedd6ef086002895f7364f78f5ef3579
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969913"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="94b11-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94b11-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="94b11-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94b11-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94b11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94b11-106">オペレーティングシステムのバージョンの範囲。</span><span class="sxs-lookup"><span data-stu-id="94b11-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="94b11-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94b11-107">Properties</span></span>
|<span data-ttu-id="94b11-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94b11-108">Property</span></span>|<span data-ttu-id="94b11-109">型</span><span class="sxs-lookup"><span data-stu-id="94b11-109">Type</span></span>|<span data-ttu-id="94b11-110">説明</span><span class="sxs-lookup"><span data-stu-id="94b11-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b11-111">description</span><span class="sxs-lookup"><span data-stu-id="94b11-111">description</span></span>|<span data-ttu-id="94b11-112">String</span><span class="sxs-lookup"><span data-stu-id="94b11-112">String</span></span>|<span data-ttu-id="94b11-113">この範囲の説明 (例: 有効な1702ビルド)</span><span class="sxs-lookup"><span data-stu-id="94b11-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="94b11-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="94b11-114">lowestVersion</span></span>|<span data-ttu-id="94b11-115">String</span><span class="sxs-lookup"><span data-stu-id="94b11-115">String</span></span>|<span data-ttu-id="94b11-116">この範囲に含まれている最小の包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="94b11-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="94b11-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="94b11-117">highestVersion</span></span>|<span data-ttu-id="94b11-118">String</span><span class="sxs-lookup"><span data-stu-id="94b11-118">String</span></span>|<span data-ttu-id="94b11-119">この範囲に含まれている最も高い包括バージョン。</span><span class="sxs-lookup"><span data-stu-id="94b11-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94b11-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="94b11-120">Relationships</span></span>
<span data-ttu-id="94b11-121">なし</span><span class="sxs-lookup"><span data-stu-id="94b11-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94b11-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94b11-122">JSON Representation</span></span>
<span data-ttu-id="94b11-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="94b11-123">Here is a JSON representation of the resource.</span></span>
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





