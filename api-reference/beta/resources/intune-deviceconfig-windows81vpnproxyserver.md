---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b694206fd65bad46c9176a9fc01586f00237bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834714"
---
# <a name="windows81vpnproxyserver-resource-type"></a>windows81VpnProxyServer リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN プロキシ サーバーです。

[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|プロキシの自動構成スクリプトの url です。 [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。|
|address|String|アドレスです。 [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。|
|port|Int32|ポートです。 有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承|
|automaticallyDetectProxySettings|ブール型|プロキシの設定を自動的に検出します。|
|bypassProxyServerForLocalAddress|ブール型|ローカル アドレスに対してプロキシ サーバーをバイパスします。|

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





