---
title: vpnDnsRule リソースの種類
description: VPN DNS ルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 983b30b1f724c3c8f76e967179c6fcdb1ff1fecb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367730"
---
# <a name="vpndnsrule-resource-type"></a>vpnDnsRule リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN DNS ルールの定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|拡張子.|
|サーバ|文字列コレクション|サーバ.|
|proxyServerUri|String|プロキシサーバーの Uri。|
|autoTrigger|Boolean|デバイスがこのドメインに接続されている場合は、自動的に VPN に接続します。既定値は False です。|
|引き続き|Boolean|VPN が接続されていない場合も、このルールをアクティブにします。既定値は False です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```



