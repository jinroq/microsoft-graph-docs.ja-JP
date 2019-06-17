---
title: deliveryOptimizationBandwidthAbsolute リソースの種類
description: 帯域幅制限 (キロバイト/秒)。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 626c46c035ec4a7af44c06a31f7269cde96a2b8b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979719"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>deliveryOptimizationBandwidthAbsolute リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

帯域幅制限 (キロバイト/秒)。


[DeliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|配信の最適化を使用して、すべての同時ダウンロードアクティビティでデバイスが使用できる最大ダウンロード帯域幅をキロバイト/秒で指定します。 有効な値は 0 ~ 4294967295
値 0 (ゼロ) は、配信の最適化が、ダウンロードに使用可能な帯域幅を使用するように動的に調整されることを意味します。 有効な値は 0 ~ 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|配信の最適化 (0-4000000) を使用して、デバイスがすべての同時アップロードアクティビティで使用する最大アップロード帯域幅 (キロバイト/秒) を指定します。 有効な値は 0 ~ 400万
既定値は0で、無制限に可能な帯域幅を許可します (アップロード帯域幅の使用を最小限にするために最適化されています)。 有効な値は 0 ~ 400万|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```





