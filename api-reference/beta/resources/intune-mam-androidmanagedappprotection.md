---
title: androidManagedAppProtection リソース タイプ
description: Android デバイス上の特定のセキュリティ グループおよびアプリの特定のセットを対象とした、管理設定の詳細を構成するために使用するポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 557aa282b86f55242756e42b47dec60a4356b6cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150527"
---
# <a name="androidmanagedappprotection-resource-type"></a>androidManagedAppProtection リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス上の特定のセキュリティ グループおよびアプリの特定のセットを対象とした、管理設定の詳細を構成するために使用するポリシー


[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List androidManagedAppProtections](../api/intune-mam-androidmanagedappprotection-list.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) コレクション|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get androidManagedAppProtection](../api/intune-mam-androidmanagedappprotection-get.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create androidManagedAppProtection](../api/intune-mam-androidmanagedappprotection-create.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|新しい [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを作成します。|
|[Delete androidManagedAppProtection](../api/intune-mam-androidmanagedappprotection-delete.md)|なし|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) を削除します。|
|[Update androidManagedAppProtection](../api/intune-mam-androidmanagedappprotection-update.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|説明|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|periodOfflineBeforeAccessCheck|Duration|デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|periodOnlineBeforeAccessCheck|Duration|デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|allowedInboundDataTransferSources|[managedappdatatransフェリーレベル](../resources/intune-mam-managedappdatatransferlevel.md)|データの転送が許可されたソース。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は `allApps`、`managedApps`、`none` です。|
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
|allowedDataStorageLocations|[managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション|ユーザーが管理対象データを格納できるデータの保存場所。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|contactSyncBlocked|Boolean|連絡先をユーザー デバイスに同期できるかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|printBlocked|Boolean|管理対象アプリからの印刷を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|fingerprintBlocked|Boolean|PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|disableAppPinIfDevicePinIsSet|Boolean|デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredOsVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningOsVersion|String|OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumRequiredAppVersion|String|バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWarningAppVersion|String|アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumWipeOsVersion|String|指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|minimumwipeappversion|String|指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。 [managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|DeviceComplianceRequired が true に設定されている場合、デバイスがルートまたは脱獄のどちらかの場合に、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は `block`、`wipe`、`warn` です。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|正しくない pin の再試行回数の最大数に基づいて、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。 [managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。 可能な値は `block`、`wipe`、`warn` です。|
|pinRequiredInsteadOfBiometricTimeout|Duration|[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承された非バイオメトリクスパスコードではなく、アプリ pin のタイムアウト (分単位)|
|isAssigned|Boolean|包含グループにポリシーを配置するかどうかを示します。 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します|
|targetedappmanagementlevels|[appmanagementlevel](../resources/intune-mam-appmanagementlevel.md)|[targetedmanagedappprotection](../resources/intune-mam-targetedmanagedappprotection.md)から継承したこのポリシーの目的のアプリ管理レベル。 使用可能な値は、`unspecified`、`unmanaged`、`mdm`、`androidEnterprise` です。|
|screenCaptureBlocked|Boolean|管理対象ユーザーによる管理対象アプリのスクリーン キャプチャが可能かどうかを示します。|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります|
|encryptAppData|Boolean|管理対象アプリのアプリケーション データを暗号化する必要があるかどうかを示します|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|minimumRequiredPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。|
|minimumWarningPatchVersion|String|ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このリストのアプリパッケージはポリシーから除外され、管理対象アプリからデータを受信できるようになります。|
|minimumWipePatchVersion|String|指定された値以下の Android セキュリティパッチレベルでは、管理対象アプリと関連会社のデータが消去されます。|
|allowedandroiddevicemanufacturers、|String|管理対象アプリが動作するために文字列として許可されるデバイスメーカーのセミコロンで区切られたリスト。|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|指定されたデバイスの製造元が許可されていない場合は、ブロックまたはワイプのいずれかの管理対象アプリの動作を定義します。 可能な値は、`block`、`wipe`、`warn` です。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション|ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します|
|apps|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション|ポリシーが配置されたアプリのリスト。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|構成の展開概要のナビゲーション プロパティ。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "minimumWipePatchVersion": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String"
}
```




