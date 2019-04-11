---
title: vpnOnDemandRule リソースの種類
description: VPN のオンデマンドルールの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3209c91400b36adba772273cfa6768049adce448
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777656"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN のオンデマンドルールの定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ssid|String コレクション|ネットワークサービスセット識別子 (ssid)。|
|dnssearchdomains|String コレクション|DNS 検索ドメイン。|
|probeUrl|文字列|プローブする URL。 リダイレクトされていない (200 HTTP 状態コードを返す) この URL が正常に取得された場合、このルールは一致します。|
|アクション|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Action. 可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。|
|domainaction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|ドメインアクション (アクションが接続を評価する場合にのみ該当)。 可能な値は、`connectIfNeeded`、`neverConnect` です。|
|ドメイン|String コレクション|ドメイン (アクションが接続を評価する場合にのみ該当)。|
|probeRequiredUrl|文字列|必要な Url をプローブします (アクションが接続を評価する場合にのみ適用され、必要に応じて、domainaction が connect である)。|

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





