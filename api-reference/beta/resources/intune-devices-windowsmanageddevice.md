---
title: windowsManagedDevice リソースの種類
description: Intune 経由で管理または事前登録された Windows デバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c3cdc65f53e79bf5a9bb5b31e1438d74ccc876f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999410"
---
# <a name="windowsmanageddevice-resource-type"></a>windowsManagedDevice リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune 経由で管理または事前登録された Windows デバイス


[Manageddevice](../resources/intune-devices-manageddevice.md)からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsManagedDevices を一覧表示する](../api/intune-devices-windowsmanageddevice-list.md)|[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)コレクション|[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsManagedDevice を取得する](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsManagedDevice の作成](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|新しい[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを作成します。|
|[WindowsManagedDevice の削除](../api/intune-devices-windowsmanageddevice-delete.md)|None|[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)を削除します。|
|[WindowsManagedDevice を更新する](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
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

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) コレクション|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに現在インストールされているすべてのアプリケーション|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|[Manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスカテゴリ|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|デバイス保護の状態。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|
|users|[user](../resources/intune-shared-user.md) コレクション|管理対象デバイスに関連付けられているプライマリユーザー。 [Manageddevice](../resources/intune-devices-manageddevice.md)から継承します|

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
  }
}
```





