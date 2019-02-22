---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6783502079ab3ce3adf3f8133662ab3eab578bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145207"
---
# <a name="windows81vpnproxyserver-resource-type"></a>windows81VpnProxyServer リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN プロキシサーバー。


[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|自動構成 scripturl|String|プロキシの自動構成スクリプトの url。 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。|
|address|String|連絡先. [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。|
|port|Int32|ポート. [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承された有効な値 0 ~ 65535|
|自動的に検出する proxysettings|ブール値|プロキシの設定を自動的に検出します。|
|bypassProxyServerForLocalAddress|ブール値|ローカルアドレスにはプロキシサーバーを使用しないでください。|

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




