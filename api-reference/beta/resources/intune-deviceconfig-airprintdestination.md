---
title: 放映 printdestination リソースの種類
description: 放映印刷先を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09301bd791b5fd8b3fa430b50f7cdf58de43944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167334"
---
# <a name="airprintdestination-resource-type"></a>放映 printdestination リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

放映印刷先を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ipAddress|String|放映される印刷先の IP アドレス。|
|resourcePath|String|プリンターに関連付けられているリソースパス。 これは、(ipBonjour レコードの rp パラメーターに対応します。 例: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer|
|port|Int32|放映された印刷先のリスニングポート。 このキーが指定されていない場合、印刷時に既定のポートが使用されます。 iOS 11.0 以降で利用可能です。|
|forcetls|Boolean|true の場合、放送印刷接続はトランスポート層セキュリティ (TLS) によって保護されます。 既定値は false です。 iOS 11.0 以降で利用可能です。|

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




