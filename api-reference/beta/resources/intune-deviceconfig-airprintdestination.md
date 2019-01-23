---
title: airPrintDestination リソースの種類
description: AirPrint のリンク先を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422496"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AirPrint のリンク先を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ipAddress|文字列型 (String)|AirPrint の宛先の IP アドレスです。|
|resourcePath|String|プリンターに関連付けられているリソースのパスです。 これは、Bonjour のレコードの _ipps.tcp の rp のパラメーターに対応しています。 例: プリンター/Canon_MG5300_series、プリンター/Xerox_Phaser_7600、ipp 印刷/Epson_IPP_Printer です。|
|port|Int32|AirPrint のリンク先のリッスン ポート。 このキーが既定のポートは AirPrint を使用して、指定されていない場合。 IOS 11.0 で利用可能な後で。|
|forceTls|Boolean|AirPrint 接続の場合は true、トランスポート層セキュリティ (TLS) によって保護されている場合。 既定では false を指定します。 IOS 11.0 で利用可能な後で。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




