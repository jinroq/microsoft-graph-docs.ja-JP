---
title: defaultManagedAppProtection リソース タイプ
description: TargetedManagedAppProtection ポリシーの対象とされていないすべてのユーザーに対して、アプリの指定したセットに関する管理設定の詳細を構成するために使用するポリシー
author: tfitzmac
ms.openlocfilehash: 17f5377df623d439fbd68342f26d9a570c676f55
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317046"
---
# <a name="defaultmanagedappprotection-resource-type"></a>defaultManagedAppProtection リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|説明|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
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
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
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
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|管理対象アプリのデータに使用する暗号化の種類。 (iOS のみ)。 可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。|
|screenCaptureBlocked|Boolean|画面キャプチャがブロックされているかどうかを示します。 (Android のみ)|
|encryptAppData|Boolean|管理対象アプリのデータを暗号化するかどうかを示します。 (Android のみ)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|この設定を有効にすると、デバイス レベルの暗号化が有効になっている場合、アプリケーション レベルの暗号化が無効です。 (Android のみ)|
|minimumRequiredSdkVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 (iOS のみ)|
|customSettings|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|minimumRequiredPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。 (Android のみ)|
|minimumWarningPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。 (Android のみ)|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|iOS アプリをこのリストには、ポリシーの対象外になります、マネージ アプリケーションからデータを受信できるようになります。 (iOS のみ)|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このリスト内の android のアプリケーション パッケージは、ポリシーの対象外になり、マネージ アプリケーションからデータを受信できるようになります。 (Android のみ)|
|faceIdBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。 (iOS のみ)|
|minimumWipeSdkVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。|
|minimumWipePatchVersion|String|Android のセキュリティ修正プログラムのレベル以下または指定した値に等しいは、マネージ アプリケーションと関連付けられている会社のデータに拭きます。 (Android のみ)|
|allowedIosDeviceModels|String|デバイス モデルのセミコロン区切りのリストは、動作するマネージ アプリケーションの文字列として使用できます。 (iOS のみ)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|、マネージ アプリケーションの動作を定義するブロック] または [指定したデバイスのモデルが許可されていない場合、クリーン インストールします。 (iOS のみ)。 使用可能な値は、`block`、`wipe` です。|
|allowedAndroidDeviceManufacturers|String|デバイスの製造元のセミコロン区切りのリストは、動作するマネージ アプリケーションの文字列として使用できます。 (Android のみ)|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|、マネージ アプリケーションの動作を定義するブロックまたは指定されたデバイスの製造元が許可されていない場合、クリーン インストールのいずれかです。 (アプリのみ)。 使用可能な値は、`block`、`wipe` です。|
|thirdPartyKeyboardsBlocked|ブール型|サードパーティ製キーボードが管理されているアプリケーションへのアクセス中に許可されている場合を定義します。 (iOS のみ)|
|filterOpenInToOnlyManagedApps|ブール型|選択されているファイル共有の場所に、マネージ アプリケーションから開くの操作がサポートされている場合を定義します。 この設定は、AllowedOutboundDataTransferDestinations を ManagedApps に設定し、DisableProtectionOfManagedOutboundOpenInData が False に設定されて場合にのみ適用されます。 (iOS のみ)|
|disableProtectionOfManagedOutboundOpenInData|ブール型|IOS OpenIn オプションを使用して他のアプリケーションに転送されるデータの保護を無効にします。 この設定はのみできる AllowedOutboundDataTransferDestinations が ManagedApps に設定されている場合に true を設定します。 (iOS のみ)|
|protectInboundDataFromUnknownSources|ブール型|不明なソースから受信したデータを保護します。 この設定はのみできる AllowedInboundDataTransferSources が AllApps に設定されている場合に true を設定します。 (iOS のみ)|

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
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```





