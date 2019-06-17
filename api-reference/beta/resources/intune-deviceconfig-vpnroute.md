---
title: vpnRoute リソースの種類
description: VPN ルートの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89b07a6f58bcd8ce5159c5bec07d01d2beea9fdd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987538"
---
# <a name="vpnroute-resource-type"></a>vpnRoute リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN ルートの定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|destinationPrefix|String|宛先プレフィックス (IPv4/v6 アドレス)。|
|prefixSize|Int32|プレフィックスのサイズです。 (1-32)。 有効な値は 1 ~ 32|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```





