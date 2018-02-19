# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス アプリ管理のシングルトン エンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceAppManagement の取得](../api/intune_mam_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceAppManagement の更新](../api/intune_mam_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedAppPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|管理対象アプリ ポリシーです。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) コレクション|iOS 管理対象アプリ ポリシーです。|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) コレクション|Android 管理対象アプリ ポリシーです。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) コレクション|既定の管理対象アプリ ポリシーです。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) コレクション|ターゲットとなる管理対象アプリの構成です。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) コレクション|MDM に登録されたデバイス上で実行されているアプリの Windows 情報保護です。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) コレクション|MDM に登録されていないデバイス上で実行されているアプリの Windows 情報保護です。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション|管理対象アプリの登録です。|
|managedAppStatuses|[managedAppStatus](../resources/intune_mam_managedappstatus.md) コレクション|管理対象アプリの状態です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



