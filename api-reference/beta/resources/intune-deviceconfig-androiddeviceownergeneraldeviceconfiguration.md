---
title: androiddeviceowner一般 devic/リソースの種類
description: このトピックでは、androiddeviceownerによって公開される宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49e70fb573bc9e2a0f66fc4b17b1cc1c53160c55
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572286"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>androiddeviceowner一般 devic/リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、androiddeviceownerによって公開される宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List androiddeviceowner一般 deviceconfigurん](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[androiddeviceowner一般 devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)のコレクション|[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androiddeviceowner一般の devic/デバイスを取得する](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)プロパティとリレーションシップを読み取ります。|
|[androiddeviceowner一般の devic/デバイスの作成](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|新しい[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。|
|[androiddeviceowner一般の devic/デバイスの削除](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|なし|[androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devicの種類を削除します。|
|[androiddeviceowner一般の devic/デバイスの更新](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)プロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountsBlockModification|Boolean|アカウントの追加または削除が無効であるかどうかを示します。|
|appsAllowInstallFromUnknownSources|Boolean|ユーザーが不明なソースを有効にできるかどうかを示します。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|アプリの自動更新ポリシーの値を示します。 可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。|
|appsdefaultpermissionpolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。 可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|appsRecommendSkippingFirstUseHints|Boolean|すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。|
|bluetoothBlockConfiguration|Boolean|ユーザーが bluetooth を構成することを禁止するかどうかを示します。|
|bluetoothBlockContactSharing|Boolean|ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。|
|cameraBlocked|Boolean|カメラの使用を無効にするかどうかを示します。|
|cellularBlockWiFiTethering|Boolean|Wi-Fi テザリングをブロックするかどうかを示します。|
|dataRoamingBlocked|Boolean|ユーザーのデータ移動を禁止するかどうかを示します。|
|dateTimeConfigurationBlocked|Boolean|ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。|
|factoryResetDeviceAdministratorEmails|String collection|デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。|
|factoryResetBlocked|Boolean|設定の出荷時のリセットオプションが無効になっているかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|デバイスがキオスクモードのときに表示される管理対象アプリの一覧。 このコレクションには、最大で 500 個の要素を含めることができます。|
|kioskModeWallpaperUrl|String|デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。|
|kioskModeExitCode|String|デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。|
|kioskModeVirtualHomeButtonEnabled|Boolean|デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。|
|microphoneForceMute|Boolean|デバイス上でのマイクのミュートをブロックするかどうかを示します。|
|networkEscapeHatchAllowed|Boolean|ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。|
|nfcblockoutgoingbeam|Boolean|NFC の送信ビームをブロックするかどうかを示します。|
|passwordblockkeyguard|Boolean|keyguard が無効であるかどうかを示します。|
|passwordblockkeygu/機能|[androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション|ブロックする device keyguard 機能のリストです。 このコレクションには、最大で 7 個の要素を含めることができます。|
|passwordExpirationDays|Int32|パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|デバイスで必要なパスワードの最小の長さを示します。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。|
|passwordPreviousPasswordCountToBlock|Int32|パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。 有効な値は 0 から 24 までです|
|passwordRequiredType|[androiddeviceownerrequiredpasswordtype](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|デバイスで必要なパスワードの最小品質を示します。 可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。 有効な値は 4 から 11 までです|
|safebootblocked|Boolean|セーフブートでのデバイスの再起動を無効にするかどうかを示します。|
|screenCaptureBlocked|Boolean|スクリーンショットを撮影する機能を無効にするかどうかを示します。|
|securityallowデバッグ機能|Boolean|ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。|
|securityRequireVerifyApps|Boolean|アプリを確認する必要があるかどうかを示します。|
|statusBarBlocked|Boolean|通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。|
|stayonmodes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション|デバイスの表示がオンのままになるモードの一覧です。 このコレクションには、最大4つの要素を含めることができます。|
|storageallowusb|Boolean|USB 大容量ストレージを許可するかどうかを示します。|
|storageblockexternalmedia|Boolean|外部メディアをブロックするかどうかを示します。|
|storageblockusbfiletransfer|Boolean|USB ファイル転送をブロックするかどうかを示します。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。 有効な値は 0 ~ 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。 有効な値は 0 ~ 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|システム更新構成の種類。 可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。|
|systemwindowsblocked ブロック|Boolean|Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。|
|ユーザー blockadd|Boolean|ユーザーおよびプロファイルの追加を無効にするかどうかを示します。|
|ユーザー blockremove|Boolean|他のユーザーのデバイスからの削除を無効にするかどうかを示します。|
|volumeblockadjustment|Boolean|マスターボリュームを調整するかどうかを示します。|
|vpnAlwaysOnPackageIdentifier|String|always on VPN 接続を処理するアプリの Android アプリパッケージ名。|
|vpnAlwaysOnLockdownMode|Boolean|always on vpn パッケージ名が指定されている場合は、vpn が切断されたときにネットワークトラフィックをロックするかどうかを指定します。|
|wifiBlockEditConfigurations|Boolean|ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
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




