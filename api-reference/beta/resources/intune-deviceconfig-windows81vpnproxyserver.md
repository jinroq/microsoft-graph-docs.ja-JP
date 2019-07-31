---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 035bbe9511692a7244e4cdc2d0b707c5edfb4146
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969101"
---
# <a name="windows81vpnproxyserver-resource-type"></a>windows81VpnProxyServer リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN プロキシサーバー。


[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|自動構成 Scripturl|String|プロキシの自動構成スクリプトの url。 [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。|
|address|String|連絡先. [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。|
|ポート|Int32|ポート. [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承された有効な値 0 ~ 65535|
|自動的に検出する Proxysettings|Boolean|プロキシの設定を自動的に検出します。|
|bypassProxyServerForLocalAddress|Boolean|ローカルアドレスにはプロキシサーバーを使用しないでください。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```





