---
title: windowsFirewallNetworkProfile リソース タイプ
description: Windows ファイアウォールのプロファイルのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae504c8224be18766da49108a3b80c5aecb48b71
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149778"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ファイアウォールのプロファイルのポリシーです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|firewallEnabled|[statemanagementsetting](../resources/intune-deviceconfig-statemanagementsetting.md)|ネットワークプロファイルに対するファイアウォールと高度なセキュリティの適用を許可またはブロックするようにホストデバイスを構成します。 可能な値は `notConfigured`、`blocked`、`allowed` です。|
|stealthModeRequired|Boolean|サーバーがステルスモードで動作することを許可します。 StealthModeRequired と StealthModeBlocked の両方が true の場合、StealthModeBlocked は優先されます。|
|stealthModeBlocked|Boolean|サーバーがステルスモードで動作しないようにします。 StealthModeRequired と StealthModeBlocked の両方が true の場合、StealthModeBlocked は優先されます。|
|incomingTrafficRequired|Boolean|他のポリシー設定に従って着信トラフィックを許可するようにファイアウォールを構成します。 IncomingTrafficRequired と IncomingTrafficBlocked の両方が true の場合、IncomingTrafficBlocked は優先されます。|
|incomingTrafficBlocked|Boolean|他のポリシー設定に関係なく、すべての着信トラフィックをブロックするようにファイアウォールを構成します。 IncomingTrafficRequired と IncomingTrafficBlocked の両方が true の場合、IncomingTrafficBlocked は優先されます。|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|マルチキャストブロードキャストトラフィックへのユニキャスト応答を許可するようにファイアウォールを構成します。 UnicastResponsesToMulticastBroadcastsRequired と UnicastResponsesToMulticastBroadcastsBlocked の両方が true の場合、UnicastResponsesToMulticastBroadcastsBlocked は優先されます。|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|マルチキャストブロードキャストトラフィックへのユニキャスト応答をブロックするようにファイアウォールを構成します。 UnicastResponsesToMulticastBroadcastsRequired と UnicastResponsesToMulticastBroadcastsBlocked の両方が true の場合、UnicastResponsesToMulticastBroadcastsBlocked は優先されます。|
|inboundNotificationsRequired|Boolean|アプリケーションがポートでリッスンできない場合に、ファイアウォールで通知を表示できるようにします。 InboundNotificationsRequired と InboundNotificationsBlocked の両方が true の場合、InboundNotificationsBlocked は優先されます。|
|inboundNotificationsBlocked|Boolean|アプリケーションがポートでリッスンできない場合に、ファイアウォールで通知が表示されないようにします。 InboundNotificationsRequired と InboundNotificationsBlocked の両方が true の場合、InboundNotificationsBlocked は優先されます。|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|ローカルストアの規則を無視するのではなく、承認されたアプリケーションルールをローカルストアからマージするように、ファイアウォールを構成します。 authorizedapplicationrulesfromgrouppolicynotmerged と authorizedapplicationpolicyfromgrouppolicyマージの両方が true である場合、authorizedapplicationpolicyfromgrouppolicyマージが優先されます。|
|authorizedapplicationルール fromgrouppolicynotマージ|Boolean|ローカルストアのルールを無視するのではなく、ローカルストアからの承認済みアプリケーションルールをマージしないように、ファイアウォールを構成します。 authorizedapplicationrulesfromgrouppolicynotmerged と authorizedapplicationpolicyfromgrouppolicyマージの両方が true である場合、authorizedapplicationpolicyfromgrouppolicyマージが優先されます。|
|globalPortRulesFromGroupPolicyMerged|Boolean|ローカルストアの規則を無視するのではなく、グループポリシーからグローバルポートの規則をローカルストアからマージするように、ファイアウォールを構成します。 globalportrulesfromgrouppolicynotmerged と globalportrulesfromgrouppolicyマージの両方が true の場合、globalportrulesfromgrouppolicyマージが優先されます。|
|globalportrulesfromgrouppolicynotmerged|Boolean|ローカルストアの規則を無視するのではなく、グローバルポートの規則をローカルストアからのグループポリシーにマージしないように、ファイアウォールを構成します。 globalportrulesfromgrouppolicynotmerged と globalportrulesfromgrouppolicyマージの両方が true の場合、globalportrulesfromgrouppolicyマージが優先されます。|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|ローカルストアの規則を無視するのではなく、グループポリシーから接続セキュリティの規則をローカルストアからマージするようにファイアウォールを構成します。 connectionsecurityrulesfromgrouppolicynotmerged と connectionsecuritypolicyfromgrouppolicyマージの両方が true の場合、connectionsecuritypolicyfromgrouppolicyマージが優先されます。|
|connectionsecurityルール fromgrouppolicynotマージ|Boolean|ローカルストアの規則を無視するのではなく、グループポリシーから接続セキュリティの規則をローカルストアから除外することができないように、ファイアウォールを構成します。 connectionsecurityrulesfromgrouppolicynotmerged と connectionsecuritypolicyfromgrouppolicyマージの両方が true の場合、connectionsecuritypolicyfromgrouppolicyマージが優先されます。|
|outboundConnectionsRequired|Boolean|既定ですべての送信接続を許可するようにファイアウォールを構成します。 OutboundConnectionsRequired と OutboundConnectionsBlocked の両方が true の場合、OutboundConnectionsBlocked は優先されます。|
|outboundConnectionsBlocked|Boolean|既定ですべての送信接続をブロックするようにファイアウォールを構成します。 OutboundConnectionsRequired と OutboundConnectionsBlocked の両方が true の場合、OutboundConnectionsBlocked は優先されます。|
|inboundConnectionsRequired|Boolean|既定ですべての受信接続を許可するようにファイアウォールを構成します。 InboundConnectionsRequired と InboundConnectionsBlocked の両方が true の場合、InboundConnectionsBlocked は優先されます。|
|inboundConnectionsBlocked|Boolean|既定ですべての受信接続をブロックするようにファイアウォールを構成します。 InboundConnectionsRequired と InboundConnectionsBlocked の両方が true の場合、InboundConnectionsBlocked は優先されます。|
|securedPacketExemptionAllowed|Boolean|stealthModeBlocked が true に設定されている場合でも、そのトラフィックの一方的なネットワークトラフィックにホストコンピューターが応答できるように、ファイアウォールを構成します。 SecuredPacketExemptionBlocked と SecuredPacketExemptionAllowed の両方が true の場合、SecuredPacketExemptionAllowed は優先されます。|
|securedPacketExemptionBlocked|Boolean|stealthModeBlocked が true に設定されている場合でも、そのトラフィックの一方的なネットワークトラフィックに対してホストコンピューターが応答するのをブロックするようにファイアウォールを構成します。 SecuredPacketExemptionBlocked と SecuredPacketExemptionAllowed の両方が true の場合、SecuredPacketExemptionAllowed は優先されます。|
|policyRulesFromGroupPolicyMerged|Boolean|ファイアウォールが、ローカルストアの規則を無視するのではなく、グループポリシーから、ローカルストアからのものと一緒に、ファイアウォールの規則ポリシーをマージするように構成します。 policyrulesfromgrouppolicynotmerged と policypolicyfromgrouppolicyマージの両方が true の場合、policypolicyfromgrouppolicy統合が優先されます。|
|policy規則 fromgrouppolicynot合併|Boolean|ファイアウォールを構成して、ローカルストアの規則を無視するのではなく、グループポリシーからのファイアウォール規則ポリシーとローカルストアの規則をマージしないようにします。 policyrulesfromgrouppolicynotmerged と policypolicyfromgrouppolicyマージの両方が true の場合、policypolicyfromgrouppolicy統合が優先されます。|

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




