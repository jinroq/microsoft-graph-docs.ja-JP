---
title: vpnTrafficRule リソースの種類
description: VPN トラフィックの規則の定義です。
author: tfitzmac
ms.openlocfilehash: 39303510fdfef39cbcb99df3f824ce29bcbfd65c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324648"
---
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN トラフィックの規則の定義です。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|名前|String|名前です。|
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





