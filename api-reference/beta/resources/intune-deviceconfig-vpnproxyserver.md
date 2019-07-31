---
title: vpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9aa15cd1ccf7e299be97d52073924258efd069d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969451"
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





