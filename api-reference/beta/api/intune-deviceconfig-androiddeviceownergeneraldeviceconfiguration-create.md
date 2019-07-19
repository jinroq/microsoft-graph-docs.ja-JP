---
title: Androiddeviceowner一般の Devic/デバイスの作成
description: 新しい Androiddeviceowner一般の Devic/デバイスオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16ba295955cc32f932612c5d2d4007ffedca46af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971431"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a>Androiddeviceowner一般の Devic/デバイスの作成

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[Androiddeviceowner一般の Devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、Androiddeviceowner一般の Devic/devicオブジェクトの JSON 表記を指定します。

次の表に、Androiddeviceowner[Devic] の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|このポリシーの OS エディションの適用。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|このポリシーの OS バージョン適用ルール。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|Devicemanagementの信頼性ルール Devicemode|[Devicemanagementの信頼性ルール Devicemode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|このポリシーのデバイスモード適用ルール。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountsBlockModification|Boolean|アカウントの追加または削除が無効であるかどうかを示します。|
|appsAllowInstallFromUnknownSources|Boolean|ユーザーが不明なソースを有効にできるかどうかを示します。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|アプリの自動更新ポリシーの値を示します。 可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|アプリに対して定義されていない場合、実行時のアクセス許可の要求に対するアクセス許可ポリシーを示します。 使用可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|appsRecommendSkippingFirstUseHints|Boolean|すべてのアプリが、追加された初回使用時のヒントをスキップするかどうかを指定します。|
|bluetoothBlockConfiguration|Boolean|ユーザーが bluetooth を構成することを禁止するかどうかを示します。|
|bluetoothBlockContactSharing|Boolean|ユーザーが bluetooth を介して連絡先を共有することを禁止するかどうかを示します。|
|cameraBlocked|Boolean|カメラの使用を無効にするかどうかを示します。|
|cellularBlockWiFiTethering|Boolean|Wi-Fi テザリングをブロックするかどうかを示します。|
|dataRoamingBlocked|Boolean|ユーザーのデータ移動を禁止するかどうかを示します。|
|dateTimeConfigurationBlocked|Boolean|ユーザーがデバイスの日付または時刻を手動で変更することを禁止するかどうかを示します。|
|factoryResetDeviceAdministratorEmails|文字列コレクション|デバイスを設定する前にリセットする必要がある、Google アカウント電子メールの一覧。|
|factoryResetBlocked|Boolean|設定の出荷時のリセットオプションが無効になっているかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|デバイスがキオスクモードのときに表示される管理対象アプリの一覧。 このコレクションには、最大で 500 個の要素を含めることができます。|
|kioskModeWallpaperUrl|String|デバイスがキオスクモードのときに壁紙に使用する、公開されている画像の URL。|
|kioskModeExitCode|String|デバイスがキオスクモードのときに、ユーザーがキオスクモードからのエスケープを許可する終了コード。|
|kioskModeVirtualHomeButtonEnabled|Boolean|デバイスがキオスクモードのときに仮想ホームボタンを表示するかどうかを指定します。|
|kioskModeBluetoothConfigurationEnabled|Boolean|ユーザーがキオスクモードで Bluetooth 設定を構成することを許可するかどうかを指定します。|
|kioskModeWiFiConfigurationEnabled|Boolean|ユーザーがキオスクモードで Wi-fi 設定を構成することを許可するかどうかを指定します。|
|microphoneForceMute|Boolean|デバイス上でのマイクのミュートをブロックするかどうかを示します。|
|networkEscapeHatchAllowed|Boolean|ブート時にデバイスが一時的なネットワーク接続に接続することを許可するかどうかを示します。|
|nfcBlockOutgoingBeam|Boolean|NFC の送信ビームをブロックするかどうかを示します。|
|passwordBlockKeyguard|Boolean|Keyguard が無効であるかどうかを示します。|
|Passwordblockkeygu/機能|[Androidkeygu/機能](../resources/intune-deviceconfig-androidkeyguardfeature.md)コレクション|ブロックする device keyguard 機能のリストです。 このコレクションには、最大で 7 個の要素を含めることができます。 可能な値は、`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures` です。|
|passwordExpirationDays|Int32|パスワードを期限切れにするために設定できる時間を秒単位で指定し、新しいパスワードを入力する必要があります。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|デバイスで必要なパスワードの最小の長さを示します。 有効な値は 4 から 16 までです|
|passwordMinimumLetterCharacters|Int32|デバイスパスワードに必要な文字の最小数を示します。 有効な値は1から16までです|
|passwordMinimumLowerCaseCharacters|Int32|デバイスパスワードに必要な小文字の最小文字数を示します。 有効な値は1から16までです|
|passwordMinimumNonLetterCharacters|Int32|デバイスパスワードに必要な文字以外の文字の最小数を示します。 有効な値は1から16までです|
|passwordMinimumNumericCharacters|Int32|デバイスパスワードに必要な最小文字数を示します。 有効な値は1から16までです|
|Passwordminimumシンボル文字|Int32|デバイスパスワードに必要な最小記号文字数を示します。 有効な値は1から16までです|
|passwordMinimumUpperCaseCharacters|Int32|デバイスのパスワードに必要な上位 caseletter 文字の最小数を示します。 有効な値は1から16までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (ミリ秒)。|
|passwordPreviousPasswordCountToBlock|Int32|パスワードの履歴の長さを示します。ユーザーは、履歴にあるパスワードと同じパスワードを入力することはできません。 有効な値は 0 から 24 までです|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|デバイスで必要なパスワードの最小品質を示します。 可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|ユーザーが間違ったパスワードを入力したときにデバイスがワイプされるまでの回数を示します。 有効な値は 4 から 11 までです|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|デバイスの再生ストアモードを示します。 可能な値は、`notConfigured`、`allowList`、`blockList` です。|
|safeBootBlocked|Boolean|セーフブートでのデバイスの再起動を無効にするかどうかを示します。|
|screenCaptureBlocked|Boolean|スクリーンショットを撮影する機能を無効にするかどうかを示します。|
|Securityallowデバッグ機能|Boolean|ユーザーがデバイスのデバッグ機能を有効にすることを禁止するかどうかを示します。|
|securityRequireVerifyApps|Boolean|アプリを確認する必要があるかどうかを示します。|
|statusBarBlocked|Boolean|通知、クイック設定、その他の画面オーバーレイを含む、ステータスバーを無効にするかどうかを示します。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション|デバイスの表示がオンのままになるモードの一覧です。 このコレクションには、最大4つの要素を含めることができます。 使用可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。|
|storageAllowUsb|Boolean|USB 大容量ストレージを許可するかどうかを示します。|
|storageBlockExternalMedia|Boolean|外部メディアをブロックするかどうかを示します。|
|storageBlockUsbFileTransfer|Boolean|USB ファイル転送をブロックするかどうかを示します。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|[システムの更新] ウィンドウが起動する午前0時からの経過時間 (分単位) を示します。 有効な値は 0 ~ 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|[システムの更新] ウィンドウが終了する午前0時からの経過時間 (分単位) を示します。 有効な値は 0 ~ 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|システム更新構成の種類。 使用可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。|
|systemWindowsBlocked ブロック|Boolean|Android システムプロンプトウィンドウ (toasts、電話活動、システム通知など) を禁止するかどうかを指定します。|
|ユーザー Blockadd|Boolean|ユーザーおよびプロファイルの追加を無効にするかどうかを示します。|
|ユーザー Blockremove|Boolean|他のユーザーのデバイスからの削除を無効にするかどうかを示します。|
|volumeBlockAdjustment|Boolean|マスターボリュームを調整するかどうかを示します。|
|vpnAlwaysOnPackageIdentifier|String|Always on VPN 接続を処理するアプリの Android アプリパッケージ名。|
|vpnAlwaysOnLockdownMode|Boolean|Always on VPN パッケージ名が指定されている場合は、VPN が切断されたときにネットワークトラフィックをロックするかどうかを指定します。|
|wifiBlockEditConfigurations|Boolean|ユーザーが wifi 接続設定を編集することを禁止するかどうかを示します。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|ユーザーがポリシーによって定義されたネットワークのみを編集することを禁止するかどうかを示します。|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androiddeviceowner一般の devic/デバイス](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3678

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
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
Content-Length: 3850

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
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





