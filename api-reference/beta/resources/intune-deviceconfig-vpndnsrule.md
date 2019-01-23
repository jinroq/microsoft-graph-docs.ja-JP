---
title: vpnDnsRule リソースの種類
description: VPN の DNS ルール定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425583"
---
# <a name="vpndnsrule-resource-type"></a>vpnDnsRule リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN の DNS ルール定義します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|名前です。|
|サーバー|String コレクション|サーバーです。|
|proxyServerUri|String|プロキシ サーバーの Uri。|
|autoTrigger|Boolean|VPN への接続に自動的にデバイスがこのドメインに接続する場合: 既定値は False です。|
|persistent|Boolean|VPN が接続されていない場合でもこの規則をアクティブにしておく既定値は False。|

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




