---
title: vpnOnDemandRule リソースの種類
description: VPN のオンデマンドルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb17bb1ec1af12f89ea1ab5470cf6a2d808868c4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944587"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN のオンデマンドルールの定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ssid|String collection|ネットワークサービスセット識別子 (Ssid)。|
|dnsSearchDomains|String collection|DNS 検索ドメイン。|
|probeUrl|String|プローブする URL。 リダイレクトされていない (200 HTTP 状態コードを返す) この URL が正常に取得された場合、このルールは一致します。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Action. 使用可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|ドメインアクション (アクションが接続を評価する場合にのみ該当)。 可能な値は、`connectIfNeeded`、`neverConnect` です。|
|ドメイン|String collection|ドメイン (アクションが接続を評価する場合にのみ該当)。|
|probeRequiredUrl|String|必要な Url をプローブします (アクションが接続を評価する場合にのみ適用され、必要に応じて、DomainAction が connect である)。|

## <a name="relationships"></a>関係
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




