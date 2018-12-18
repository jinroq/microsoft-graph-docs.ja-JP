---
title: AndroidDeviceOwnerGeneralDeviceConfiguration を更新します。
description: AndroidDeviceOwnerGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: bf81569d5af7e223ff24e34bc031a19633d22edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340097"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a>AndroidDeviceOwnerGeneralDeviceConfiguration を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。
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
要求の本文に[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトの JSON の形式を指定します。

[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール型|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountsBlockModification|ブール型|追加または削除、アカウントが無効かどうかを示します。|
|appsAllowInstallFromUnknownSources|ブール型|不明なソースの設定を有効にするユーザーを許可するかどうかを示します。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|アプリケーションの自動更新ポリシーの値を示します。 可能な値は、`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always` です。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|いずれかが定義されていない場合、アプリケーションの具体的には、実行時のアクセス許可の要求のアクセス許可ポリシーを示します。 可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|bluetoothBlockConfiguration|ブール型|Bluetooth の構成からユーザーをブロックするかどうかを示します。|
|bluetoothBlockContactSharing|ブール型|Bluetooth を使用して連絡先の共有からユーザーをブロックするかどうかを示します。|
|cameraBlocked|Boolean|カメラの使用を無効にするかどうかを示します。|
|cellularBlockWiFiTethering|Boolean|Wi-Fi テザリングをブロックするかどうかを示します。|
|dataRoamingBlocked|ブール型|ユーザーによるデータの移動を禁止するかどうかを示します。|
|dateTimeConfigurationBlocked|ブール型|日付またはデバイス上の時刻を手動で変更するからユーザーをブロックするかどうかを示します|
|factoryResetDeviceAdministratorEmails|String コレクション|デバイスは、工場出荷時を設定する前にリセットした後に認証する必要があります Google アカウントのメールのリストです。|
|factoryResetBlocked|Boolean|設定の工場出荷時リセット ・ オプションが無効になっているかどうかを示します。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|キオスク モードでは、デバイスに表示される管理対象のアプリケーションの一覧です。 このコレクションには、最大で 500 個の要素を含めることができます。|
|microphoneForceMute|ブール型|Unmuting デバイスのマイクをブロックするかどうかを示します。|
|networkEscapeHatchAllowed|ブール型|デバイスがブート時に一時的なネットワーク接続への接続を許可するかどうかを示します。|
|nfcBlockOutgoingBeam|ブール型|NFC 送信ビームをブロックするかどうかを示します。|
|passwordBlockKeyguard|ブール型|Keyguard が無効になっているかどうかを示します。|
|passwordExpirationDays|Int32|期限が切れるし、新しいパスワードが必要になる前のパスワードを設定できる時間 (秒) の量を示します。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|デバイスに必要なパスワードの最小の長さを示します。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトするまで非アクティブのミリ秒です。|
|passwordPreviousPasswordCountToBlock|Int32|場所ユーザーことはできませんが、履歴内の任意のパスワードと同じパスワードを入力するのには、パスワードの履歴の長さを示します。 有効な値は 0 から 24 までです|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|デバイスに必要なパスワードの最小の品質を示します。 可能な値は、`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|デバイスをワイプする前に、ユーザーが誤ったパスワードを入力できる回数を示します。 有効な値は 4 から 11 までです|
|safeBootBlocked|ブール型|セーフ ブート デバイスが無効になってを再起動するかどうかを示します。|
|screenCaptureBlocked|Boolean|スクリーン ショットを実行する機能を無効にするかどうかを示します。|
|securityAllowDebuggingFeatures|ブール型|デバイスのデバッグ機能を有効にすることからユーザーをブロックするかどうかを示します。|
|securityRequireVerifyApps|Boolean|示しているかどうかのアプリケーションが必要なことを確認します。|
|statusBarBlocked|ブール型|示すかどうか、またはステータス バーを無効に、通知、すばやく設定およびその他の画面のオーバーレイを含みます。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)コレクション|デバイスの表示が残ります電源モードの一覧です。 このコレクションには、最大 4 つの要素を含めることができます。 可能な値は、`notConfigured`、`ac`、`usb`、`wireless` です。|
|storageAllowUsb|ブール型|USB 大容量記憶装置を許可するかどうかを示します。|
|storageBlockExternalMedia|ブール型|外部メディアをブロックするかどうかを示します。|
|storageBlockUsbFileTransfer|ブール型|USB ファイル転送をブロックするかどうかを示します。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|システム更新プログラムの開始を午前 0 時以降後の分単位の数を示します。 有効な値の 0 から 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|システムの更新] ウィンドウを終了する午前 0 時以降後の分単位の数を示します。 有効な値の 0 から 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|システム更新の構成の型。 可能な値は、`deviceDefault`、`postpone`、`windowed`、`automatic` です。|
|usersBlockAdd|ブール型|ユーザーとプロファイルを追加することが無効になっているかどうかを示します。|
|usersBlockRemove|ブール型|デバイスから他のユーザーを削除するを無効にするかどうかを示します。|
|volumeBlockAdjustment|ブール型|マスター ボリュームが無効になっているを調整するかどうかを示します。|
|wifiBlockEditConfigurations|ブール型|Wifi 接続の設定を編集することからユーザーをブロックするかどうかを示します。|
|wifiBlockEditPolicyDefinedConfigurations|ブール型|ポリシーで定義されているネットワークだけを編集するユーザーをブロックするかどうかを示します。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2073

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





