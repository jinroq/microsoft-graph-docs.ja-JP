---
title: windowsManagedDevice リソースの種類
description: 管理または整いました Intune を使用されている Windows のデバイス
ms.openlocfilehash: 753d6c40cb47ebd7c9e7fd0736ca8c574ceb80b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069901"
---
# <a name="windowsmanageddevice-resource-type"></a>windowsManagedDevice リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理または整いました Intune を使用されている Windows のデバイス

[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)コレクション|[WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsManagedDevice を取得します。](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|[WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsManagedDevice を作成します。](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|新しい[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを作成します。|
|[WindowsManagedDevice を削除します。](../api/intune-devices-windowsmanageddevice-delete.md)|なし|の[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)を削除します。|
|[WindowsManagedDevice を更新します。](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|[WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの一意の識別子|
|userId|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスに関連付けられているユーザーの一意の識別子|
|deviceName|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの名前|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|デバイスのハードウェアの詳細。  記憶域の製造元、シリアル番号などの情報が含まれています。[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|デバイスの所有権。 '会社' または[managedDevice](../resources/intune-devices-manageddevice.md)からの '個人' の継承を使用できます。 可能な値は、`unknown`、`company`、`personal` です。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|デバイスの所有権。 '会社' または[managedDevice](../resources/intune-devices-manageddevice.md)からの '個人' の継承を使用できます。 可能な値は、`unknown`、`company`、`personal` です。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|デバイスの状態を管理します。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|デバイスのシャーシの種類です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。|
|operatingSystem|String|デバイスのオペレーティング システム。 Windows では、iOS などです。[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|デバイスのプラットフォームです。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|デバイスのコンプライアンス状態。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|String|デバイスが脱獄またはルート化されているかどうかを示します。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|デバイスの管理チャネル。 Intune、EA などです。[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm` です。|
|osVersion|String|デバイスのオペレーティング システムのバージョン。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|easActivated|Boolean|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|easDeviceId|String|デバイスの Exchange ActiveSync の ID。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|aadRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|azureADRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|デバイスの登録の種類。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|失われたモードが有効になっているか、 [managedDevice](../resources/intune-devices-manageddevice.md)からの継承を無効にかどうかを示します。 使用可能な値は、`disabled`、`enabled` です。|
|activationLockBypassCode|String|デバイスのアクティベーション ロックをバイパスするためのコード。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|emailAddress|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスに関連付けられているユーザーの email(s)|
|azureActiveDirectoryDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|azureADDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|デバイスの登録状態。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。|
|deviceCategoryDisplayName|String|デバイスのカテゴリ表示名を継承[managedDevice から](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|デバイスは、 [managedDevice](../resources/intune-devices-manageddevice.md)からの継承の状態を管理|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|最後にデバイスが Exchange に接続した時刻。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange でのデバイスのアクセスの状態。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Exchange でのデバイスのアクセス状態の理由。
 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。|
|remoteAssistanceSessionUrl|String|デバイスとのリモート アシスタンス セッションを確立できるようにする URL。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|remoteAssistanceSessionErrorDetails|String|リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|isEncrypted|Boolean|[ManagedDevice](../resources/intune-devices-manageddevice.md)から、デバイスの暗号化状態継承|
|userPrincipalName|String|デバイス ユーザー プリンシパル名で継承される[managedDevice から](../resources/intune-devices-manageddevice.md)|
|model|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスのモデル|
|manufacturer|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスの製造元|
|imei|String|IMEI は[managedDevice](../resources/intune-devices-manageddevice.md)から継承|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるがデバイスのコンプライアンスの猶予期間の有効期限が切れると、日付と時刻|
|シリアル番号|String|シリアル番号は[managedDevice](../resources/intune-devices-manageddevice.md)から継承|
|phoneNumber|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの電話番号|
|androidSecurityPatchLevel|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から android のセキュリティ ・ パッチ ・ レベル継承|
|userDisplayName|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から、ユーザーの表示名継承|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|ConfigrMgr クライアントには、 [managedDevice](../resources/intune-devices-manageddevice.md)からの継承の機能が有効になっています。|
|wiFiMacAddress|String|Wi-fi MAC は、 [managedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|デバイスの正常性構成証明の状態。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|subscriberCarrier|String|サブスクライバーのキャリアは、 [managedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|meid|String|MEID は[managedDevice](../resources/intune-devices-manageddevice.md)から継承|
|totalStorageSpaceInBytes|Int64|バイトが[managedDevice](../resources/intune-devices-manageddevice.md)から継承することでストレージの合計|
|freeStorageSpaceInBytes|Int64|空きバイト数は、 [managedDevice](../resources/intune-devices-manageddevice.md)から継承することで|
|managedDeviceName|String|デバイスを識別する名前が自動的に生成されます。 ユーザー フレンドリ名に上書きできます。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。 読み取り専用です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション|最後に[managedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスのユーザーのログオンを示します|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|レポート preferMdmOverGroupPolicy 設定日付と時刻が設定されています。  設定すると、Intune MDM 設定が優先されますグループ ポリシー設定の競合がある場合。 読み取り専用です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|autopilotEnrolled|ブール値|自動操縦を使用して管理対象のデバイスが登録されている場合にレポートします。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|requireUserEnrollmentApproval|ブール値|マネージ iOS デバイスがユーザーの承認登録の場合にレポートします。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|managementCertificateExpirationDate|DateTimeOffset|デバイス管理証明書の有効期限の日付継承[managedDevice](../resources/intune-devices-manageddevice.md)からの報告します。|
|iccid|String|A SIM カードの一意の識別番号は集積回路カードの識別子です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|udid|String|IOS と macOS デバイスに一意のデバイス識別子です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|roleScopeTagIds|String コレクション|このデバイス インスタンスのスコープのタグ Id のリストです。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|windowsActiveMalwareCount|Int32|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される windows デバイスのアクティブなマルウェアの数|
|windowsRemediatedMalwareCount|Int32|この windows デバイス継承[managedDevice](../resources/intune-devices-manageddevice.md)からの修正されたマルウェアの数|
|notes|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から IT 管理者は継承によって作成されたデバイスに関する注意事項|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|構成マネージャー クライアント正常性の状態、 [managedDevice](../resources/intune-devices-manageddevice.md)から、MDM と構成マネージャー エージェントの継承によって管理されているデバイスに対してのみ有効です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイス上に現在インストールされているすべてのアプリケーション|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|[ManagedDevice](../resources/intune-devices-manageddevice.md)からのデバイス カテゴリ継承|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|デバイス保護の状態です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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





