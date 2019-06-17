---
title: vpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8fabc24daad5c13a1d62405ec6ca73843ccd12d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987545"
---
# <a name="vpnproxyserver-resource-type"></a>vpnProxyServer リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN プロキシサーバー。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|自動構成 Scripturl|String|プロキシの自動構成スクリプトの url。|
|address|String|連絡先.|
|ポート|Int32|ポート. 有効な値は 0 ~ 65535|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





