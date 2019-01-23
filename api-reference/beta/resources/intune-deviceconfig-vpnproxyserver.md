---
title: vpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425674"
---
# <a name="vpnproxyserver-resource-type"></a>vpnProxyServer リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN プロキシ サーバーです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|プロキシの自動構成スクリプトの url です。|
|address|String|アドレスです。|
|port|Int32|ポートです。 0 から 65535 までの有効な値|

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




