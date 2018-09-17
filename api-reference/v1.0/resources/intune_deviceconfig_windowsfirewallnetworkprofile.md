# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ファイアウォールのプロファイルのポリシーです。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|ホスト ・ デバイスを許可またはブロックするファイアウォールとネットワークのプロファイルの高度なセキュリティの強制を構成します。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|stealthModeBlocked|ブール値|サーバーがステルス モードで動作するのを防ぎます StealthModeRequired と StealthModeBlocked の両方が true の場合、StealthModeBlocked が優先します。|
|incomingTrafficBlocked|ブール値|他のポリシーの設定に関係なく、すべての受信トラフィックをブロックするようにファイアウォールを構成します IncomingTrafficRequired と IncomingTrafficBlocked の両方が true の場合、IncomingTrafficBlocked が優先します。|
|unicastResponsesToMulticastBroadcastsBlocked|ブール値|マルチキャスト ブロードキャスト トラフィックへのユニキャスト応答をブロックするようにファイアウォールを構成します UnicastResponsesToMulticastBroadcastsRequired と UnicastResponsesToMulticastBroadcastsBlocked の両方が true の場合、UnicastResponsesToMulticastBroadcastsBlocked が優先します。|
|inboundNotificationsBlocked|ブール値|アプリケーションがポートでリッスンしないようにブロックされているときに、ファイアウォールによる通知を表示しないようにします InboundNotificationsRequired と InboundNotificationsBlocked の両方が true の場合、InboundNotificationsBlocked が優先します。|
|authorizedApplicationRulesFromGroupPolicyMerged|ブール値|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからの承認済みのアプリケーションに関する規則とローカル ストアからの規則を統合するように構成します AuthorizedApplicationRulesFromGroupPolicyNotMerged と AuthorizedApplicationRulesFromGroupPolicyMerged の両方が true の場合、AuthorizedApplicationRulesFromGroupPolicyMerged が優先します。|
|globalPortRulesFromGroupPolicyMerged|ブール値|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからのグローバル ポートの規則と、ローカル ストアからの規則を統合するように構成します GlobalPortRulesFromGroupPolicyNotMerged と GlobalPortRulesFromGroupPolicyMerged の両方が true の場合、GlobalPortRulesFromGroupPolicyMerged が優先します。|
|connectionSecurityRulesFromGroupPolicyMerged|ブール値|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからの接続セキュリティの規則と、ローカル ストアからの規則を統合するように構成します ConnectionSecurityRulesFromGroupPolicyNotMerged と ConnectionSecurityRulesFromGroupPolicyMerged の両方が true の場合、ConnectionSecurityRulesFromGroupPolicyMerged が優先します。|
|outboundConnectionsBlocked|ブール値|既定で、ファイアウォールがすべての送信接続をブロックするように構成します OutboundConnectionsRequired と OutboundConnectionsBlocked の両方が true の場合、OutboundConnectionsBlocked が優先します。|
|inboundConnectionsBlocked|ブール値|既定で、ファイアウォールがすべての受信接続をブロックするように構成します InboundConnectionsRequired と InboundConnectionsBlocked の両方が true の場合、InboundConnectionsBlocked が優先します。|
|securedPacketExemptionAllowed|ブール値|stealthModeBlocked が true に設定されている場合でも、ホスト コンピューターが要請していないネットワーク トラフィックに応答し、トラフィックが IPSec によって保護されるように、ファイアウォールを構成します SecuredPacketExemptionBlocked と SecuredPacketExemptionAllowed の両方が true の場合、SecuredPacketExemptionAllowed が優先します。|
|policyRulesFromGroupPolicyMerged|ブール値|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからのファイアウォール規則のポリシーと、ローカル ストアからのポリシーを統合するように構成します PolicyRulesFromGroupPolicyNotMerged と PolicyRulesFromGroupPolicyMerged の両方が true の場合、PolicyRulesFromGroupPolicyMerged が優先します。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}-->
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








