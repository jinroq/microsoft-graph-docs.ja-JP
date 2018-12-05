---
title: airPrintDestination リソースの種類
description: AirPrint のリンク先を表します。
ms.openlocfilehash: a1f30f5c71a8ee79bb537ad4ae1f20ce8a05d184
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068803"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

AirPrint のリンク先を表します。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ipAddress|文字列型 (String)|AirPrint の宛先の IP アドレスです。|
|resourcePath|String|プリンターに関連付けられているリソースのパスです。 これは、Bonjour のレコードの _ipps.tcp の rp のパラメーターに対応しています。 例: プリンター/Canon_MG5300_series、プリンター/Xerox_Phaser_7600、ipp 印刷/Epson_IPP_Printer です。|
|port|Int32|AirPrint のリンク先のリッスン ポート。 このキーが既定のポートは AirPrint を使用して、指定されていない場合。 IOS 11.0 で利用可能な後で。|
|forceTls|ブール値|AirPrint 接続の場合は true、トランスポート層セキュリティ (TLS) によって保護されている場合。 既定では false を指定します。 IOS 11.0 で利用可能な後で。|

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




