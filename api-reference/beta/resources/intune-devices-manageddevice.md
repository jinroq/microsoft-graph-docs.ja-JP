---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
ms.openlocfilehash: eaca9444df77c2f95f6a6f9845c9383cd53cd99f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071858"
---
# <a name="manageddevice-resource-type"></a>managedDevice リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune 経由で管理または事前登録されるデバイス
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。|
|[executeAction アクション](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)|まだ文書化されていません|
|[enableLostMode アクション](../api/intune-devices-manageddevice-enablelostmode.md)|なし|失われるモードを有効にします。|
|[playLostModeSound アクション](../api/intune-devices-manageddevice-playlostmodesound.md)|なし|リモート ロック|
|[setDeviceName アクション](../api/intune-devices-manageddevice-setdevicename.md)|なし|デバイスのデバイス名を設定します。|
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
|[revokeAppleVppLicenses アクション](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|なし|デバイスのすべてのアップル Vpp ライセンスを失効させる|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子|
|userId|String|デバイスに関連付けられているユーザーの一意の識別子|
|deviceName|String|デバイスの名前|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|デバイスのハードウェアの詳細。  記憶域の製造元、シリアル番号などの情報が含まれています。|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|デバイスの所有権。 '会社' または '個人' にすることができます。 可能な値は、`unknown`、`company`、`personal` です。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|デバイスの所有権。 '会社' または '個人' にすることができます。 可能な値は、`unknown`、`company`、`personal` です。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|デバイスの状態を管理します。 可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|デバイスのシャーシの種類です。 可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。|
|operatingSystem|String|デバイスのオペレーティング システム。 Windows、iOS など。|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|デバイスのプラットフォームです。 使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|デバイスのコンプライアンス状態。 可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|String|デバイスが脱獄またはルート化されているかどうかを示します。|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|デバイスの管理チャネル。 Intune、EA などです。使用可能な値: `eas`、 `mdm`、 `easMdm`、 `intuneClient`、 `easIntuneClient`、 `configurationManagerClient`、 `configurationManagerClientMdm`、 `configurationManagerClientMdmEas`、 `unknown`、 `jamf`、 `googleCloudDevicePolicyController`、 `microsoft365ManagedMdm`。|
|osVersion|String|デバイスのオペレーティング システムのバージョン。|
|easActivated|Boolean|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。|
|easDeviceId|String|デバイスの Exchange ActiveSync の ID。|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。|
|aadRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。|
|azureADRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|デバイスの登録の種類。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|失われたモードが有効か無効を示します。 使用可能な値は、`disabled`、`enabled` です。|
|activationLockBypassCode|String|デバイスのアクティベーション ロックをバイパスするためのコード。|
|emailAddress|String|デバイスに関連付けられているユーザーの電子メール|
|azureActiveDirectoryDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。|
|azureADDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|デバイスの登録状態。 可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。|
|deviceCategoryDisplayName|String|デバイス カテゴリの表示名|
|isSupervised|Boolean|デバイスの管理状況|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|最後にデバイスが Exchange に接続した時刻。|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange でのデバイスのアクセスの状態。 可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。|
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
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。 読み取り専用です。 可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション|最後のデバイスのユーザーにログオンしていることを示します|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|レポート preferMdmOverGroupPolicy 設定日付と時刻が設定されています。  設定すると、Intune MDM 設定が優先されますグループ ポリシー設定の競合がある場合。 読み取り専用です。|
|autopilotEnrolled|ブール値|自動操縦を使用して管理対象のデバイスが登録されている場合にレポートします。|
|requireUserEnrollmentApproval|ブール値|マネージ iOS デバイスがユーザーの承認登録の場合にレポートします。|
|managementCertificateExpirationDate|DateTimeOffset|デバイスの管理の証明書の有効期限の日付をレポート|
|iccid|String|A SIM カードの一意の識別番号は集積回路カードの識別子です。|
|udid|String|IOS と macOS デバイスに一意のデバイス識別子です。|
|roleScopeTagIds|String コレクション|このデバイス インスタンスのスコープのタグ Id のリストです。|
|windowsActiveMalwareCount|Int32|この windows デバイスのアクティブなマルウェアの数|
|windowsRemediatedMalwareCount|Int32|この windows デバイス用の修正されたマルウェアの数|
|notes|String|IT 管理者によって作成されたデバイスに関する注意事項|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|構成マネージャー クライアント正常性の状態、または構成マネージャーの MDM エージェントによって管理されるデバイスに対してのみ有効です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|デバイス上に現在インストールされているすべてのアプリケーション|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|デバイス カテゴリ|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|デバイス保護の状態です。|

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
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
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
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
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
  "partnerReportedThreatState": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





