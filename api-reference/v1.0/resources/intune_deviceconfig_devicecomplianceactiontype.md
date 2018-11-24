# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

列挙型の操作をスケジュールします。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAction|0|操作は必要ありません。|
|通知|1|通知を送信します。|
|ブロック|2|AAD でデバイスをブロックします。|
|退職|3|デバイスを破棄します。|
|ワイプ|4|デバイスをワイプします。|
|removeResourceAccessProfiles|5|デバイスからリソースのアクセス ・ プロファイルを削除します。|
|pushNotification|9|デバイスにプッシュ通知を送信します。|



