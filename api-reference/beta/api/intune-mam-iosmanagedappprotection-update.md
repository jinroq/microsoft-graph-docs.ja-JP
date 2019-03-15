---
title: Update iosManagedAppProtection
description: iosManagedAppProtection オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bccf984fa66eacf9dc96b507debb15425748a3d1
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571383"
---
# <a name="update-iosmanagedappprotection"></a>Update iosManagedAppProtection

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトの JSON 表記を指定します。

次の表に、[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|description|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|String|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|期間|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|期間|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[managedappdatatransフェリーレベル](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可されたソース。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 使用可能な値は、`allApps`、`managedApps`、`none` です。|
|allowedOutboundDataTransferDestinations|[managedappdatatransフェリーレベル](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可された宛先。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`allApps`、`managedApps`、`none` です。|
|organizationalCredentialsRequired|Boolean|アプリを使用するために組織の資格情報が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedOutboundClipboardSharingLevel|[managedappクリップボードの sharinglevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。|
|dataBackupBlocked|Boolean|管理対象アプリのデータのバックアップがブロックされるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|deviceComplianceRequired|Boolean|デバイスの準拠が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|managedBrowserToOpenLinksRequired|Boolean|管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|saveAsBlocked|Boolean|ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOfflineBeforeWipeIsEnforced|Duration|アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|pinRequired|Boolean|アプリ レベルの pin が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|maximumPinRetries|Int32|管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|simplePinBlocked|Boolean|simplePin がブロックされるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumPinLength|Int32|PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`numeric`、`alphanumericAndSymbol` です。|
|periodBeforePinReset|Duration|PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedDataStorageLocations|[managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 使用可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。|
|contactSyncBlocked|Boolean|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|printBlocked|Boolean|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|fingerprintBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|Boolean|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredOsVersion|String|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningOsVersion|String|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredAppVersion|String|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningAppVersion|String|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWipeOsVersion|String|指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumwipeappversion|String|指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|DeviceComplianceRequired が true に設定されている場合、デバイスがルートまたは脱獄のどちらかの場合に、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 使用可能な値は、`block`、`wipe`、`warn` です。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|正しくない pin の再試行回数の最大数に基づいて、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 使用可能な値は、`block`、`wipe`、`warn` です。|
|pinRequiredInsteadOfBiometricTimeout|期間|[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承された非バイオメトリクスパスコードではなく、アプリ pin のタイムアウト (分単位)|
|allowedoutboundクリップの sharingexceptionlength|Int32|組織データおよびアカウントから任意のアプリケーションに切り取りまたはコピーすることができる文字数を指定します。 この設定は、allowedoutboundクリップボードの sharinglevel 制限より優先されます。 既定値 ' 0 ' は、例外が許可されていないことを意味します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|isAssigned|Boolean|包含グループにポリシーを配置するかどうかを示します。 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します|
|targetedappmanagementlevels|[appmanagementlevel](../resources/intune-mam-appmanagementlevel.md)|[targetedmanagedappprotection](../resources/intune-mam-targetedmanagedappprotection.md)から継承したこのポリシーの目的のアプリ管理レベル。 可能な値は、`unspecified`、`unmanaged`、`mdm`、`androidEnterprise` です。|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|管理対象アプリのデータに使用する暗号化の種類。 可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。|
|minimumRequiredSdkVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|faceIdBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このリスト内のアプリはポリシーから除外され、管理対象アプリからデータを受信できるようになります。|
|minimumWipeSdkVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。|
|allowedIosDeviceModels|String|管理対象アプリが動作するために、文字列として許可されるデバイスモデルのセミコロンで区切られたリスト。|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|指定されたデバイスモデルが許可されていない場合は、ブロックまたはワイプのいずれかの管理対象アプリの動作を定義します。 使用可能な値は、`block`、`wipe`、`warn` です。|
|thirdPartyKeyboardsBlocked|Boolean|管理対象アプリへのアクセス時にサードパーティ製のキーボードを許可するかどうかを定義します。|
|filterOpenInToOnlyManagedApps|Boolean|管理対象アプリから、選択された共有ファイルの場所に対してオープンイン操作がサポートされているかどうかを定義します。 この設定は、allowedoutbounddatatrans小 DisableProtectionOfManagedOutboundOpenInData が managedapps に設定されていて、が False に設定されている場合にのみ適用されます。|
|disableProtectionOfManagedOutboundOpenInData|Boolean|[IOS openin] オプションを使用して、他のアプリに転送されるデータの保護を無効にします。 この設定は、allowedoutbounddatatransferdestinations が managedapps に設定されている場合にのみ、True になることができます。|
|protectInboundDataFromUnknownSources|Boolean|不明なソースからの受信データを保護します。 AllowedInboundDataTransferSources が allapps に設定されている場合にのみ、この設定は True になります。|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトを応答本文で返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
Content-type: application/json
Content-length: 2544

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2716

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```




