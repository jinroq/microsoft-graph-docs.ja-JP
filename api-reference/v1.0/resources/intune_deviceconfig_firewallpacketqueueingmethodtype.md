# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

FirewallPacketQueueingMethod に指定できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|値は Intune により未構成、ユーザーにより構成されたデバイスの規定値を上書きしないでください。|
|無効|1|パケットのキューを無効にします|
|queueInbound|2|キューが暗号化されたパケットを受信|
|queueOutbound|3|キューは、転送のためのアウトバウンド パケットを復号化|
|queueBoth|4|着信および発信パケットをキューします|








