---
title: vpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8a452cdde7c4c360107a67396d8f5ce49d6eb1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145277"
---
# <a name="vpnproxyserver-resource-type"></a>vpnProxyServer リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN プロキシサーバー。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|自動構成 scripturl|String|プロキシの自動構成スクリプトの url。|
|address|String|連絡先.|
|port|Int32|ポート. 有効な値は 0 ~ 65535|

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




