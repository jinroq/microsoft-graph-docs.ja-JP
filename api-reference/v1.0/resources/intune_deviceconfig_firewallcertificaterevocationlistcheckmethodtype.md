# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

FirewallCertificateRevocationListCheckMethod に対して使用可能な値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|値は Intune により未構成、ユーザーにより構成されたデバイスの規定値を上書きしないでください。|
|なし|1|証明書失効リストをチェックしないでください。|
|試行|2|CRL（証明書失効リスト）チェックを試行し、証明書がチェックにより確認される場合のみ証明書を許可|
|要求|3|証明書を許可する前に正常な CRL チェックを要求|








