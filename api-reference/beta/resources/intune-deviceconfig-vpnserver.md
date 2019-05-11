---
title: vpnServer リソースの種類
description: VPN サーバーの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67f0e91c0b2d024a07ab632a5e61e1106bbc65fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944528"
---
# <a name="vpnserver-resource-type"></a>vpnServer リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN サーバーの定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|description|String|説明。|
|address|String|Address (IP アドレス、FQDN または URL)|
|isDefaultServer|Boolean|既定のサーバー。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```




