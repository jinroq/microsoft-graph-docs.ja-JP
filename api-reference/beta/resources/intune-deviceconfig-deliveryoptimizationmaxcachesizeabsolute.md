---
title: deliveryOptimizationMaxCacheSizeAbsolute リソースの種類
description: 配信の最適化最大キャッシュサイズ絶対種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97d5c076051aed4fd905ef147f7adbd14168bc29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970732"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="748c1-103">deliveryOptimizationMaxCacheSizeAbsolute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="748c1-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="748c1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="748c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="748c1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="748c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="748c1-106">配信の最適化最大キャッシュサイズ絶対種類。</span><span class="sxs-lookup"><span data-stu-id="748c1-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="748c1-107">[DeliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="748c1-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="748c1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="748c1-108">Properties</span></span>
|<span data-ttu-id="748c1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="748c1-109">Property</span></span>|<span data-ttu-id="748c1-110">型</span><span class="sxs-lookup"><span data-stu-id="748c1-110">Type</span></span>|<span data-ttu-id="748c1-111">説明</span><span class="sxs-lookup"><span data-stu-id="748c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748c1-112">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="748c1-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="748c1-113">Int64</span><span class="sxs-lookup"><span data-stu-id="748c1-113">Int64</span></span>|<span data-ttu-id="748c1-114">配信最適化キャッシュの最大サイズを GB 単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="748c1-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="748c1-115">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="748c1-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="748c1-116">値 0 (ゼロ) は、"無制限" キャッシュを意味します。</span><span class="sxs-lookup"><span data-stu-id="748c1-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="748c1-117">配信の最適化では、デバイスのディスク領域が不足しているときにキャッシュがクリアされます。</span><span class="sxs-lookup"><span data-stu-id="748c1-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="748c1-118">有効な値は 0 ~ 4294967295</span><span class="sxs-lookup"><span data-stu-id="748c1-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="748c1-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="748c1-119">Relationships</span></span>
<span data-ttu-id="748c1-120">なし</span><span class="sxs-lookup"><span data-stu-id="748c1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="748c1-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="748c1-121">JSON Representation</span></span>
<span data-ttu-id="748c1-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="748c1-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```





