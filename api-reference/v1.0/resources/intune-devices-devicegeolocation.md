---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542033"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの場所

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|場所が記録された、UTC を基準とする時刻|
|longitude|倍精度浮動小数点数|デバイスの場所の経度座標|
|latitude|倍精度浮動小数点数|デバイスの場所の緯度座標|
|altitude|倍精度浮動小数点数|海抜標高 (メートル単位)|
|horizontalAccuracy|倍精度浮動小数点数|経度と緯度の精度 (メートル単位)|
|verticalAccuracy|倍精度浮動小数点数|標高の精度 (メートル単位)|
|heading|倍精度浮動小数点数|真北を基準とする方角|
|speed|Double|デバイスの移動速度 (m/秒)|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



