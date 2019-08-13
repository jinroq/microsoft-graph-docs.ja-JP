---
title: defaultManagedAppProtection リソース タイプ
description: TargetedManagedAppProtection ポリシーの対象とされていないすべてのユーザーに対して、アプリの指定したセットに関する管理設定の詳細を構成するために使用するポリシー
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f361c2c098a63beda7a856b367ea92cd632090eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332268"
---
# <a name="defaultmanagedappprotection-resource-type"></a>defaultManagedAppProtection リソース タイプ

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

TargetedManagedAppProtection ポリシーの対象とされていないすべてのユーザーに対して、アプリの指定したセットに関する管理設定の詳細を構成するために使用するポリシー


[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List defaultManagedAppProtections](../api/intune-mam-defaultmanagedappprotection-list.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) コレクション|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-create.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|新しい [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを作成します。|
|[Delete defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-delete.md)|なし|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) を削除します。|
|[Update defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|description|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|期間|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|期間|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[Managedappdatatransフェリーレベル](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可されたソース。 [Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`allApps`、`managedApps`、`none` です。|
|allowedOutboundDataTransferDestinations|[Managedappdatatransフェリーレベル](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可された宛先。 [Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`allApps`、`managedApps`、`none` です。|
|organizationalCredentialsRequired|Boolean|アプリを使用するために組織の資格情報が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedOutboundClipboardSharingLevel|[Managedappクリップボードの Sharinglevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。 [Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。|
|dataBackupBlocked|Boolean|管理対象アプリのデータのバックアップがブロックされるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|deviceComplianceRequired|Boolean|デバイスの準拠が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|managedBrowserToOpenLinksRequired|Boolean|管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|saveAsBlocked|Boolean|ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOfflineBeforeWipeIsEnforced|Duration|アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|pinRequired|Boolean|アプリ レベルの pin が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|maximumPinRetries|Int32|管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|simplePinBlocked|Boolean|simplePin がブロックされるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumPinLength|Int32|PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。 [Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`numeric`、`alphanumericAndSymbol` です。|
|periodBeforePinReset|Duration|PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedDataStorageLocations|[Managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|contactSyncBlocked|Boolean|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|printBlocked|Boolean|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|fingerprintBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|Boolean|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredOsVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningOsVersion|String|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredAppVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningAppVersion|String|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWipeOsVersion|String|指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWipeAppVersion|String|指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|DeviceComplianceRequired が true に設定されている場合、デバイスがルートまたは脱獄のどちらかの場合に、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。 [Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`block`、`wipe`、`warn` です。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|正しくない pin の再試行回数の最大数に基づいて、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。 [Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は、`block`、`wipe`、`warn` です。|
|pinRequiredInsteadOfBiometricTimeout|期間|[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承された非バイオメトリクスパスコードではなく、アプリ pin のタイムアウト (分単位)|
|Allowedoutboundクリップの Sharingexceptionlength|Int32|組織データおよびアカウントから任意のアプリケーションに切り取りまたはコピーすることができる文字数を指定します。 この設定は、Allowedoutboundクリップボードの Sharinglevel 制限より優先されます。 既定値 ' 0 ' は、例外が許可されていないことを意味します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承したアプリ通知制限を指定します。 可能な値は、`allow`、`blockOrganizationalData`、`block` です。|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|管理対象アプリのデータに使用する暗号化の種類。 (iOS のみ)。 使用可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。|
|screenCaptureBlocked|Boolean|画面キャプチャがブロックされているかどうかを示します。 (Android のみ)|
|encryptAppData|Boolean|管理対象アプリのデータを暗号化するかどうかを示します。 (Android のみ)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|この設定を有効にすると、デバイスレベルの暗号化が有効になっている場合、アプリレベルの暗号化が無効になります。 (Android のみ)|
|minimumRequiredSdkVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 (iOS のみ)|
|customSettings|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|minimumRequiredPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。 (Android のみ)|
|minimumWarningPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。 (Android のみ)|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このリストに含まれる iOS アプリはポリシーから除外され、管理対象アプリからデータを受信できるようになります。 (iOS のみ)|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このリストの Android アプリパッケージは、ポリシーから除外され、管理対象アプリからデータを受信できるようになります。 (Android のみ)|
|faceIdBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。 (iOS のみ)|
|minimumWipeSdkVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。|
|minimumWipePatchVersion|String|指定された値以下の Android セキュリティパッチレベルでは、管理対象アプリと関連会社のデータが消去されます。 (Android のみ)|
|allowedIosDeviceModels|String|管理対象アプリが動作するために、文字列として許可されるデバイスモデルのセミコロンで区切られたリスト。 (iOS のみ)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|指定されたデバイスモデルが許可されていない場合は、ブロックまたはワイプのいずれかの管理対象アプリの動作を定義します。 (iOS のみ)。 可能な値は、`block`、`wipe`、`warn` です。|
|Allowedandroiddevicemanufacturers、|String|管理対象アプリが動作するために文字列として許可されるデバイスメーカーのセミコロンで区切られたリスト。 (Android のみ)|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|指定されたデバイスの製造元が許可されていない場合は、ブロックまたはワイプのいずれかの管理対象アプリの動作を定義します。 (Android のみ)。 可能な値は、`block`、`wipe`、`warn` です。|
|filterOpenInToOnlyManagedApps|Boolean|管理対象アプリから、選択された共有ファイルの場所に対してオープンイン操作がサポートされているかどうかを定義します。 この設定は、Allowedoutbounddatatrans小 DisableProtectionOfManagedOutboundOpenInData が ManagedApps に設定されていて、が False に設定されている場合にのみ適用されます。 (iOS のみ)|
|disableProtectionOfManagedOutboundOpenInData|Boolean|[IOS OpenIn] オプションを使用して、他のアプリに転送されるデータの保護を無効にします。 この設定は、AllowedOutboundDataTransferDestinations が ManagedApps に設定されている場合にのみ、True になることができます。 (iOS のみ)|
|protectInboundDataFromUnknownSources|Boolean|不明なソースからの受信データを保護します。 AllowedInboundDataTransferSources が AllApps に設定されている場合にのみ、この設定は True になります。 (iOS のみ)|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|管理対象アプリを機能させるための Android の Saf Etynet デバイスの構成証明要件を定義します。 可能な値は、`none`、`basicIntegrity`、`basicIntegrityAndDeviceCertification` です。|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|指定した Android の Saf Etynet 構成 requirment が失敗した場合に、警告またはブロックのいずれかの管理対象アプリの動作を定義します。 可能な値は、`block`、`wipe`、`warn` です。|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|管理対象アプリを機能させるための Android の Saf Etynet アプリの検証要件を定義します。 可能な値は、`none`、`enabled` です。|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|指定した Android アプリの検証 requirment が失敗した場合に、警告またはブロックのいずれかの管理対象アプリの動作を定義します。 可能な値は、`block`、`wipe`、`warn` です。|
|customBrowserProtocol|String|IOS で microsoft.rtc.management.writeableconfig.settings.weblink.weblink を開くためのカスタムブラウザープロトコル。 (iOS のみ)|
|customBrowserPackageId|String|Android で microsoft.rtc.management.writeableconfig.settings.weblink.weblink を開くためのカスタムブラウザーの一意識別子。 (Android のみ)|
|customBrowserDisplayName|String|Android で microsoft.rtc.management.writeableconfig.settings.weblink.weblink を開くために推奨されるカスタムブラウザーのフレンドリ名。 (Android のみ)|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション|ポリシーが配置されたアプリのリスト。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|構成の展開概要のナビゲーション プロパティ。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
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
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": 1024,
  "notificationRestriction": "String",
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
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "String",
  "minimumWipePatchVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserProtocol": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String"
}
```



