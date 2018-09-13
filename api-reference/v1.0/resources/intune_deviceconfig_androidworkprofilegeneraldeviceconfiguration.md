# <a name="androidworkprofilegeneraldeviceconfiguration-resource-type"></a>androidWorkProfileGeneralDeviceConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android 作業プロファイルの全般的なデバイス構成です。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidWorkProfileGeneralDeviceConfigurations のリスト](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_list.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) コレクション|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップを一覧にします。|
|[AndroidWorkProfileGeneralDeviceConfiguration を取得する](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_get.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)| [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み込みます。|
|[AndroidWorkProfileGeneralDeviceConfiguration を作成する](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_create.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|新しい [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトを作成します。|
|[AndroidWorkProfileGeneralDeviceConfiguration を削除する](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_delete.md)|なし|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) を削除します。|
|[AndroidWorkProfileGeneralDeviceConfiguration を更新する](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_update.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)| [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|passwordBlockFingerprintUnlock|ブール値|指紋によるロック解除を禁止するかどうかを示します。|
|passwordBlockTrustAgents|ブール値|Smart Lock や他の信頼エージェントをブロックするかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|パスワードの最小の長さ。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。 有効な値は 4 から 11 までです|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|許可される共有するデータの種類。 可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。|
|workProfileBlockNotificationsWhileDeviceLocked|ブール型|デバイスがロックされているときに通知をブロックするかどうかを示します。|
|workProfileBlockAddingAccounts|ブール型|ユーザーが作業プロファイル内のアカウントを追加/削除できないようにブロックします。|
|workProfileBluetoothEnableContactSharing|ブール型|企業の連絡先にアクセスするための bluetooth デバイスを許可します。|
|workProfileBlockScreenCapture|ブール型|作業プロファイルで、画面キャプチャをブロックします。|
|workProfileBlockCrossProfileCallerId|ブール型|個人プロフィールに作業プロファイルの呼び出し元 ID が表示されないようにします。|
|workProfileBlockCamera|ブール型|作業プロファイルのカメラをブロックします。|
|workProfileBlockCrossProfileContactsSearch|ブール型|個人プロフィールで利用可能な作業プロファイルの連絡先をブロックします。|
|workProfileBlockCrossProfileCopyPaste|ブール型|ブール値は、クロス プロファイルのコピー/貼り付けが許可されていない設定を有効にするかどうかを示します。|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|workProfilePasswordBlockFingerprintUnlock|ブール型|作業プロファイルを指紋でロック解除するのを禁止するかどうかを示します。|
|workProfilePasswordBlockTrustAgents|ブール型|作業プロファイルでスマートロックや他の信頼エージェントをブロックするかどうかを示します。|
|workProfilePasswordExpirationDays|Int32|作業プロファイルのパスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|workProfilePasswordMinimumLength|Int32|作業プロファイル パスワードの最小長。 有効な値は 4 から 16 までです|
|workProfilePasswordMinNumericCharacters|Int32|作業プロファイル パスワードに必要な数字の最小数です。 有効な値は 1 から 10 までです|
|workProfilePasswordMinNonLetterCharacters|Int32|作業プロファイルのパスワードに必要なアルファベット以外の文字数の最小値です。 有効な値は 1 から 10 までです|
|workProfilePasswordMinLetterCharacters|Int32|作業プロファイルのパスワードに必要な文字数の最小値です。 有効な値は 1 から 10 までです|
|workProfilePasswordMinLowerCaseCharacters|Int32|作業プロファイルのパスワードに必要な小文字の文字数の最小値です。 有効な値は 1 から 10 までです|
|workProfilePasswordMinUpperCaseCharacters|Int32|作業プロファイルのパスワードに必要な大文字の文字数の最小値です。 有効な値は 1 から 10 までです|
|workProfilePasswordMinSymbolCharacters|Int32|作業プロファイルのパスワードに必要なシンボル数の最小値です。 有効な値は 1 から 10 までです|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|workProfilePasswordPreviousPasswordBlockCount|Int32|ブロックする、以前の作業プロファイルパスワードの数。 有効な値は 0 から 24 までです|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|作業プロファイルが削除され、すべての企業データが削除されるまでに許容されるサインインエラー数です。 有効な値は 4 から 11 までです|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|必要な作業プロファイル パスワードの種類です。 可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。|
|workProfileRequirePassword|ブール型|作業プロファイルにパスワードが必要かどうか|
|securityRequireVerifyApps|ブール値|Android の検証アプリ機能がオンになっている必要があります。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileGeneralDeviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








