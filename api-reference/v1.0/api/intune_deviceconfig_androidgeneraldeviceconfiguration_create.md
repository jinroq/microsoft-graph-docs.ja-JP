# <a name="create-androidgeneraldeviceconfiguration"></a>androidGeneralDeviceConfiguration を作成

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) オブジェクトを作成します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

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
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、androidGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。

次の表に、androidGeneralDeviceConfiguration 作成時に必要なプロパティを示します。

|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|appsBlockClipboardSharing|ブール値|アプリケーション間でコピー/貼り付けを行うためのクリップボードの共有をブロックするかどうかを示します。|
|appsBlockCopyPaste|ブール値|アプリケーション内でのコピー/貼り付けをブロックするかどうかを示します。|
|appsBlockYouTube|ブール値|YouTube アプリをブロックするかどうかを示します。|
|bluetoothBlocked|ブール値|Bluetooth をブロックするかどうかを示します。|
|cameraBlocked|ブール値|カメラの使用を禁止するかどうかを示します。|
|cellularBlockDataRoaming|ブール値|データ ローミングをブロックするかどうかを示します。|
|cellularBlockMessaging|ブール値|SMS/MMS メッセージングをブロックするかどうかを示します。|
|cellularBlockVoiceRoaming|ブール値|音声通話ローミングをブロックするかどうかを示します。|
|cellularBlockWiFiTethering|ブール値|Wi-Fi テザリングの同期をブロックするかどうかを示します。|
|compliantAppsList|[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション|コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|CompliantAppsList 内にあるリストの種類。 可能な値は、 `none`、`appsInListCompliant`、`appsNotInListCompliant` です。|
|diagnosticDataBlockSubmission|ブール値|診断データの送信をブロックするかどうかを示します。|
|locationServicesBlocked|ブール値|位置情報サービスをブロックするかどうかを示します。|
|googleAccountBlockAutoSync|ブール値|Google アカウントの自動同期をブロックするかどうかを示します。|
|googlePlayStoreBlocked|ブール値|Google Play ストアをブロックするかどうかを示します。|
|kioskModeBlockSleepButton|ブール値|キオスク モード中に画面スリープ ボタンをブロックするかどうかを示します。|
|kioskModeBlockVolumeButtons|ブール値|キオスク モード中にボリューム ボタンをブロックするかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション|デバイスがキオスク モードのときに実行できるアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|nfcBlocked|ブール値|近距離無線通信をブロックするかどうかを示します。|
|passwordBlockFingerprintUnlock|ブール値|指紋によるロック解除を禁止するかどうかを示します。|
|passwordBlockTrustAgents|ブール値|Smart Lock や他の信頼エージェントをブロックするかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|パスワードの最小の長さ。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。 有効な値は 4 から 11 までです|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|必要なパスワードの種類。 指定できる値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。|
|passwordRequired|ブール値|パスワードを要求するかどうかを指定します。|
|powerOffBlocked|ブール値|デバイスの電源オフをブロックするかどうかを示します。|
|factoryResetBlocked|ブール値|ユーザーが出荷時の設定にリセットできないようにするかどうかを示します。|
|screenCaptureBlocked|ブール値|スクリーンショットを禁止するかどうかを示します。|
|deviceSharingAllowed|ブール値|デバイスの共有モードを許可するかどうかを示します。|
|storageBlockGoogleBackup|ブール値|Google バックアップを禁止するかどうかを示します。|
|storageBlockRemovableStorage|ブール値|リムーバブル記憶域の使用を禁止するかどうかを示します。|
|storageRequireDeviceEncryption|ブール値|デバイスの暗号化が必要かどうかを示します。|
|storageRequireRemovableStorageEncryption|ブール値|リムーバブル記憶域の暗号化が必要かどうかを示します。|
|voiceAssistantBlocked|ブール値|音声アシスタントの使用を禁止するかどうかを示します。|
|voiceDialingBlocked|ブール値|音声ダイヤルをブロックするかどうかを示します。|
|webBrowserBlockPopups|ブール値|Web ブラウザー内のポップアップをブロックするかどうかを示します。|
|webBrowserBlockAutofill|ブール値|Web ブラウザーの自動塗りつぶし機能をブロックするかどうかを示します。|
|webBrowserBlockJavaScript|ブール値|Web ブラウザー内の JavaScript をブロックするかどうかを示します。|
|webBrowserBlocked|ブール値|Web ブラウザーをブロックするかどうかを示します。|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|Web ブラウザー内の Cookie の設定。 可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。|
|wiFiBlocked|ブール値|Wi-Fi の同期をブロックするかどうかを示します。|
|appsInstallAllowList|[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション|KNOX デバイス上にインストールできるアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|appsLaunchBlockList|[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション|KNOX デバイス上での起動がブロックされているアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|appsHideList|[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション|KNOX デバイス上で非表示にするアプリのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|securityRequireVerifyApps|ブール値|Android の検証アプリ機能をオンにするよう要求します。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3097

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



