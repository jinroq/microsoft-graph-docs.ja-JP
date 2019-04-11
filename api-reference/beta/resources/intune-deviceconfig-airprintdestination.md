---
title: 放映 printdestination リソースの種類
description: 放映印刷先を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3218a40ee1a735cef585866e1ca0c9f80ad95671
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779973"
---
# <a name="airprintdestination-resource-type"></a>放映 printdestination リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

放映印刷先を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ipAddress|String|放映される印刷先の IP アドレス。|
|resourcePath|文字列|プリンターに関連付けられているリソースパス。 これは、(ipBonjour レコードの rp パラメーターに対応します。 例: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer|
|ポート|Int32|放映された印刷先のリスニングポート。 このキーが指定されていない場合、印刷時に既定のポートが使用されます。 iOS 11.0 以降で利用可能です。|
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





