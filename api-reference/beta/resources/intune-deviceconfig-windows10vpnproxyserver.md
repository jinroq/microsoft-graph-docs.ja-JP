---
title: windows10VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
author: tfitzmac
ms.openlocfilehash: e21b964ab1bd648cd042a1364ecf5f0942ded085
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309458"
---
# <a name="windows10vpnproxyserver-resource-type"></a>windows10VpnProxyServer リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN プロキシ サーバーです。

[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|プロキシの自動構成スクリプトの url です。 [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。|
|address|String|アドレスです。 [VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。|
|port|Int32|ポートです。 有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承|
|bypassProxyServerForLocalAddress|ブール型|ローカル アドレスに対してプロキシ サーバーをバイパスします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```





