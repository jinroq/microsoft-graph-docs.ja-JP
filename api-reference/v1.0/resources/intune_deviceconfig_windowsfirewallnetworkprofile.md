# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ファイアウォールのプロファイルのポリシーです。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|ファイアウォールと高度なセキュリティの実行をオンにします。 可能な値は、 `notConfigured`、`blocked`、`allowed` です。|
|stealthModeBlocked|Boolean|サーバーがステルス モードで動作するのを防ぎます|
|incomingTrafficBlocked|Boolean|他のポリシーの設定に関係なく、すべての受信トラフィックをブロックするようにファイアウォールを構成します|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|マルチキャスト ブロードキャスト トラフィックへのユニキャスト応答をブロックするようにファイアウォールを構成します|
|inboundNotificationsBlocked|Boolean|アプリケーションがポートでリッスンしないようにブロックされているときに、ファイアウォールによる通知を表示しないようにします|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからの承認済みのアプリケーションに関する規則とローカル ストアからの規則を統合するように構成します|
|globalPortRulesFromGroupPolicyMerged|Boolean|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからのグローバル ポートの規則と、ローカル ストアからの規則を統合するように構成します|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからの接続セキュリティの規則と、ローカル ストアからの規則を統合するように構成します|
|outboundConnectionsBlocked|Boolean|既定で、ファイアウォールがすべての送信接続をブロックするように構成します|
|inboundConnectionsBlocked|Boolean|既定で、ファイアウォールがすべての受信接続をブロックするように構成します|
|securedPacketExemptionAllowed|Boolean|stealthModeBlocked が true に設定されている場合でも、ホスト コンピューターが要請していないネットワーク トラフィックに応答し、トラフィックが IPSec によって保護されるように、ファイアウォールを構成します|
|policyRulesFromGroupPolicyMerged|Boolean|ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからのファイアウォール規則のポリシーと、ローカル ストアからのポリシーを統合するように構成します|

## <a name="relationships"></a>リレーションシップ
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



