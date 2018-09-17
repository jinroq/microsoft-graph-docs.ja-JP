# <a name="androidcompliancepolicy-resource-type"></a>androidCompliancePolicy リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このクラスには、Android のコンプライアンス設定が含まれています。

[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidCompliancePolicies をリストします](../api/intune_deviceconfig_androidcompliancepolicy_list.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) コレクション|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[androidCompliancePolicy を取得します](../api/intune_deviceconfig_androidcompliancepolicy_get.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[AndroidCompliancePolicy を作成します](../api/intune_deviceconfig_androidcompliancepolicy_create.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|新しい [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトを作成します。|
|[AndroidCompliancePolicy を削除します](../api/intune_deviceconfig_androidcompliancepolicy_delete.md)|なし|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) を削除します。|
|[androidCompliancePolicy を更新します](../api/intune_deviceconfig_androidcompliancepolicy_update.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|passwordRequired|ブール値|デバイスのロックを解除するパスワードを要求します。|
|passwordMinimumLength|Int32|パスワードの最小文字数。 有効な値は 4 から 16 までです|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|パスワード内の文字の種類。 可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。|
|passwordMinutesOfInactivityBeforeLock|Int32|パスワードが要求されるまでの非アクティブ時間 (分)。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 65535 までです|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。|
|securityPreventInstallAppsFromUnknownSources|ブール値|デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。|
|securityDisableUsbDebugging|ブール値|Android デバイスでの USB デバッグを無効にします。|
|securityRequireVerifyApps|ブール値|Android の検証アプリ機能をオンにするよう要求します。|
|deviceThreatProtectionEnabled|ブール値|デバイスの脅威保護が有効になっていることを要求します。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。 可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。|
|securityBlockJailbrokenDevices|ブール値|デバイスの脱獄またはルート化を認めません。|
|osMinimumVersion|文字列|Android の最小バージョン。|
|osMaximumVersion|文字列|Android の最大バージョン。|
|minAndroidSecurityPatchLevel|文字列|Android セキュリティ パッチの最小レベル。|
|storageRequireEncryption|ブール値|Android デバイスでの暗号化を要求します。|
|securityRequireSafetyNetAttestationBasicIntegrity|ブール値|デバイスが SafetyNet の基本整合性チェックに合格することを要求します。|
|securityRequireSafetyNetAttestationCertifiedDevice|ブール値|デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。|
|securityRequireGooglePlayServices|ブール値|Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。|
|securityRequireUpToDateSecurityProviders|ブール値|デバイスに最新のセキュリティ プロバイダーが必要です。 デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。|
|securityRequireCompanyPortalAppIntegrity|ブール値|デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) コレクション|このルールのスケジュール済みのアクションのリスト ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) コレクション|DeviceComplianceDeviceStatus のリスト。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) コレクション|DeviceComplianceUserStatus のリスト。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|デバイス コンプライアンスとデバイス状態の概要 ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|デバイス コンプライアンスのユーザー状態の概要 ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|コンプライアンス設定状態のデバイスの要約 ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|割り当て|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) コレクション|このコンプライアンス ポリシーの割り当てのコレクション。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidCompliancePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```








