---
title: Update androidGeneralDeviceConfiguration
description: androidGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 1fedace3681289d0270bc944368e8b19dcc16103
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071117"
---
# <a name="update-androidgeneraldeviceconfiguration"></a>Update androidGeneralDeviceConfiguration

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。

次の表に、[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは値の取得のみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|appsBlockClipboardSharing|Boolean|アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。|
|appsBlockCopyPaste|Boolean|アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。|
|appsBlockYouTube|Boolean|YouTube アプリをブロックするかどうかを示します。|
|bluetoothBlocked|Boolean|Bluetooth をブロックするかどうかを示します。|
|cameraBlocked|Boolean|カメラの使用を禁止するかどうかを示します。|
|cellularBlockDataRoaming|Boolean|データ ローミングをブロックするかどうかを示します。|
|cellularBlockMessaging|Boolean|SMS/MMS メッセージングをブロックするかどうかを示します。|
|cellularBlockVoiceRoaming|Boolean|音声通話ローミングをブロックするかどうかを示します。|
|cellularBlockWiFiTethering|Boolean|Wi-Fi テザリングの同期をブロックするかどうかを示します。|
|compliantAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|CompliantAppsList 内にあるリストの種類。 可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。|
|diagnosticDataBlockSubmission|Boolean|診断データの送信をブロックするかどうかを示します。|
|locationServicesBlocked|Boolean|位置情報サービスをブロックするかどうかを示します。|
|googleAccountBlockAutoSync|Boolean|Google アカウントの自動同期をブロックするかどうかを示します。|
|googlePlayStoreBlocked|Boolean|Google Play ストアをブロックするかどうかを示します。|
|kioskModeBlockSleepButton|Boolean|キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。|
|kioskModeBlockVolumeButtons|Boolean|キオスク モード中にボリューム ボタンをブロックするかどうかを示します。|
|dateAndTimeBlockChanges|ブール値|日付や連盟ノックス ・ モードでの時間の変更をブロックするかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|デバイスがキオスク モードのときに実行できるアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|nfcBlocked|Boolean|近距離無線通信をブロックするかどうかを示します。|
|passwordBlockFingerprintUnlock|Boolean|指紋によるロック解除を禁止するかどうかを示します。|
|passwordBlockTrustAgents|Boolean|Smart Lock や他の信頼エージェントをブロックするかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|パスワードの最小の長さ。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。 有効な値は 4 から 11 までです|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。|
|passwordRequired|Boolean|パスワードを要求するかどうかを指定します。|
|powerOffBlocked|Boolean|デバイスの電源オフをブロックするかどうかを示します。|
|factoryResetBlocked|Boolean|ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。|
|screenCaptureBlocked|Boolean|スクリーンショットを禁止するかどうかを示します。|
|deviceSharingAllowed|Boolean|デバイスの共有モードを許可するかどうかを示します。|
|storageBlockGoogleBackup|Boolean|Google バックアップを禁止するかどうかを示します。|
|storageBlockRemovableStorage|Boolean|リムーバブル記憶域の使用を禁止するかどうかを示します。|
|storageRequireDeviceEncryption|Boolean|デバイスの暗号化が必要かどうかを示します。|
|storageRequireRemovableStorageEncryption|Boolean|リムーバブル記憶域の暗号化が必要かどうかを示します。|
|voiceAssistantBlocked|Boolean|音声アシスタントの使用を禁止するかどうかを示します。|
|voiceDialingBlocked|Boolean|音声ダイヤルをブロックするかどうかを示します。|
|webBrowserBlockPopups|Boolean|Web ブラウザー内のポップアップをブロックするかどうかを示します。|
|webBrowserBlockAutofill|Boolean|Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。|
|webBrowserBlockJavaScript|Boolean|Web ブラウザー内の JavaScript をブロックするかどうかを示します。|
|webBrowserBlocked|Boolean|Web ブラウザーをブロックするかどうかを示します。|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Web ブラウザー内の Cookie の設定。 可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。|
|wiFiBlocked|Boolean|Wi-Fi の同期をブロックするかどうかを示します。|
|appsInstallAllowList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|KNOX デバイス上にインストールできるアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|appsLaunchBlockList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|KNOX デバイス上での起動がブロックされているアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|appsHideList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|KNOX デバイス上で非表示にするアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|securityRequireVerifyApps|Boolean|Android の検証アプリ機能をオンにするよう要求します。|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3153

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```




