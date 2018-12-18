---
title: vpnOnDemandRule リソースの種類
description: VPN オンデマンド ルール定義します。
author: tfitzmac
ms.openlocfilehash: 72b85971dc9c613026bb9e720ca55165845e0c9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352193"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN オンデマンド ルール定義します。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ssid|String コレクション|ネットワーク サービスでは、識別子 (Ssid) を設定します。|
|dnsSearchDomains|String コレクション|DNS ドメインを検索します。|
|probeUrl|String|プローブへの URL です。 この URL は、正常に場合、リダイレクトには、(HTTP ステータス コード 200 を返す) をフェッチ、この規則に一致します。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|アクションです。 可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|ドメインのアクション (アクションは、接続を評価するときにのみ該当する)。 使用可能な値は、`connectIfNeeded`、`neverConnect` です。|
|ドメイン|String コレクション|(操作は、接続を評価するときにのみ該当する) のドメインです。|
|probeRequiredUrl|String|(操作は、接続を評価し、必要な場合に DomainAction を接続するときにのみ該当する) が必要な Url をプローブします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```





