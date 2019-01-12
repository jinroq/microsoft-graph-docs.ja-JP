---
title: androidGeneralDeviceConfiguration リソース タイプ
description: このトピックでは、androidGeneralDeviceConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: c40c039208daef817701dd3f3dd43b0a0a2bd9d1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945987"
---
# <a name="androidgeneraldeviceconfiguration-resource-type"></a>androidGeneralDeviceConfiguration リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、androidGeneralDeviceConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List androidGeneralDeviceConfigurations](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-list.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) コレクション|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get androidGeneralDeviceConfiguration](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-get.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create androidGeneralDeviceConfiguration](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-create.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)|新しい [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを作成します。|
|[Delete androidGeneralDeviceConfiguration](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-delete.md)|なし|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) を削除します。|
|[Update androidGeneralDeviceConfiguration](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-update.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
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
|securityRequireVerifyApps|Boolean|Android の検証アプリ機能がオンになっている必要があります。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
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
  "@odata.type": "microsoft.graph.androidGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
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
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
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
  "webBrowserCookieSettings": "String",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "securityRequireVerifyApps": true
}
```



