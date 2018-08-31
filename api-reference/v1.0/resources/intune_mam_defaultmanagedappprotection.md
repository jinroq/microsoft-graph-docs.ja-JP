# <a name="defaultmanagedappprotection-resource-type"></a>defaultManagedAppProtection リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

TargetedManagedAppProtection ポリシーの対象とされていないすべてのユーザーに対して、アプリの指定したセットに関する管理設定の詳細を構成するために使用するポリシー

[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[defaultManagedAppProtections をリスト](../api/intune_mam_defaultmanagedappprotection_list.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) コレクション|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[defaultManagedAppProtection を取得](../api/intune_mam_defaultmanagedappprotection_get.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[defaultManagedAppProtection を作成](../api/intune_mam_defaultmanagedappprotection_create.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|新しい [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトを作成します。|
|[defaultManagedAppProtection を削除](../api/intune_mam_defaultmanagedappprotection_delete.md)|なし|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) を削除します。|
|[defaultManagedAppProtection を更新する](../api/intune_mam_defaultmanagedappprotection_update.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|displayName|文字列|ポリシーの表示名。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|説明|文字列|ポリシーの説明。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|ID|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|version|文字列|エンティティのバージョン。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|期間|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|期間|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|データの転送が許可されたソース。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、 `allApps`、`managedApps`、`none` です。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|データの転送が許可された宛先。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、 `allApps`、`managedApps`、`none` です。|
|organizationalCredentialsRequired|ブール値|アプリを使用するために組織の資格情報が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。|
|dataBackupBlocked|ブール値|管理対象アプリのデータのバックアップがブロックされるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|deviceComplianceRequired|ブール値|デバイスの準拠が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|managedBrowserToOpenLinksRequired|ブール値|管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|saveAsBlocked|ブール値|ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|periodOfflineBeforeWipeIsEnforced|期間|アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|pinRequired|ブール値|アプリ レベルの pin が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|maximumPinRetries|Int32|正しくない pin の再試行の最大回数。この回数を超えると管理対象アプリがブロックされるか消去されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|simplePinBlocked|ブール値|simplePin がブロックされるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumPinLength|Int32|PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、`numeric`、`alphanumericAndSymbol` です。|
|periodBeforePinReset|期間|PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedDataStorageLocations|[managedAppDataStorageLocation 列挙型](../resources/intune_mam_managedappdatastoragelocation.md) コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|contactSyncBlocked|ブール値|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|printBlocked|ブール値|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|fingerprintBlocked|ブール値|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|ブール値|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumRequiredOsVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumWarningOsVersion|文字列|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumRequiredAppVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumWarningAppVersion|文字列|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune_mam_managedappdataencryptiontype.md)|管理対象アプリのデータに使用する暗号化の種類。 (iOS のみ)。 可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。|
|screenCaptureBlocked|ブール値|画面キャプチャがブロックされているかどうかを示します。|
|encryptAppData|ブール値|管理対象アプリのデータを暗号化するかどうかを示します。 (Android のみ)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|ブール値|この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります|
|minimumRequiredSdkVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。|
|customSettings|[keyValuePair](../resources/intune_mam_keyvaluepair.md) コレクション|このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|minimumRequiredPatchVersion|文字列|ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。|
|minimumWarningPatchVersion|文字列|ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。|
|faceIdBlocked|ブール値|PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|アプリ|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) コレクション|ポリシーが配置されたアプリのリスト。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|構成の展開概要のナビゲーション プロパティ。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppProtection",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "appDataEncryptionType": "String",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "faceIdBlocked": true
}
```



