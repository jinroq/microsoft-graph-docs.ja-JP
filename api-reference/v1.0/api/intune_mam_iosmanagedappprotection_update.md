# <a name="update-iosmanagedappprotection"></a>iosManagedAppProtection を更新

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementApps.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|承諾|アプリケーションまたは JSON|

## <a name="request-body"></a>要求本文
要求本文で、[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) オブジェクトの JSON 表記を指定します。

次の表に、[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) の作成時に必要なプロパティを示します。

|プロパティ|タイプ|説明|
|:---|:---|:---|
|displayName|文字列|ポリシーの表示名。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|説明|文字列|ポリシーの説明。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|ID|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|バージョン|文字列|エンティティのバージョン。 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|期間|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|期間|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|データの転送が許可されたソース。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`allApps`、`managedApps`、`none` です。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|データの転送が許可された宛先。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`allApps`、`managedApps`、`none` です。|
|organizationalCredentialsRequired|ブール値|アプリを使用するために組織の資格情報が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。|
|dataBackupBlocked|ブール値|管理対象アプリのデータのバックアップがブロックされるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|deviceComplianceRequired|ブール値|デバイスの準拠が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|managedBrowserToOpenLinksRequired|ブール値|管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|saveAsBlocked|ブール値|ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|periodOfflineBeforeWipeIsEnforced|期間|アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|pinRequired|ブール値|アプリ レベルの pin が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|maximumPinRetries|Int32|正しくない pin の再試行の最大回数。この回数を超えると管理対象アプリがブロックまたは消去されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|simplePinBlocked|ブール値|simplePin がブロックされるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumPinLength|Int32|PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。[managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`numeric`、`alphanumericAndSymbol` です。|
|periodBeforePinReset|期間|PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md) コレクション|ユーザーが管理対象データを格納できるデータの保存場所。[ManagedAppProtection](../resources/intune_mam_managedappprotection.md) から継承されます。指定できる値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。|
|contactSyncBlocked|ブール値|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|printBlocked|ブール値|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|fingerprintBlocked|ブール値|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|ブール値|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumRequiredOsVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumWarningOsVersion|文字列|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumRequiredAppVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|minimumWarningAppVersion|文字列|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune_mam_managedappprotection.md) から継承します|
|isAssigned|ブール値|包含グループにポリシーを配置するかどうかを示します。 [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) から継承します|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune_mam_managedappdataencryptiontype.md)|マネージ アプリケーションのデータに使用する暗号化の種類。可能な値は、`useDeviceSettings`、 `afterDeviceRestart`、 `whenDeviceLockedExceptOpenFiles`、 `whenDeviceLocked`です。|
|minimumRequiredSdkVersion|文字列|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|faceIdBlocked|ブール値|PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) オブジェクトを応答本文で返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
Content-type: application/json
Content-length: 1570

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1740

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```








