---
title: windowsFirewallNetworkProfile リソース タイプ
description: Windows ファイアウォールのプロファイルのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 21feca83653e9c72b43fdd2fe0e510bb5a563e64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984368"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ファイアウォールのプロファイルのポリシーです。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|ホスト ・ デバイスを許可またはブロックするファイアウォールとネットワークのプロファイルの高度なセキュリティの強制を構成します。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|stealthModeRequired|ブール型|ステルス ・ モードで動作するサーバーを許可します。 StealthModeRequired と StealthModeBlocked の両方が true の場合、StealthModeBlocked が優先します。|
|stealthModeBlocked|Boolean|サーバーがステルス ・ モードで動作するを防ぐ。 StealthModeRequired と StealthModeBlocked の両方が true の場合、StealthModeBlocked が優先します。|
|incomingTrafficRequired|ブール型|その他のポリシーの設定に基づいて受信トラフィックを許可するファイアウォールを構成します。 IncomingTrafficRequired と IncomingTrafficBlocked の両方が true の場合、IncomingTrafficBlocked が優先します。|
|incomingTrafficBlocked|Boolean|その他のポリシー設定に関係なくすべての着信トラフィックをブロックするファイアウォールを構成します。 IncomingTrafficRequired と IncomingTrafficBlocked の両方が true の場合、IncomingTrafficBlocked が優先します。|
|unicastResponsesToMulticastBroadcastsRequired|ブール型|マルチキャスト ブロードキャスト トラフィックに対するユニキャスト応答を許可するファイアウォールを構成します。 UnicastResponsesToMulticastBroadcastsRequired と UnicastResponsesToMulticastBroadcastsBlocked の両方が true の場合、UnicastResponsesToMulticastBroadcastsBlocked が優先します。|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|マルチキャスト ブロードキャスト トラフィックへのユニキャスト応答をブロックするファイアウォールを構成します。 UnicastResponsesToMulticastBroadcastsRequired と UnicastResponsesToMulticastBroadcastsBlocked の両方が true の場合、UnicastResponsesToMulticastBroadcastsBlocked が優先します。|
|inboundNotificationsRequired|ブール型|ポートをリッスンしているアプリケーションがブロックされたときに通知を表示するようにファイアウォールを使用できます。 InboundNotificationsRequired と InboundNotificationsBlocked の両方が true の場合、InboundNotificationsBlocked が優先します。|
|inboundNotificationsBlocked|Boolean|ファイアウォールがからのポートでリッスンしているアプリケーションがブロックされたときに通知を表示するを防ぎます。 InboundNotificationsRequired と InboundNotificationsBlocked の両方が true の場合、InboundNotificationsBlocked が優先します。|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーの承認済みのアプリケーションの規則をマージするようにファイアウォールを構成します。 AuthorizedApplicationRulesFromGroupPolicyNotMerged と AuthorizedApplicationRulesFromGroupPolicyMerged の両方が true の場合、AuthorizedApplicationRulesFromGroupPolicyMerged が優先します。|
|authorizedApplicationRulesFromGroupPolicyNotMerged|ブール型|承認済みのアプリケーションの結合を防ぐためにファイアウォールを構成するローカルを無視するのではなくローカル ストアからのグループ ポリシーからのルールがルールを保存します。 AuthorizedApplicationRulesFromGroupPolicyNotMerged と AuthorizedApplicationRulesFromGroupPolicyMerged の両方が true の場合、AuthorizedApplicationRulesFromGroupPolicyMerged が優先します。|
|globalPortRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーからグローバルなポートの規則をマージするようにファイアウォールを構成します。 GlobalPortRulesFromGroupPolicyNotMerged と GlobalPortRulesFromGroupPolicyMerged の両方が true の場合、GlobalPortRulesFromGroupPolicyMerged が優先します。|
|globalPortRulesFromGroupPolicyNotMerged|ブール型|グループ ポリシーとローカル ストアの規則を無視するのではなくローカル ストアからのグローバル ポートの規則のマージを防ぐためにファイアウォールを構成します。 GlobalPortRulesFromGroupPolicyNotMerged と GlobalPortRulesFromGroupPolicyMerged の両方が true の場合、GlobalPortRulesFromGroupPolicyMerged が優先します。|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーからの接続セキュリティの規則をマージするようにファイアウォールを構成します。 ConnectionSecurityRulesFromGroupPolicyNotMerged と ConnectionSecurityRulesFromGroupPolicyMerged の両方が true の場合、ConnectionSecurityRulesFromGroupPolicyMerged が優先します。|
|connectionSecurityRulesFromGroupPolicyNotMerged|ブール型|結合を防ぐためにファイアウォールを構成するローカルを無視するのではなくローカル ストアからのグループ ポリシーからの接続セキュリティの規則は、規則を保存します。 ConnectionSecurityRulesFromGroupPolicyNotMerged と ConnectionSecurityRulesFromGroupPolicyMerged の両方が true の場合、ConnectionSecurityRulesFromGroupPolicyMerged が優先します。|
|outboundConnectionsRequired|ブール型|既定ですべての送信接続を許可するファイアウォールを構成します。 OutboundConnectionsRequired と OutboundConnectionsBlocked の両方が true の場合、OutboundConnectionsBlocked が優先します。|
|outboundConnectionsBlocked|Boolean|既定ですべての送信接続をブロックするファイアウォールを構成します。 OutboundConnectionsRequired と OutboundConnectionsBlocked の両方が true の場合、OutboundConnectionsBlocked が優先します。|
|inboundConnectionsRequired|ブール型|既定ですべての着信接続を許可するファイアウォールを構成します。 InboundConnectionsRequired と InboundConnectionsBlocked の両方が true の場合、InboundConnectionsBlocked が優先します。|
|inboundConnectionsBlocked|Boolean|既定ですべての着信接続をブロックするファイアウォールを構成します。 InboundConnectionsRequired と InboundConnectionsBlocked の両方が true の場合、InboundConnectionsBlocked が優先します。|
|securedPacketExemptionAllowed|Boolean|StealthModeBlocked を設定した場合でも、トラフィックが IPSec でセキュリティ保護するの一方的なネットワーク トラフィックに応答するホスト コンピューターを許可するファイアウォールの設定を true にします。 SecuredPacketExemptionBlocked と SecuredPacketExemptionAllowed の両方が true の場合、SecuredPacketExemptionAllowed が優先します。|
|securedPacketExemptionBlocked|ブール型|StealthModeBlocked を設定した場合でも、トラフィックが IPSec でセキュリティ保護するの一方的なネットワーク トラフィックに応答するホスト コンピューターをブロックするファイアウォールの設定を true にします。 SecuredPacketExemptionBlocked と SecuredPacketExemptionAllowed の両方が true の場合、SecuredPacketExemptionAllowed が優先します。|
|policyRulesFromGroupPolicyMerged|Boolean|ローカル ストアの規則を無視するのではなくローカル ストアからのグループ ポリシーからポリシーをファイアウォールの規則をマージするようにファイアウォールを構成します。 PolicyRulesFromGroupPolicyNotMerged と PolicyRulesFromGroupPolicyMerged の両方が true の場合、PolicyRulesFromGroupPolicyMerged が優先します。|
|policyRulesFromGroupPolicyNotMerged|ブール型|ファイアウォール規則のマージを防ぐためにファイアウォールが構成され、ローカルを無視するのではなくローカル ストアからのグループ ポリシーからのポリシー ルールを格納します。 PolicyRulesFromGroupPolicyNotMerged と PolicyRulesFromGroupPolicyMerged の両方が true の場合、PolicyRulesFromGroupPolicyMerged が優先します。|

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
  "stealthModeRequired": true,
  "stealthModeBlocked": true,
  "incomingTrafficRequired": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsRequired": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsRequired": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyNotMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyNotMerged": true,
  "outboundConnectionsRequired": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsRequired": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "securedPacketExemptionBlocked": true,
  "policyRulesFromGroupPolicyMerged": true,
  "policyRulesFromGroupPolicyNotMerged": true
}
```





