---
title: vpnRoute リソースの種類
description: VPN ルートの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffa3569d8d1a769779201cf056de07c80594b68e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944545"
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

## <a name="relationships"></a>関係
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




