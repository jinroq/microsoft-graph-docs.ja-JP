# <a name="compliancestate-enum-type"></a>complianceState 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

コンプライアンスの状態です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|unknown|0|不明|
|compliant|1|準拠|
|noncompliant|2|非準拠のデバイスであり、企業リソースからブロックされる|
|conflict|3|他の規則と競合している|
|error|4|エラー|
|inGracePeriod|254|非準拠のデバイスであるが、社内リソースにアクセスできる|
|configManager|255|構成マネージャーがマネージしている|



