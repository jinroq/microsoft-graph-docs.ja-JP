# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

AppLocker アプリケーションのコントロールの種類の使用可能な値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。|
|enforceComponentsAndStoreApps|1|Windows コンポーネントとストア アプリを強制します。|
|auditComponentsAndStoreApps|2|Windows コンポーネントとストア アプリを監査します。|
|enforceComponentsStoreAppsAndSmartlocker|3|Windowsコンポーネントを監査し、アプリとスマートロッカーを保管します。|
|auditComponentsStoreAppsAndSmartlocker|4|Windowsコンポーネントを監査し、アプリとスマートロッカーを保管します。|



