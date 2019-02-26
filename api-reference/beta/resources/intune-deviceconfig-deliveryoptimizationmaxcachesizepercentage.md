---
title: deliveryOptimizationMaxCacheSizePercentage リソースの種類
description: 配信の最適化最大キャッシュサイズの割合の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7579b95d0adefb09c9312596f4604fe9d5b05548
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177834"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="4e29d-103">deliveryOptimizationMaxCacheSizePercentage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e29d-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

> <span data-ttu-id="4e29d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e29d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e29d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e29d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e29d-106">配信の最適化最大キャッシュサイズの割合の種類。</span><span class="sxs-lookup"><span data-stu-id="4e29d-106">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="4e29d-107">[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4e29d-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e29d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e29d-108">Properties</span></span>
|<span data-ttu-id="4e29d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e29d-109">Property</span></span>|<span data-ttu-id="4e29d-110">型</span><span class="sxs-lookup"><span data-stu-id="4e29d-110">Type</span></span>|<span data-ttu-id="4e29d-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e29d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e29d-112">maximumcachesizepercentage</span><span class="sxs-lookup"><span data-stu-id="4e29d-112">maximumCacheSizePercentage</span></span>|<span data-ttu-id="4e29d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4e29d-113">Int32</span></span>|<span data-ttu-id="4e29d-114">配信の最適化で利用できる最大キャッシュサイズを指定します。ディスクサイズの割合 (1-100) で指定します。</span><span class="sxs-lookup"><span data-stu-id="4e29d-114">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="4e29d-115">有効な値は 1 ~ 100</span><span class="sxs-lookup"><span data-stu-id="4e29d-115">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e29d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e29d-116">Relationships</span></span>
<span data-ttu-id="4e29d-117">なし</span><span class="sxs-lookup"><span data-stu-id="4e29d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e29d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e29d-118">JSON Representation</span></span>
<span data-ttu-id="4e29d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e29d-119">Here is a JSON representation of the resource.</span></span>
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




