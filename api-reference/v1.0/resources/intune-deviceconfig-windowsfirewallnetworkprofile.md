---
title: windowsFirewallNetworkProfile リソース タイプ
description: Windows ファイアウォールのプロファイルのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e30f01031d46babf066b6778edf7801de7eac46c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917963"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ファイアウォールのプロファイルのポリシーです。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|ホスト ・ デバイスを許可またはブロックするファイアウォールとネットワークのプロファイルの高度なセキュリティの強制を構成します。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|stealthModeBlocked|Boolean|サーバーがステルス ・ モードで動作するを防ぐ。 StealthModeRequired と StealthModeBlocked の両方が true の場合、StealthModeBlocked が優先します。|
|incomingTrafficBlocked|Boolean|その他のポリシー設定に関係なくすべての着信トラフィックをブロックするファイアウォールを構成します。 IncomingTrafficRequired と IncomingTrafficBlocked の両方が true の場合、IncomingTrafficBlocked が優先します。|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|マルチキャスト ブロードキャスト トラフィックへのユニキャスト応答をブロックするファイアウォールを構成します。 UnicastResponsesToMulticastBroadcastsRequired と UnicastResponsesToMulticastBroadcastsBlocked の両方が true の場合、UnicastResponsesToMulticastBroadcastsBlocked が優先します。|
|inboundNotificationsBlocked|Boolean|ファイアウォールがからのポートでリッスンしているアプリケーションがブロックされたときに通知を表示するを防ぎます。 InboundNotificationsRequired と InboundNotificationsBlocked の両方が true の場合、InboundNotificationsBlocked が優先します。|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーの承認済みのアプリケーションの規則をマージするようにファイアウォールを構成します。 AuthorizedApplicationRulesFromGroupPolicyNotMerged と AuthorizedApplicationRulesFromGroupPolicyMerged の両方が true の場合、AuthorizedApplicationRulesFromGroupPolicyMerged が優先します。|
|globalPortRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーからグローバルなポートの規則をマージするようにファイアウォールを構成します。 GlobalPortRulesFromGroupPolicyNotMerged と GlobalPortRulesFromGroupPolicyMerged の両方が true の場合、GlobalPortRulesFromGroupPolicyMerged が優先します。|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーからの接続セキュリティの規則をマージするようにファイアウォールを構成します。 ConnectionSecurityRulesFromGroupPolicyNotMerged と ConnectionSecurityRulesFromGroupPolicyMerged の両方が true の場合、ConnectionSecurityRulesFromGroupPolicyMerged が優先します。|
|outboundConnectionsBlocked|Boolean|既定ですべての送信接続をブロックするファイアウォールを構成します。 OutboundConnectionsRequired と OutboundConnectionsBlocked の両方が true の場合、OutboundConnectionsBlocked が優先します。|
|inboundConnectionsBlocked|Boolean|既定ですべての着信接続をブロックするファイアウォールを構成します。 InboundConnectionsRequired と InboundConnectionsBlocked の両方が true の場合、InboundConnectionsBlocked が優先します。|
|securedPacketExemptionAllowed|Boolean|StealthModeBlocked を設定した場合でも、トラフィックが IPSec でセキュリティ保護するの一方的なネットワーク トラフィックに応答するホスト コンピューターを許可するファイアウォールの設定を true にします。 SecuredPacketExemptionBlocked と SecuredPacketExemptionAllowed の両方が true の場合、SecuredPacketExemptionAllowed が優先します。|
|policyRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーからポリシーをファイアウォールの規則をマージするようにファイアウォールを構成します。 PolicyRulesFromGroupPolicyNotMerged と PolicyRulesFromGroupPolicyMerged の両方が true の場合、PolicyRulesFromGroupPolicyMerged が優先します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeBlocked": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "policyRulesFromGroupPolicyMerged": true
}
```



