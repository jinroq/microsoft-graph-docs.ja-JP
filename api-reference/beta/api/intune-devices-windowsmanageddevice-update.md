---
title: WindowsManagedDevice を更新する
description: WindowsManagedDevice オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c34794e490dfde03adadb730094f47a9e55ff377
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309885"
---
# <a name="update-windowsmanageddevice"></a>WindowsManagedDevice を更新する

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトの JSON 表記を指定します。

次の表に、 [Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの一意識別子|
|userId|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに関連付けられているユーザーの一意識別子|
|deviceName|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの名前|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|デバイスのハードワードの詳細。  記憶領域、製造元、シリアル番号などの情報が含まれます。[Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|デバイスの所有権。 ' Company ' または ' personal ' を[Manageddevice](../resources/intune-devices-manageddevice.md)から継承することができます。 可能な値は、`unknown`、`company`、`personal` です。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|デバイスの所有権。 ' Company ' または ' personal ' を[Manageddevice](../resources/intune-devices-manageddevice.md)から継承することができます。 可能な値は、`unknown`、`company`、`personal` です。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|デバイスの管理状態。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|デバイスのシャーシの種類。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。|
|operatingSystem|文字列|デバイスのオペレーティング システム。 Windows、iOS など[Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|デバイスのプラットフォーム。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|デバイスのコンプライアンス状態。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|String|デバイスが脱獄またはルート化されているかどうかを示します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|デバイスの管理チャネル。 Intune、EAS など。[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm` です。|
|osVersion|String|デバイスのオペレーティング システムのバージョン。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|easActivated|Boolean|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|easDeviceId|String|デバイスの Exchange ActiveSync の ID。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|aadRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|azureADRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|デバイスの登録の種類。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|失われたモードが有効になっているか、 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承が無効かどうかを示します。 可能な値は、`disabled`、`enabled` です。|
|activationLockBypassCode|String|デバイスのアクティベーション ロックをバイパスするためのコード。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|emailAddress|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに関連付けられているユーザーの電子メール|
|azureActiveDirectoryDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|azureADDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用です。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|デバイスの登録状態。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。|
|deviceCategoryDisplayName|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスカテゴリの表示名|
|isSupervised|Boolean|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの監視状態|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|最後にデバイスが Exchange に接続した時刻。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange でのデバイスのアクセスの状態。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Exchange でのデバイスのアクセス状態の理由。
 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。|
|remoteAssistanceSessionUrl|String|デバイスとのリモート アシスタンス セッションを確立できるようにする URL。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|remoteAssistanceSessionErrorDetails|String|リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|isEncrypted|Boolean|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの暗号化状態|
|userPrincipalName|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスユーザープリンシパル名|
|model|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスのモデル|
|manufacturer|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの製造元|
|imei|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイスコンプライアンスの猶予期間が[Manageddevice](../resources/intune-devices-manageddevice.md)から継承される日時|
|シリアル番号|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたシリアル|
|phoneNumber|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの電話番号|
|androidSecurityPatchLevel|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された Android セキュリティパッチレベル|
|userDisplayName|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたユーザーの表示名|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された grmgr クライアントの有効な機能の設定|
|wiFiMacAddress|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された wi-fi MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|デバイスの正常性構成証明の状態。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|subscriberCarrier|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたサブスクライバーキャリア|
|meid|String|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された meid|
|totalStorageSpaceInBytes|Int64|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された合計記憶域 (バイト)|
|freeStorageSpaceInBytes|Int64|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された空き記憶域 (バイト単位)|
|managedDeviceName|String|デバイスを識別する名前が自動的に生成されます。 ユーザー フレンドリ名に上書きできます。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。 読み取り専用です。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。 可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。|
|retireAfterDateTime|DateTimeOffset|スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの最後にログオンしたユーザーを示します|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。  設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。 読み取り専用です。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|autopilotEnrolled|Boolean|管理対象デバイスが自動パイロットで登録されているかどうかを報告します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|requireUserEnrollmentApproval|Boolean|管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|managementCertificateExpirationDate|DateTimeOffset|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイス管理証明書の有効期限日を報告します|
|iccid|String|Ic カード識別子。 SIM カードの一意の識別番号です。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|udid|String|IOS および macOS デバイスの一意のデバイス識別子。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|roleScopeTagIds|文字列コレクション|このデバイスインスタンスの範囲タグ Id のリスト。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|windowsActiveMalwareCount 再計算|Int32|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された、この windows デバイスのアクティブなマルウェアの数|
|windowsRemediatedMalwareCount|Int32|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された、この windows デバイスの修復されたマルウェアの数|
|notes|String|IT 管理者によって作成された、 [manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイス上のメモ|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されているデバイスに対してのみ有効。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Configuration manager クライアント情報。管理されたデバイス、または管理されたデバイス、または[Manageddevice](../resources/intune-devices-manageddevice.md)から継承された、ConfigMgr エージェントによって管理されたデバイスに対してのみ有効です。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7520

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value"
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value"
  }
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7569

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value"
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value"
  }
}
```






