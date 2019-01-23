---
title: vpnTrafficRule リソースの種類
description: VPN トラフィックの規則の定義です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415286"
---
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN トラフィックの規則の定義です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|名前です。|
|プロトコル|Int32|(0 ~ 255) のプロトコル。 0 から 255 までの有効な値|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション|プロトコルが TCP または UDP 6 (17) である場合にのみ、ローカル ポートの範囲を設定できます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション|プロトコルが TCP または UDP 6 (17) である場合にのみ、リモート ポートの範囲を設定できます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション|ローカル アドレスの範囲です。 このコレクションには、最大で 500 個の要素を含めることができます。|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション|リモート アドレスの範囲です。 このコレクションには、最大で 500 個の要素を含めることができます。|
|appId|文字列型 (String)|アプリケーション識別子、アプリケーションでこのトラフィック ルールがトリガーされる場合です。|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|アプリケーションの種類、アプリケーションでこのトラフィック ルールがトリガーされる場合。 可能な値は、`none`、`desktop`、`universal` です。|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|いつトリガーされると、アプリケーションでは、このルートの分割トンネリングを有効にするかどうかを示します。 可能な値は、`none`、`splitTunnel`、`forceTunnel` です。|
|クレーム|String|このトラフィックの規則に関連付けられている請求します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```




