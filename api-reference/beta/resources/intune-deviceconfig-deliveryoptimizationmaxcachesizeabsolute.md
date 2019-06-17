---
title: deliveryOptimizationMaxCacheSizeAbsolute リソースの種類
description: 配信の最適化最大キャッシュサイズ絶対種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfeb2e4279e9858f9fd8f923657c8e32bf129396
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979586"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>deliveryOptimizationMaxCacheSizeAbsolute リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

配信の最適化最大キャッシュサイズ絶対種類。


[DeliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|配信最適化キャッシュの最大サイズを GB 単位で指定します。 有効な値は 0 ~ 4294967295
値 0 (ゼロ) は、"無制限" キャッシュを意味します。 配信の最適化では、デバイスのディスク領域が不足しているときにキャッシュがクリアされます。 有効な値は 0 ~ 4294967295|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
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





