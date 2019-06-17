---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44c4b6285bc291001c35a5dd0d9580596599247f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983107"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの場所

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|場所が記録された、UTC を基準とする時刻|
|lastCollectedDateTime|DateTimeOffset|場所が記録された、UTC を基準とする時刻|
|longitude|倍精度浮動小数点数|デバイスの場所の経度座標|
|latitude|2 行分|デバイスの場所の緯度座標|
|altitude|2 行分|海抜標高 (メートル単位)|
|horizontalAccuracy|2 行分|経度と緯度の精度 (メートル単位)|
|verticalAccuracy|2 行分|標高の精度 (メートル単位)|
|heading|2 行分|真北を基準とする方角|
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
  "lastCollectedDateTimeUtc": "String (timestamp)",
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





