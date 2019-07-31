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
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>deliveryOptimizationMaxCacheSizePercentage リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

配信の最適化最大キャッシュサイズの割合の種類。


[DeliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|maximumCacheSizePercentage|Int32|配信の最適化で利用できる最大キャッシュサイズを指定します。ディスクサイズの割合 (1-100) で指定します。 有効な値は 1 ~ 100|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
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





