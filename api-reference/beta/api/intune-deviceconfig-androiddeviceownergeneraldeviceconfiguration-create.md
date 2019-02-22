---
title: androiddeviceowner一般の devic/デバイスの作成
description: 新しい androiddeviceowner一般の devic/デバイスオブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e05e696b0a2c127abdc8c365829599777f55beae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143093"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a>androiddeviceowner一般の devic/デバイスの作成

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、androiddeviceowner一般の devic/devicオブジェクトの JSON 表記を指定します。

次の表に、androiddeviceowner[devic] の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountsBlockModification|ブール値|アカウントの追加または削除が無効であるかどうかを示します。|
|appsAllowInstallFromUnknownSources|ブール値|ユーザーが不明なソースを有効にできるかどうかを示します。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|アプリの自動更新ポリシーの値を示します。 可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。|
|appsdefaultpermissionpolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。 使用可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|appsRecommendSkippingFirstUseHints|ブール値|すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。|
|bluetoothBlockConfiguration|ブール値|ユーザーが bluetooth を構成することを禁止するかどうかを示します。|
|bluetoothBlockContactSharing|ブール値|ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。|
|cameraBlocked|ブール値|カメラの使用を無効にするかどうかを示します。|
|cellularBlockWiFiTethering|Boolean|Wi-Fi テザリングをブロックするかどうかを示します。|
|dataRoamingBlocked|ブール値|ユーザーのデータ移動を禁止するかどうかを示します。|
|dateTimeConfigurationBlocked|ブール値|ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。|
|factoryResetDeviceAdministratorEmails|String collection|デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。|
|factoryResetBlocked|Boolean|設定の出荷時のリセットオプションが無効になっているかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|デバイスがキオスクモードのときに表示される管理対象アプリの一覧。 このコレクションには、最大で 500 個の要素を含めることができます。|
|kioskModeWallpaperUrl|String|デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。|
|kioskModeExitCode|String|デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。|
|kioskModeVirtualHomeButtonEnabled|ブール値|デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。|
|microphoneForceMute|ブール値|デバイス上でのマイクのミュートをブロックするかどうかを示します。|
|networkEscapeHatchAllowed|ブール値|ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。|
|nfcblockoutgoingbeam|ブール値|NFC の送信ビームをブロックするかどうかを示します。|
|passwordblockkeyguard|ブール値|keyguard が無効であるかどうかを示します。|
|passwordblockkeygu/機能|[androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション|ブロックする device keyguard 機能のリストです。 このコレクションには、最大で 7 個の要素を含めることができます。 可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。|
|passwordExpirationDays|Int32|パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|デバイスで必要なパスワードの最小の長さを示します。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。|
|passwordPreviousPasswordCountToBlock|Int32|パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。 有効な値は 0 から 24 までです|
|passwordRequiredType|[androiddeviceownerrequiredpasswordtype](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|デバイスで必要なパスワードの最小品質を示します。 可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。 有効な値は 4 から 11 までです|
|safebootblocked|ブール値|セーフブートでのデバイスの再起動を無効にするかどうかを示します。|
|screenCaptureBlocked|Boolean|スクリーンショットを撮影する機能を無効にするかどうかを示します。|
|securityallowデバッグ機能|ブール値|ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。|
|securityRequireVerifyApps|ブール値|アプリを確認する必要があるかどうかを示します。|
|statusBarBlocked|ブール値|通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。|
|stayonmodes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション|デバイスの表示がオンのままになるモードの一覧です。 このコレクションには、最大4つの要素を含めることができます。 使用可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。|
|storageallowusb|ブール値|USB 大容量ストレージを許可するかどうかを示します。|
|storageblockexternalmedia|ブール値|外部メディアをブロックするかどうかを示します。|
|storageblockusbfiletransfer|ブール値|USB ファイル転送をブロックするかどうかを示します。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。 有効な値は 0 ~ 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。 有効な値は 0 ~ 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|システム更新構成の種類。 使用可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。|
|systemwindowsblocked ブロック|ブール値|Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。|
|ユーザー blockadd|ブール値|ユーザーおよびプロファイルの追加を無効にするかどうかを示します。|
|ユーザー blockremove|ブール値|他のユーザーのデバイスからの削除を無効にするかどうかを示します。|
|volumeblockadjustment|ブール値|マスターボリュームを調整するかどうかを示します。|
|vpnAlwaysOnPackageIdentifier|String|always on VPN 接続を処理するアプリの Android アプリパッケージ名。|
|vpnAlwaysOnLockdownMode|ブール値|always on vpn パッケージ名が指定されている場合は、vpn が切断されたときにネットワークトラフィックをロックするかどうかを指定します。|
|wifiBlockEditConfigurations|ブール値|ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。|
|wifiBlockEditPolicyDefinedConfigurations|ブール値|ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2517

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2689

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




