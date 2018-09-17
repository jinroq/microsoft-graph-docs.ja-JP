# <a name="windowsphone81generalconfiguration-resource-type"></a>windowsPhone81GeneralConfiguration リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、windowsPhone81GeneralConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsPhone81GeneralConfigurations をリストします。](../api/intune_deviceconfig_windowsphone81generalconfiguration_list.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) コレクション|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsPhone81GeneralConfiguration を取得します。](../api/intune_deviceconfig_windowsphone81generalconfiguration_get.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsPhone81GeneralConfiguration を作成する](../api/intune_deviceconfig_windowsphone81generalconfiguration_create.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|新しい [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトを作成します。|
|[windowsPhone81GeneralConfiguration を削除します。](../api/intune_deviceconfig_windowsphone81generalconfiguration_delete.md)|なし|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) を削除します。|
|[windowsPhone81GeneralConfiguration を更新します。](../api/intune_deviceconfig_windowsphone81generalconfiguration_update.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|applyOnlyToWindowsPhone81|ブール型|このポリシーを Windows Phone 8.1 にのみ適用するかどうかを示す値。 このプロパティは読み取り専用です。|
|appsBlockCopyPaste|ブール型|コピー/貼り付けを禁止するかどうかを示します。|
|bluetoothBlocked|ブール型|Bluetooth をブロックするかどうかを示します。|
|cameraBlocked|ブール型|カメラをブロックするかどうかを示します。|
|cellularBlockWifiTethering|ブール型|Wi-Fi テザリングをブロックするかどうかを示します。 Wi-Fi がブロックされていれば、この値は関係ありません。|
|compliantAppsList|[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション|コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|AppComplianceList 内にあるリスト。可能な値は、 `none`、 `appsInListCompliant`、 `appsNotInListCompliant`です。|
|diagnosticDataBlockSubmission|ブール型|診断データの送信をブロックするかどうかを示します。|
|emailBlockAddingAccounts|ブール型|カスタム電子メール アカウントをブロックするかどうかを示します。|
|locationServicesBlocked|ブール型|位置情報サービスをブロックするかどうかを示します。|
|microsoftAccountBlocked|ブール型|Microsoft アカウントの使用を禁止するかどうかを示します。|
|nfcBlocked|ブール型|近距離無線通信をブロックするかどうかを示します。|
|passwordBlockSimple|ブール型|カレンダーの同期を禁止するかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。|
|passwordMinimumLength|Int32|パスワードの最小の長さ。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordMinimumCharacterSetCount|Int32|パスワードが含まなければならない文字セットの数。|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|必要なパスワードの種類です。可能な値は、 `deviceDefault`、 `alphanumeric`、 `numeric`です。|
|passwordRequired|ブール型|パスワードを要求するかどうかを指定します。|
|screenCaptureBlocked|ブール型|スクリーンショットを禁止するかどうかを示します。|
|storageBlockRemovableStorage|ブール型|リムーバブル記憶域をブロックするかどうかを示します。|
|storageRequireEncryption|ブール型|暗号化が必要かどうかを示します。|
|webBrowserBlocked|ブール型|Web ブラウザーをブロックするかどうかを示します。|
|wifiBlocked|ブール型|Wi-Fi をブロックするかどうかを示します。|
|wifiBlockAutomaticConnectHotspots|ブール型|Wi-Fi ホットスポットへの自動接続をブロックするかどうかを示します。 Wi-Fi がブロックされていれば、この値は関係ありません。|
|wifiBlockHotspotReporting|ブール型|Wi-Fi ホットスポット レポートをブロックするかどうかを示します。 Wi-Fi がブロックされていれば、この値は関係ありません。|
|windowsStoreBlocked|ブール型|Windows ストアをブロックするかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|課題|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
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
  "@odata.type": "microsoft.graph.windowsPhone81GeneralConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```








