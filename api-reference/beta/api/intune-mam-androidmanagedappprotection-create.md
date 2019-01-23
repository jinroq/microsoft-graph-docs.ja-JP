---
title: Create androidManagedAppProtection
description: 新しい androidManagedAppProtection オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73c3b149bab70d8f3bb54f15eafd0b414c4e5486
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393201"
---
# <a name="create-androidmanagedappprotection"></a>Create androidManagedAppProtection

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを作成します。

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
POST /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、androidManagedAppProtection オブジェクトの JSON 表記を指定します。

次の表に、androidManagedAppProtection の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|説明|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|String|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|Duration|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|Duration|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可されたソース。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 可能な値は、`allApps`、`managedApps`、`none` です。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可された宛先。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 可能な値は、`allApps`、`managedApps`、`none` です。|
|organizationalCredentialsRequired|Boolean|アプリを使用するために組織の資格情報が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。|
|dataBackupBlocked|Boolean|管理対象アプリのデータのバックアップがブロックされるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|deviceComplianceRequired|Boolean|デバイスの準拠が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|managedBrowserToOpenLinksRequired|Boolean|管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|saveAsBlocked|Boolean|ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOfflineBeforeWipeIsEnforced|Duration|アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|pinRequired|Boolean|アプリ レベルの pin が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|maximumPinRetries|Int32|間違った暗証番号 (pin) の再試行の最大数は、マネージ アプリケーションがブロックされているかどうかが消去する前にしようとします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|simplePinBlocked|Boolean|simplePin がブロックされるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumPinLength|Int32|PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 可能な値は、`numeric`、`alphanumericAndSymbol` です。|
|periodBeforePinReset|Duration|PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。|
|contactSyncBlocked|Boolean|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|printBlocked|Boolean|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|fingerprintBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|Boolean|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredOsVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningOsVersion|String|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredAppVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningAppVersion|String|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWipeOsVersion|String|マネージ アプリケーションと関連付けられている会社のデータを消去は指定されたバージョン以下のバージョンです。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWipeAppVersion|String|マネージ アプリケーションと関連付けられている会社のデータを消去は指定されたバージョン以下のバージョンです。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|、マネージ アプリケーションの動作を定義するブロックまたはワイプ、デバイスのルートとなるか、とか、jailbroken、DeviceComplianceRequired が設定されている場合 true に設定します。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 使用可能な値は、`block`、`wipe` です。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|マネージ アプリケーションの動作では、いずれかのブロックを定義またはワイプ、不正な pin の再試行回数の最大数に基づいています。 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。 使用可能な値は、`block`、`wipe` です。|
|pinRequiredInsteadOfBiometricTimeout|Duration|[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から非生体認証パスコード継承ではなく、アプリのピンを分単位でタイムアウト|
|isAssigned|Boolean|包含グループにポリシーを配置するかどうかを示します。 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します|
|targetedAppManagementLevels|[appManagementLevel](../resources/intune-mam-appmanagementlevel.md)|[TargetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)から継承されるこのポリシーの目的のアプリケーション管理のレベル。 可能な値は、`unspecified`、`unmanaged`、`mdm`、`androidEnterprise` です。|
|screenCaptureBlocked|Boolean|管理対象ユーザーによる管理対象アプリのスクリーン キャプチャが可能かどうかを示します。|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります|
|encryptAppData|Boolean|管理対象アプリのアプリケーション データを暗号化する必要があるかどうかを示します|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|minimumRequiredPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。|
|minimumWarningPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このリスト内のアプリケーションのパッケージでは、ポリシーの対象外になり、マネージ アプリケーションからデータを受信できるようになります。|
|minimumWipePatchVersion|String|Android のセキュリティ修正プログラムのレベル以下または指定した値に等しいは、マネージ アプリケーションと関連付けられている会社のデータに拭きます。|
|allowedAndroidDeviceManufacturers|String|デバイスの製造元のセミコロン区切りのリストは、動作するマネージ アプリケーションの文字列として使用できます。|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|、マネージ アプリケーションの動作を定義するブロックまたは指定されたデバイスの製造元が許可されていない場合、クリーン インストールのいずれかです。 使用可能な値は、`block`、`wipe` です。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
Content-type: application/json
Content-length: 2460

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2632

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
}
```




