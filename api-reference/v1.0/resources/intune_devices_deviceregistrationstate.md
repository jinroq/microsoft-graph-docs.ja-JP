# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス登録のステータス。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notRegistered|0|デバイスは登録されていません。|
|登録済み|2|デバイスが登録されています。|
|破棄|3|デバイスがブロックされている、消去されている、または廃止されています。|
|keyConflict|4|デバイスに重大な競合があります。|
|approvalPending|5|デバイスは、承認が保留中です。|
|certificateReset|6|デバイスの証明書がリセットされました。|
|notRegisteredPendingEnrollment|7|デバイスが登録されていません。登録は保留中です。|
|不明|8|デバイス ライセンス登録のステータスは不明です。|



