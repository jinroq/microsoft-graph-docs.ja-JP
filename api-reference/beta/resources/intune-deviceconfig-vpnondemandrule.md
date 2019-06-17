---
title: vpnOnDemandRule リソースの種類
description: VPN のオンデマンドルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa1ac8562ac2a43db43bb359cb189f8a4ed9500b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987580"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN のオンデマンドルールの定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ssid|文字列コレクション|ネットワークサービスセット識別子 (Ssid)。|
|dnsSearchDomains|文字列コレクション|DNS 検索ドメイン。|
|probeUrl|String|プローブする URL。 リダイレクトされていない (200 HTTP 状態コードを返す) この URL が正常に取得された場合、このルールは一致します。|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Action. 使用可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|ドメインアクション (アクションが接続を評価する場合にのみ該当)。 可能な値は、`connectIfNeeded`、`neverConnect` です。|
|ドメイン|文字列コレクション|ドメイン (アクションが接続を評価する場合にのみ該当)。|
|probeRequiredUrl|String|必要な Url をプローブします (アクションが接続を評価する場合にのみ適用され、必要に応じて、DomainAction が connect である)。|

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





