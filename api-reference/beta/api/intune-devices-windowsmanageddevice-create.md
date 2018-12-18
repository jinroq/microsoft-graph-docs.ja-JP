---
title: WindowsManagedDevice を作成します。
description: 新しい windowsManagedDevice オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 21626854a52ed305dbf237562e151e168330f170
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324445"
---
# <a name="create-windowsmanageddevice"></a>WindowsManagedDevice を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを作成します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に windowsManagedDevice オブジェクトの JSON の形式を指定します。

次の表は、windowsManagedDevice を作成するときに必要なプロパティを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの一意の識別子|
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
|isEncrypted|ブール型|[ManagedDevice](../resources/intune-devices-manageddevice.md)から、デバイスの暗号化状態継承|
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
|autopilotEnrolled|ブール型|自動操縦を使用して管理対象のデバイスが登録されている場合にレポートします。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|requireUserEnrollmentApproval|ブール型|マネージ iOS デバイスがユーザーの承認登録の場合にレポートします。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|managementCertificateExpirationDate|DateTimeOffset|デバイス管理証明書の有効期限の日付継承[managedDevice](../resources/intune-devices-manageddevice.md)からの報告します。|
|iccid|String|A SIM カードの一意の識別番号は集積回路カードの識別子です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|udid|String|IOS と macOS デバイスに一意のデバイス識別子です。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|roleScopeTagIds|String コレクション|このデバイス インスタンスのスコープのタグ Id のリストです。 [ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。|
|windowsActiveMalwareCount|Int32|[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される windows デバイスのアクティブなマルウェアの数|
|windowsRemediatedMalwareCount|Int32|この windows デバイス継承[managedDevice](../resources/intune-devices-manageddevice.md)からの修正されたマルウェアの数|
|notes|String|[ManagedDevice](../resources/intune-devices-manageddevice.md)から IT 管理者は継承によって作成されたデバイスに関する注意事項|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|構成マネージャー クライアント正常性の状態、 [managedDevice](../resources/intune-devices-manageddevice.md)から、MDM と構成マネージャー エージェントの継承によって管理されているデバイスに対してのみ有効です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7173

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7222

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```





