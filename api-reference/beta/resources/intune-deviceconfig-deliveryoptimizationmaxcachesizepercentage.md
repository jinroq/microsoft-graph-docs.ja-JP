---
title: deliveryOptimizationMaxCacheSizePercentage リソースの種類
description: 配信の最適化最大キャッシュサイズの割合の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: adc27f85a4b02adbf5a8a589fd2bd07db0622978
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970725"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="e0c94-103">deliveryOptimizationMaxCacheSizePercentage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0c94-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

> <span data-ttu-id="e0c94-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0c94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0c94-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0c94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0c94-106">配信の最適化最大キャッシュサイズの割合の種類。</span><span class="sxs-lookup"><span data-stu-id="e0c94-106">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="e0c94-107">[DeliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e0c94-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0c94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0c94-108">Properties</span></span>
|<span data-ttu-id="e0c94-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0c94-109">Property</span></span>|<span data-ttu-id="e0c94-110">型</span><span class="sxs-lookup"><span data-stu-id="e0c94-110">Type</span></span>|<span data-ttu-id="e0c94-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0c94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0c94-112">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="e0c94-112">maximumCacheSizePercentage</span></span>|<span data-ttu-id="e0c94-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c94-113">Int32</span></span>|<span data-ttu-id="e0c94-114">配信の最適化で利用できる最大キャッシュサイズを指定します。ディスクサイズの割合 (1-100) で指定します。</span><span class="sxs-lookup"><span data-stu-id="e0c94-114">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="e0c94-115">有効な値は 1 ~ 100</span><span class="sxs-lookup"><span data-stu-id="e0c94-115">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0c94-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0c94-116">Relationships</span></span>
<span data-ttu-id="e0c94-117">なし</span><span class="sxs-lookup"><span data-stu-id="e0c94-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0c94-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0c94-118">JSON Representation</span></span>
<span data-ttu-id="e0c94-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0c94-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```





