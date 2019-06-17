---
title: 放映 Printdestination リソースの種類
description: 放映印刷先を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 665e4d5a8e8c3f715150bd81075385a7a6dd8c1a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965775"
---
# <a name="airprintdestination-resource-type"></a>放映 Printdestination リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

放映印刷先を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ipAddress|String|放映される印刷先の IP アドレス。|
|resourcePath|String|プリンターに関連付けられているリソースパス。 これは、(ipBonjour レコードの rp パラメーターに対応します。 例: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer|
|ポート|Int32|放映された印刷先のリスニングポート。 このキーが指定されていない場合、印刷時に既定のポートが使用されます。 IOS 11.0 以降で利用可能です。|
|forceTls|Boolean|True の場合、放送印刷接続はトランスポート層セキュリティ (TLS) によって保護されます。 既定値は false です。 IOS 11.0 以降で利用可能です。|

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





