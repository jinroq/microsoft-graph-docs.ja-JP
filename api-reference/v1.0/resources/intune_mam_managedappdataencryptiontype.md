# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

マネージ アプリのデータの暗号化レベルを示します
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useDeviceSettings|0|アプリのデータはデバイスのデフォルト設定に基づき暗号化されている|
|afterDeviceRestart|1|アプリのデータはデバイスを再起動すると暗号化される|
|whenDeviceLockedExceptOpenFiles|2|このポリシーに関連付けられたアプリのデータは、オープンしているファイルのデータを除き、デバイスがロックされると暗号化される|
|whenDeviceLocked|3|このポリシーに関連付けられたアプリのデータは、デバイスがロックされると暗号化される|



