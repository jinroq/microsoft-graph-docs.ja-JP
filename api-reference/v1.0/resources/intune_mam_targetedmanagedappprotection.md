# <a name="targetedmanagedappprotection-resource-type"></a>targetedManagedAppProtection リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のセキュリティ グループを対象とした管理設定の詳細を構成するために使用するポリシー

[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[targetedManagedAppProtectionsをリストする](../api/intune_mam_targetedmanagedappprotection_list.md)|[targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) コレクション|[targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[targetedManagedAppProtectionを取得する](../api/intune_mam_targetedmanagedappprotection_get.md)|[targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|[targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[動作を割り当てる](../api/intune_mam_targetedmanagedappprotection_assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列|ポリシーの表示名。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|説明|文字列|ポリシーの説明。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|ID|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|バージョン|文字列|エンティティのバージョン。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|期間|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|期間|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|データの転送が許可されたソース。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、`allApps`、`managedApps`、`none` です。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|データの転送が許可された宛先。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、`allApps`、`managedApps`、`none` です。|
|organizationalCredentialsRequired|ブール値|アプリを使用するために組織の資格情報が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。|
|dataBackupBlocked|ブール値|管理対象アプリのデータのバックアップがブロックされるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|deviceComplianceRequired|ブール値|デバイスの準拠が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|managedBrowserToOpenLinksRequired|ブール値|管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|saveAsBlocked|ブール値|ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|periodOfflineBeforeWipeIsEnforced|期間|アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|pinRequired|ブール値|アプリ レベルの pin が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|maximumPinRetries|Int32|正しくない pin の再試行の最大回数。この回数を超えると管理対象アプリがブロックまたは消去されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|simplePinBlocked|ブール値|simplePin がブロックされるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumPinLength|Int32|PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します。 可能な値は、`numeric`、`alphanumericAndSymbol` です。|
|periodBeforePinReset|期間|PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md) コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|contactSyncBlocked|ブール値|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|printBlocked|ブール値|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|fingerprintBlocked|ブール値|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|ブール値|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumRequiredOsVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumWarningOsVersion|文字列|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumRequiredAppVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumWarningAppVersion|文字列|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|isAssigned|ブール値|包含グループにポリシーを配置するかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) コレクション|ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppProtection",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
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
  "isAssigned": true
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/intune_mam_targetedmanagedappprotection.md/microsoft.graph.targetedManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
