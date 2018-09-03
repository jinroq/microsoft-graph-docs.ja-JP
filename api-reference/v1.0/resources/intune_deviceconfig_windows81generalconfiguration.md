# <a name="windows81generalconfiguration-resource-type"></a>windows81GeneralConfiguration リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、windows81GeneralConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windows81GeneralConfigurations をリスト](../api/intune_deviceconfig_windows81generalconfiguration_list.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) コレクション|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windows81GeneralConfiguration を取得](../api/intune_deviceconfig_windows81generalconfiguration_get.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windows81GeneralConfiguration を作成](../api/intune_deviceconfig_windows81generalconfiguration_create.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|新しい [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトを作成します。|
|[windows81GeneralConfiguration を削除](../api/intune_deviceconfig_windows81generalconfiguration_delete.md)|なし|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) を削除します。|
|[windows81GeneralConfiguration を更新](../api/intune_deviceconfig_windows81generalconfiguration_update.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|description|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|accountsBlockAddingNonMicrosoftAccountEmail|ブール値|Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。|
|applyOnlyToWindows81|ブール値|このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。 このプロパティは読み取り専用です。|
|browserBlockAutofill|ブール値|自動入力を禁止するかどうかを示します。|
|browserBlockAutomaticDetectionOfIntranetSites|ブール値|イントラネット サイトの自動検出をブロックするかどうかを示します。|
|browserBlockEnterpriseModeAccess|ブール値|エンタープライズ モードのアクセスを禁止するかどうかを示します。|
|browserBlockJavaScript|ブール値|ユーザーが JavaScript を使用することを禁止するかどうかを示します。|
|browserBlockPlugins|ブール値|プラグインを禁止するかどうかを示します。|
|browserBlockPopups|ブール値|ポップアップをブロックするかどうかを示します。|
|browserBlockSendingDoNotTrackHeader|ブール値|ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。|
|browserBlockSingleWordEntryOnIntranetSites|ブール値|イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。|
|browserRequireSmartScreen|ブール値|スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。|
|browserEnterpriseModeSiteListLocation|文字列|エンタープライズ モードのサイト リストの場所。 ローカル ファイル、ローカル ネットワーク、http の場所が該当します。|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|インターネット セキュリティ レベル。 可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|イントラネット セキュリティ レベル。 可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。|
|browserLoggingReportLocation|文字列|ログ レポートの場所。|
|browserRequireHighSecurityForRestrictedSites|ブール値|制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。|
|browserRequireFirewall|ブール値|ファイアウォールが必要かどうかを示します。|
|browserRequireFraudWarning|ブール値|不正行為の警告を必要とするかどうかを示します。|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|信頼済みサイトのセキュリティ レベル。 可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。|
|cellularBlockDataRoaming|ブール値|データ ローミングをブロックするかどうかを示します。|
|diagnosticsBlockDataSubmission|ブール値|診断データの送信をブロックするかどうかを示します。|
|passwordBlockPicturePasswordAndPin|ブール値|ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限 (日数)。|
|passwordMinimumLength|Int32|パスワードの最小文字数。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordPreviousPasswordBlockCount|Int32|再使用を禁止する、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|必要なパスワードの種類。 指定できる値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるサインインの失敗回数。|
|storageRequireDeviceEncryption|ブール値|モバイル デバイスでの暗号化が必要かどうかを示します。|
|updatesRequireAutomaticUpdates|ブール値|自動更新が必要かどうかを示します。|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|ユーザー アカウント制御の設定。 可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。|
|workFoldersUrl|文字列|作業フォルダーの URL。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration",
  "@odata.annotations": [
    {
      "property": "applyOnlyToWindows81",
      "capabilities": {
        "computed": true,
        "permissions": "Read"
      }
    }
  ]
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



