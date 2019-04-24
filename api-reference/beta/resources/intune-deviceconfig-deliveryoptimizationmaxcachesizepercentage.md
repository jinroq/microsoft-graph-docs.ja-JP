---
title: deliveryOptimizationMaxCacheSizePercentage リソースの種類
description: 配信の最適化最大キャッシュサイズの割合の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f48b85c269da4204b985a19701b9d40a50358e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461207"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>deliveryOptimizationMaxCacheSizePercentage リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

配信の最適化最大キャッシュサイズの割合の種類。


[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|maximumcachesizepercentage|Int32|配信の最適化で利用できる最大キャッシュサイズを指定します。ディスクサイズの割合 (1-100) で指定します。 有効な値は 1 ~ 100|

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





