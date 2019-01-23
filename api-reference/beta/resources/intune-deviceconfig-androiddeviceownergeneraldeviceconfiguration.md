---
title: androidDeviceOwnerGeneralDeviceConfiguration リソースの種類
description: このトピックでは、宣言されたメソッドに、プロパティと androidDeviceOwnerGeneralDeviceConfiguration リソースによって公開されているリレーションシップの説明を提供します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac403bd13091a9db61b7f27462caecf6934b452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403750"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>androidDeviceOwnerGeneralDeviceConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、宣言されたメソッドに、プロパティと androidDeviceOwnerGeneralDeviceConfiguration リソースによって公開されているリレーションシップの説明を提供します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)コレクション|[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AndroidDeviceOwnerGeneralDeviceConfiguration を取得します。](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidDeviceOwnerGeneralDeviceConfiguration を作成します。](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|新しい[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。|
|[AndroidDeviceOwnerGeneralDeviceConfiguration を削除します。](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|なし|の[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)を削除します。|
|[AndroidDeviceOwnerGeneralDeviceConfiguration を更新します。](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountsBlockModification|Boolean|追加または削除、アカウントが無効かどうかを示します。|
|appsAllowInstallFromUnknownSources|Boolean|不明なソースの設定を有効にするユーザーを許可するかどうかを示します。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|アプリケーションの自動更新ポリシーの値を示します。 可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|いずれかが定義されていない場合、アプリケーションの具体的には、実行時のアクセス許可の要求のアクセス許可ポリシーを示します。 可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|appsRecommendSkippingFirstUseHints|Boolean|すべてのアプリケーションをお勧めするかどうかは、追加可能性があります、最初の時間の使用のヒントをスキップします。|
|bluetoothBlockConfiguration|Boolean|Bluetooth の構成からユーザーをブロックするかどうかを示します。|
|bluetoothBlockContactSharing|Boolean|Bluetooth を使用して連絡先の共有からユーザーをブロックするかどうかを示します。|
|cameraBlocked|Boolean|カメラの使用を無効にするかどうかを示します。|
|cellularBlockWiFiTethering|Boolean|Wi-Fi テザリングをブロックするかどうかを示します。|
|dataRoamingBlocked|Boolean|ユーザーによるデータの移動を禁止するかどうかを示します。|
|dateTimeConfigurationBlocked|Boolean|日付またはデバイス上の時刻を手動で変更するからユーザーをブロックするかどうかを示します|
|factoryResetDeviceAdministratorEmails|String コレクション|デバイスは、工場出荷時を設定する前にリセットした後に認証する必要があります Google アカウントのメールのリストです。|
|factoryResetBlocked|Boolean|設定の工場出荷時リセット ・ オプションが無効になっているかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|キオスク モードでは、デバイスに表示される管理対象のアプリケーションの一覧です。 このコレクションには、最大で 500 個の要素を含めることができます。|
|kioskModeWallpaperUrl|String|キオスク モードでは、デバイスとは、壁紙に使用するパブリックにアクセス可能なイメージの URL。|
|kioskModeExitCode|String|ユーザーがキオスク モードでは、デバイスとは、キオスク モードからエスケープできるようにするためのコードを終了します。|
|kioskModeVirtualHomeButtonEnabled|Boolean|キオスク モードでは、デバイスと仮想のホーム ボタンを表示するかどうかを指定します。|
|microphoneForceMute|Boolean|Unmuting デバイスのマイクをブロックするかどうかを示します。|
|networkEscapeHatchAllowed|Boolean|デバイスがブート時に一時的なネットワーク接続への接続を許可するかどうかを示します。|
|nfcBlockOutgoingBeam|Boolean|NFC 送信ビームをブロックするかどうかを示します。|
|passwordBlockKeyguard|Boolean|Keyguard が無効になっているかどうかを示します。|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション|ブロックするデバイスの keyguard の機能の一覧です。 このコレクションには、最大で 7 個の要素を含めることができます。|
|passwordExpirationDays|Int32|期限が切れるし、新しいパスワードが必要になる前のパスワードを設定できる時間 (秒) の量を示します。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|デバイスに必要なパスワードの最小の長さを示します。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトするまで非アクティブのミリ秒です。|
|passwordPreviousPasswordCountToBlock|Int32|場所ユーザーことはできませんが、履歴内の任意のパスワードと同じパスワードを入力するのには、パスワードの履歴の長さを示します。 有効な値は 0 から 24 までです|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|デバイスに必要なパスワードの最小の品質を示します。 可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|デバイスをワイプする前に、ユーザーが誤ったパスワードを入力できる回数を示します。 有効な値は 4 から 11 までです|
|safeBootBlocked|Boolean|セーフ ブート デバイスが無効になってを再起動するかどうかを示します。|
|screenCaptureBlocked|Boolean|スクリーン ショットを実行する機能を無効にするかどうかを示します。|
|securityAllowDebuggingFeatures|Boolean|デバイスのデバッグ機能を有効にすることからユーザーをブロックするかどうかを示します。|
|securityRequireVerifyApps|Boolean|示しているかどうかのアプリケーションが必要なことを確認します。|
|statusBarBlocked|Boolean|示すかどうか、またはステータス バーを無効に、通知、すばやく設定およびその他の画面のオーバーレイを含みます。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション|デバイスの表示が残ります電源モードの一覧です。 このコレクションには、最大 4 つの要素を含めることができます。|
|storageAllowUsb|Boolean|USB 大容量記憶装置を許可するかどうかを示します。|
|storageBlockExternalMedia|Boolean|外部メディアをブロックするかどうかを示します。|
|storageBlockUsbFileTransfer|Boolean|USB ファイル転送をブロックするかどうかを示します。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|システム更新プログラムの開始を午前 0 時以降後の分単位の数を示します。 有効な値の 0 から 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|システムの更新] ウィンドウを終了する午前 0 時以降後の分単位の数を示します。 有効な値の 0 から 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|システム更新の構成の型。 可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。|
|systemWindowsBlocked|Boolean|Android システムをブロックするかどうかは、toasts、電話活動、およびシステムの警告のように、windows を確認します。|
|usersBlockAdd|Boolean|ユーザーとプロファイルを追加することが無効になっているかどうかを示します。|
|usersBlockRemove|Boolean|デバイスから他のユーザーを削除するを無効にするかどうかを示します。|
|volumeBlockAdjustment|Boolean|マスター ボリュームが無効になっているを調整するかどうかを示します。|
|vpnAlwaysOnPackageIdentifier|String|常時接続で VPN 接続を処理するアプリケーションの android アプリのパッケージ名です。|
|vpnAlwaysOnLockdownMode|Boolean|常にオンの VPN は、パッケージの名前は指定、かどうか、その VPN が切断されたときに、ネットワーク トラフィックをロックされます。|
|wifiBlockEditConfigurations|Boolean|Wifi 接続の設定を編集することからユーザーをブロックするかどうかを示します。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|ポリシーで定義されているネットワークだけを編集するユーザーをブロックするかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "kioskModeWallpaperUrl": "String",
  "kioskModeExitCode": "String",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




