---
title: deviceGeoLocation リソースの種類
description: デバイスの場所
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395056"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの場所

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|場所が記録された、UTC を基準とする時刻|
|lastCollectedDateTime|DateTimeOffset|場所が記録された、UTC を基準とする時刻|
|longitude|Double|デバイスの場所の経度座標|
|latitude|Double|デバイスの場所の緯度座標|
|altitude|Double|海抜標高 (メートル単位)|
|horizontalAccuracy|Double|経度と緯度の精度 (メートル単位)|
|verticalAccuracy|Double|標高の精度 (メートル単位)|
|heading|Double|真北を基準とする方角|
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




