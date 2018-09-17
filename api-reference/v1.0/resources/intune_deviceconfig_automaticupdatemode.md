# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

自動更新モードを使用可能な値です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義済み、既定値、目的なし。|
|notifyDownload|1|ダウンロード時に通知。|
|autoInstallAtMaintenanceTime|2|メンテナンス時に自動インストール。|
|autoInstallAndRebootAtMaintenanceTime|3|メンテナンス時に自動インストールと再起動。|
|autoInstallAndRebootAtScheduledTime|4|設定時刻に自動インストールと再起動。|
|autoInstallAndRebootWithoutEndUserControl|5|エンド ユーザーによる操作なしに自動インストールと再起動。|








