---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3672e9a03c3259c56744a9c786cf6b1b8eacc7f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522630"
---
# <a name="manageddevice-resource-type"></a>managedDevice リソース タイプ

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune 経由で管理または事前登録されるデバイス

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedDevices](../api/intune-devices-manageddevice-list.md)|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create managedDevice](../api/intune-devices-manageddevice-create.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|新しい [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを作成します。|
|[Delete managedDevice](../api/intune-devices-manageddevice-delete.md)|なし|[managedDevice](../resources/intune-devices-manageddevice.md) を削除します。|
|[Update managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。|
|[retire action](../api/intune-devices-manageddevice-retire.md)|なし|デバイスを破棄します|
|[wipe action](../api/intune-devices-manageddevice-wipe.md)|なし|デバイスをワイプします|
|[resetPasscode action](../api/intune-devices-manageddevice-resetpasscode.md)|なし|パスコードをリセットします|
|[remoteLock action](../api/intune-devices-manageddevice-remotelock.md)|なし|リモート ロック|
|[requestRemoteAssistance action](../api/intune-devices-manageddevice-requestremoteassistance.md)|なし|リモート アシスタンスを要求します|
|[disableLostMode action](../api/intune-devices-manageddevice-disablelostmode.md)|なし|紛失モードを無効化します|
|[locateDevice action](../api/intune-devices-manageddevice-locatedevice.md)|なし|デバイスを検索します|
|[bypassActivationLock action](../api/intune-devices-manageddevice-bypassactivationlock.md)|なし|アクティベーション ロックをバイパスします|
|[rebootNow action](../api/intune-devices-manageddevice-rebootnow.md)|なし|デバイスを再起動します|
|[shutDown action](../api/intune-devices-manageddevice-shutdown.md)|なし|デバイスをシャットダウンします|
|[recoverPasscode action](../api/intune-devices-manageddevice-recoverpasscode.md)|なし|パスコードを回復します|
|[cleanWindowsDevice action](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|なし|Windows デバイスをクリーンにします|
|[logoutSharedAppleDeviceActiveUser action](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|なし|共有の Apple デバイスのアクティブなユーザーをログアウトします|
|[deleteUserFromSharedAppleDevice action](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|なし|共有の Apple デバイスからユーザーを削除します|
|[syncDevice action](../api/intune-devices-manageddevice-syncdevice.md)|なし|まだ文書化されていません|
|[windowsDefenderScan action](../api/intune-devices-manageddevice-windowsdefenderscan.md)|なし|まだ文書化されていません|
|[windowsDefenderUpdateSignatures action](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|なし|まだ文書化されていません|
|[updateWindowsDeviceAccount action](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子|
|userId|String|デバイスに関連付けられているユーザーの一意の識別子|
|deviceName|String|デバイスの名前|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|デバイスの所有権。 ' company ' または ' personal ' にすることができます。 使用可能な値は、`unknown`、`company`、`personal` です。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。|
|operatingSystem|String|デバイスのオペレーティング システム。 Windows、iOS など。|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|デバイスのコンプライアンス状態。 可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|String|デバイスが脱獄またはルート化されているかどうかを示します。|
|managementAgent|[managementagenttype](../resources/intune-devices-managementagenttype.md)|デバイスの管理チャネル。 Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。|
|osVersion|String|デバイスのオペレーティング システムのバージョン。|
|easActivated|ブール型|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。|
|easDeviceId|String|デバイスの Exchange ActiveSync の ID。|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。|
|azureADRegistered|ブール型|Azure Active Directory が登録されているデバイスかどうかを示します。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|デバイスの登録の種類。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|activationLockBypassCode|String|デバイスのアクティベーション ロックをバイパスするためのコード。|
|emailAddress|String|デバイスに関連付けられているユーザーの電子メール|
|azureADDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|デバイスの登録状態。 可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。|
|deviceCategoryDisplayName|String|デバイス カテゴリの表示名|
|isSupervised|ブール型|デバイスの管理状況|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|最後にデバイスが Exchange に接続した時刻。|
|exchangeAccessState|[devicemanagementexchangeaccessstate](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange でのデバイスのアクセスの状態。 可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Exchange でのデバイスのアクセス状態の理由。
 可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。|
|remoteAssistanceSessionUrl|String|デバイスとのリモート アシスタンス セッションを確立できるようにする URL。|
|remoteAssistanceSessionErrorDetails|String|リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。|
|isEncrypted|Boolean|デバイスの暗号化の状態|
|userPrincipalName|String|デバイスのユーザー プリンシパル名。|
|model|String|デバイスのモデル|
|manufacturer|String|デバイスのメーカー|
|imei|String|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が経過する DateTime|
|serialNumber|String|シリアル番号|
|phoneNumber|String|デバイスの電話番号|
|androidSecurityPatchLevel|String|Android セキュリティ パッチのレベル|
|userDisplayName|String|ユーザーの表示名|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|ConfigrMgr クライアント対応機能
|
|wiFiMacAddress|String|Wi-Fi MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|デバイスの正常性構成証明の状態。|
|subscriberCarrier|String|サブスクライバー通信事業者|
|meid|String|MEID|
|totalStorageSpaceInBytes|Int64|記憶域の合計 (バイト)|
|freeStorageSpaceInBytes|Int64|空き記憶域 (バイト)|
|managedDeviceName|String|デバイスを識別する名前が自動的に生成されます。 ユーザー フレンドリ名に上書きできます。|
|partnerReportedThreatState|[manageddevicepartnerreportedhealthstate](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。 読み取り専用です。 可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|デバイス カテゴリ|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```



