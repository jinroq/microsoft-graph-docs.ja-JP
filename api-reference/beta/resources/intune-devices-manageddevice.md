---
title: managedDevice リソース タイプ
description: Intune 経由で管理または事前登録されるデバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca9e4b4e3af7a7f307dd91bce748a7175ac2cce6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372294"
---
# <a name="manageddevice-resource-type"></a>managedDevice リソース タイプ

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune 経由で管理または事前登録されるデバイス

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。|
|[executeAction アクション](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)|まだ文書化されていません|
|[enableLostMode アクション](../api/intune-devices-manageddevice-enablelostmode.md)|None|削除モードを有効にする|
|[playLostModeSound アクション](../api/intune-devices-manageddevice-playlostmodesound.md)|None|リモート ロック|
|[setDeviceName アクション](../api/intune-devices-manageddevice-setdevicename.md)|None|デバイスのデバイス名を設定します。|
|[rotateFileVaultKey アクション](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|None|まだ文書化されていません|
|[getFileVaultKey 関数](../api/intune-devices-manageddevice-getfilevaultkey.md)|文字列型 (String)|まだ文書化されていません|
|[retire action](../api/intune-devices-manageddevice-retire.md)|None|デバイスを破棄します|
|[wipe action](../api/intune-devices-manageddevice-wipe.md)|None|デバイスをワイプします|
|[resetPasscode action](../api/intune-devices-manageddevice-resetpasscode.md)|None|パスコードをリセットします|
|[remoteLock action](../api/intune-devices-manageddevice-remotelock.md)|None|リモート ロック|
|[requestRemoteAssistance action](../api/intune-devices-manageddevice-requestremoteassistance.md)|None|リモート アシスタンスを要求します|
|[disableLostMode action](../api/intune-devices-manageddevice-disablelostmode.md)|None|紛失モードを無効化します|
|[locateDevice action](../api/intune-devices-manageddevice-locatedevice.md)|None|デバイスを検索します|
|[bypassActivationLock action](../api/intune-devices-manageddevice-bypassactivationlock.md)|None|アクティベーション ロックをバイパスします|
|[rebootNow action](../api/intune-devices-manageddevice-rebootnow.md)|None|デバイスを再起動します|
|[shutDown action](../api/intune-devices-manageddevice-shutdown.md)|None|デバイスをシャットダウンします|
|[recoverPasscode action](../api/intune-devices-manageddevice-recoverpasscode.md)|None|パスコードを回復します|
|[cleanWindowsDevice action](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|None|Windows デバイスをクリーンにします|
|[logoutSharedAppleDeviceActiveUser action](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|None|共有の Apple デバイスのアクティブなユーザーをログアウトします|
|[deleteUserFromSharedAppleDevice action](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|なし|共有の Apple デバイスからユーザーを削除します|
|[syncDevice action](../api/intune-devices-manageddevice-syncdevice.md)|None|まだ文書化されていません|
|[windowsDefenderScan action](../api/intune-devices-manageddevice-windowsdefenderscan.md)|None|まだ文書化されていません|
|[windowsDefenderUpdateSignatures action](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|None|まだ文書化されていません|
|[updateWindowsDeviceAccount action](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|なし|まだ文書化されていません|
|[revokeAppleVppLicenses アクション](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|None|デバイスのすべての Apple Vpp ライセンスを取り消す|
|[sendCustomNotificationToCompanyPortal アクション](../api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal.md)|None|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子|
|userId|String|デバイスに関連付けられているユーザーの一意の識別子|
|deviceName|String|デバイスの名前|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|デバイスのハードワードの詳細。  記憶領域、製造元、シリアル番号などの情報が含まれます。|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|デバイスの所有権。 ' Company ' または ' personal ' にすることができます。 可能な値は、`unknown`、`company`、`personal` です。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|デバイスの所有権。 ' Company ' または ' personal ' にすることができます。 可能な値は、`unknown`、`company`、`personal` です。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|デバイスの管理状態。 可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|デバイスのシャーシの種類。 可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。|
|operatingSystem|文字列|デバイスのオペレーティング システム。 Windows、iOS など。|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|デバイスのプラットフォーム。 可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|デバイスのコンプライアンス状態。 可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|String|デバイスが脱獄またはルート化されているかどうかを示します。|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|デバイスの管理チャネル。 Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`|
|osVersion|String|デバイスのオペレーティング システムのバージョン。|
|easActivated|Boolean|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。|
|easDeviceId|String|デバイスの Exchange ActiveSync の ID。|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。|
|aadRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。|
|azureADRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|デバイスの登録の種類。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|失われたモードが有効か無効かを示します。 可能な値は、`disabled`、`enabled` です。|
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
|retireAfterDateTime|DateTimeOffset|スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション|デバイスの最後にログオンしたユーザーを示します|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。  設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。 読み取り専用です。|
|autopilotEnrolled|Boolean|管理対象デバイスが自動パイロットで登録されているかどうかを報告します。|
|requireUserEnrollmentApproval|Boolean|管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。|
|managementCertificateExpirationDate|DateTimeOffset|デバイス管理証明書の有効期限を報告する|
|iccid|String|Ic カード識別子。 SIM カードの一意の識別番号です。|
|udid|String|IOS および macOS デバイスの一意のデバイス識別子。|
|roleScopeTagIds|文字列コレクション|このデバイスインスタンスの範囲タグ Id のリスト。|
|windowsActiveMalwareCount 再計算|Int32|この windows デバイスのアクティブなマルウェアの数|
|windowsRemediatedMalwareCount|Int32|この windows デバイスの修復済みマルウェアの数|
|notes|String|IT 管理者によって作成されたデバイスのメモ|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Configuration manager クライアント情報。管理されたデバイス、duel で管理されているデバイス、または ConfigMgr エージェントが管理する3つのデバイスに対してのみ有効です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|デバイスに現在インストールされているすべてのアプリケーション|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|デバイス カテゴリ|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|デバイス保護の状態。|
|users|[user](../resources/intune-shared-user.md) コレクション|管理対象デバイスに関連付けられているプライマリユーザー。|

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "osBuildNumber": "String"
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "retireAfterDateTime": "String (timestamp)",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String"
  }
}
```



