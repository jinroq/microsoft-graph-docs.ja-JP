---
title: Microsoft Graph の変更ログ
description: この変更ログでは、Microsoft Graph と、v1.0 およびベータ版のエンドポイント Microsoft Graph API の変更内容について説明します。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: e4f8be6555aef71bfcb67f8fbc8671bacf6e6728
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344984"
---
# <a name="changelog-for-microsoft-graph"></a>Microsoft Graph の変更ログ

この変更ログでは、Microsoft Graph と、v1.0 およびベータ版のエンドポイント Microsoft Graph API の変更内容について説明します。

Microsoft Graph API に関する既知の問題の詳細については、「[既知の問題](known-issues.md)」を参照してください。

## <a name="may-2019"></a>2019 年 5 月

### <a name="reports-apis"></a>レポート API

| **変更の種類** | **バージョン** | **説明**                  |
|:----------------|:------------|:-----------------------------------------|
| 追加        | ベータ版  | **OwnerPrincipalName**プロパティが [oneDriveUsageAccountDetail](/graph/api/resources/oneDriveUsageAccountDetail?view=graph-rest-beta)エンティティに追加されました。|
| 追加        | ベータ版  | **ownerPrincipalName**プロパティが[sharePointSiteUsageDetail](/graph/api/resources/sharePointSiteUsageDetail?view=graph-rest-beta)エンティティに追加されました。|

### <a name="directory-apis"></a>ディレクトリ API
| **変更の種類** | **バージョン** | **説明** |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | 
  **assignedlabels**プロパティが[group](https://docs.microsoft.com/ja-JP/graph/api/resources/group?view=graph-rest-beta) エンティティに追加されました。 このプロパティは、グループに関連付けられている機密ラベル ペア (ラベル ID、ラベル名) のリストを表します。

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[deviceManagementDerivedCredentialSettings](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialsettings?view=graph-rest-beta)<br/>[iosDerivedCredentialAuthenticationConfiguration](/graph/api/resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration?view=graph-rest-beta)<br/>[securityBaselineCategoryStateSummary](/graph/api/resources/intune-deviceintent-securitybaselinecategorystatesummary?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[deviceManagementDerivedCredentialIssuer](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialissuer?view=graph-rest-beta)<br/>[deviceManagementDerivedCredentialNotificationType](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype?view=graph-rest-beta)<br/>[emailCertificateType](/graph/api/resources/intune-deviceconfig-emailcertificatetype?view=graph-rest-beta)<br/>[mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) コレクションに executeAction アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [rotateFileVaultKey](/graph/api/intune-devices-manageddevice-rotatefilevaultkey?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) に [migrateToTemplate](/graph/api/intune-deviceintent-devicemanagementintent-migratetotemplate?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [getFileVaultKey](/graph/api/intune-devices-manageddevice-getfilevaultkey?view=graph-rest-beta) 機能を追加しました |
|削除|ベータ版|次の列挙型を削除しました。<br/>**mobileAppDependecyType**<br/>|
|削除|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) コレクションの executeAction アクションを削除しました |
|追加|ベータ版|[androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) エンティティに **usernameFormatString**、**passwordFormatString** および **preSharedKey** プロパティを追加しました|
|追加|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに **customBrowserPackageId** および **customBrowserDisplayName** プロパティを追加しました|
|追加|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **customBrowserProtocol**、**customBrowserPackageId** および **customBrowserDisplayName** プロパティを追加しました|
|削除|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティから **thirdPartyKeyboardsBlocked** プロパティを削除しました|
|変更|ベータ版|[deviceManagementAbstractComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**implementationId** を必須から省略可能に変更しました<br/>|
|追加|ベータ版|[deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) エンティティに、**versionInfo**、**isDeprecated** および **intentCount** プロパティを追加しました|
|追加|ベータ版|[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta) エンティティに、**assignedUserPrincipalName** プロパティを追加しました|
|追加|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティに **signingCertificateType** および **encryptionCertificateType** プロパティを追加しました|
|追加|ベータ版|[iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) エンティティに **usernameFormatString** および **passwordFormatString** プロパティを追加しました|
|追加|ベータ版|[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **kioskModeBlockAutoLock**、、**kioskModeBlockRingerSwitch**、、**kioskModeBlockScreenRotation**、、**kioskModeBlockSleepButton**、、**kioskModeBlockTouchscreen**、、**cellularBlockPersonalHotspotModification** および **siriDisableServerLogging** プロパティを追加しました|
|追加|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに、**customBrowserProtocol** プロパティ を追加しました|
|削除|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティから **thirdPartyKeyboardsBlocked** プロパティを削除しました|
|追加|ベータ版|[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**iCloudBlockPhotoLibrary**、**screenCaptureBlocked**、**classroomAppBlockRemoteScreenObservation**、**classroomAppForceUnpromptedScreenObservation**、**classroomForceAutomaticallyJoinClasses**、**classroomForceRequestPermissionToLeaveClasses** および **classroomForceUnpromptedAppAndDeviceLock** プロパティを追加しました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、プロパティ **retireAfterDateTime** を追加しました|
|変更|ベータ版|[mobileAppDependency](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**dependencyType** を [mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta) から [mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta) に変更しました<br/>|
|追加|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティに **tpmRequired** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **roleScopeTagIds** プロパティを追加しました|
|追加|ベータ版|[windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta) エンティティに **configDeviceHealthMonitoringCustomScope** プロパティを追加しました|
|追加|ベータ版|[deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) エンティティに **migratableTo** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティに **derivedCredentialSettings** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) エンティティに **derivedCredentialSettings** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta) エンティティに **derivedCredentialSettings** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[securityBaselineTemplate](/graph/api/resources/intune-deviceintent-securitybaselinetemplate?view=graph-rest-beta) エンティティに **ategoryDeviceStateSummaries** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta) 列挙型に **wpaEnterprise** メンバーを追加しました|
|追加|ベータ版|[devicePlatformType](/graph/api/resources/intune-shared-deviceplatformtype?view=graph-rest-beta) 列挙型に **unknown** メンバーが追加されました|
|追加|ベータ版|[easAuthenticationMethod](/graph/api/resources/intune-deviceconfig-easauthenticationmethod?view=graph-rest-beta) 列挙型に **derivedCredential** メンバーを追加しました|
|追加|ベータ版|[managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 列挙型に **wipe** メンバーを追加しました|
|変更|ベータ版|[managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta) 列挙型で次のプロパティの型を変更しました:<br/>**fullScan** を 2 から 3 に変更しました。<br/>**quickScan** を 3 から 4 に変更しました。<br/>**signatureUpdate** を 4 から 5 に変更しました。<br/>|
|追加|ベータ版|[vpnAuthenticationMethod](/graph/api/resources/intune-deviceconfig-vpnauthenticationmethod?view=graph-rest-beta) 列挙型に **derivedCredential** メンバーを追加しました|
|追加|ベータ版|[wiFiAuthenticationMethod](/graph/api/resources/intune-deviceconfig-wifiauthenticationmethod?view=graph-rest-beta) 列挙型に **derivedCredential** メンバーを追加しました|

### <a name="risky-users-api"></a>リスクの高いユーザーの API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [riskyUserHistoryItem](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta) エンティティを追加しました。 |
| 追加 | ベータ版 | [履歴のリスト](/graph/api/riskyuser-list-history?view=graph-rest-beta)の操作を追加しました。 |

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0       | セキュア スコア API を [セキュリティ API](/graph/api/resources/securescore-api-overview?view=graph-rest-1.0) に追加しました。これには次のリソースと操作が含まれています。<br/>[secureScore](/graph/api/resources/securescore?view=graph-rest-1.0) (および関連するエンティティ)<br/>[secureScores のリスト](/graph/api/securescores-list?view=graph-rest-1.0)<br/>[secureScoreControlProfile](/graph/api/resources/securescorecontrolprofile?view=graph-rest-1.0)<br/>[secureScoreControlProfiles のリスト](/graph/api/securescorecontrolprofiles-list?view=graph-rest-1.0)<br/>[secureScoreControlProfiles の更新](/graph/api/securescorecontrolprofiles-update?view=graph-rest-1.0) |


## <a name="april-2019"></a>2019 年 4 月

### <a name="azure-ad-apis"></a>Azure AD API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | v1.0 |  新しい **Azure AD 用の監査ログ API** を導入しました。[directoryAudit](/graph/api/resources/directoryAudit?view=graph-rest-v1.0) からディレクトリ管理タスクのアクティビティ ログが提供され、[signIns](/graph/api/resources/signIns?view=graph-rest-v1.0) からサインイン アクティビティが提供されます。|
| 追加 | ベータ版 | **アクセス レビュー**に対する新しいアプリケーション アクセス許可 AccessReview.Read.All、ProgramControl.Read.All、ProgramControl.ReadWrite.All を追加しました。 詳細については、[アクセス レビュー API のリファレンス](/graph/api/resources/accessreviews-root?view=graph-rest-beta)を参照してください。 |
| 追加 | ベータ版 | **signInSessionsValidFromDateTime** プロパティを[ユーザー](/graph/api/resources/user?view=graph-rest-beta) リソースに追加します。 これは、**refreshTokensValidFromDateTime** プロパティの名前変更ですが、両方のプロパティはクライアントがスムーズに移行できるようにサポートされます。 数ヶ月後に、古いプロパティ **refreshTokensValidFromDateTime** が削除されます。|
| 追加 | ベータ版 | **revokeSignInSessions** アクションを[ユーザー](/graph/api/resources/user?view=graph-rest-beta) リソースに追加します。 これは、**invalidateAllRefreshTokens** プロパティの名前変更ですが、両方のサービス アクションはクライアントがスムーズに移行できるようにサポートされます。 数ヶ月後に、古いサービス アクション **invalidateAllRefreshTokens** は削除されます。 |

### <a name="azure-ad-b2c-apis"></a>Azure AD B2C APIs

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 |新しいリソースタイプ[trustFrameworkPolicy](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)が導入されました。 このリソースタイプは、[作成](/graph/api/trustframework-post-trustframeworkpolicy?view=graph-rest-beta)、[一覧表示](/graph/api/trustframework-list-trustframeworkpolicies?view=graph-rest-beta)、[取得](/graph/api/trustframeworkpolicy-get?view=graph-rest-beta)、 [更新](/graph/api/trustframework-put-trustframeworkpolicy?view=graph-rest-beta)、および[削除](/graph/api/trustframerkpolicy-delete?view=graph-rest-beta)の操作をサポートしています。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidDeviceOwnerCompliancePolicy](/graph/api/resources/intune-deviceconfig-androiddeviceownercompliancepolicy?view=graph-rest-beta)<br/><br/>[macOSExtensionsConfiguration](/graph/api/resources/intune-deviceconfig-macosextensionsconfiguration?view=graph-rest-beta)<br/><br/>[mobileAppDependency](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta)<br/><br/>[mobileAppRelationship](/graph/api/resources/intune-apps-mobileapprelationship?view=graph-rest-beta)<br/><br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[macOSKernelExtension](/graph/api/resources/intune-deviceconfig-macoskernelextension?view=graph-rest-beta)<br/><br/>[macOSLaunchItem](/graph/api/resources/intune-deviceconfig-macoslaunchitem?view=graph-rest-beta)<br/><br/>[mobileAppRelationshipState](/graph/api/resources/intune-apps-mobileapprelationshipstate?view=graph-rest-beta)<br/><br/>[win32LobAppFileSystemRequirement](/graph/api/resources/intune-apps-win32lobappfilesystemrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppPowerShellScriptRequirement](/graph/api/resources/intune-apps-win32lobapppowershellscriptrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppRegistryRequirement](/graph/api/resources/intune-apps-win32lobappregistryrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppRequirement](/graph/api/resources/intune-apps-win32lobapprequirement?view=graph-rest-beta)<br/><br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[androidDeviceOwnerPlayStoreMode](/graph/api/resources/intune-deviceconfig-androiddeviceownerplaystoremode?view=graph-rest-beta)<br/><br/>[mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta)<br/><br/>[win32LobAppPowerShellScriptDetectionType](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetectiontype?view=graph-rest-beta)<br/><br/>|
|追加|ベータ版|[ updateRelationships ](/graph/api/intune-apps-mobileapp-updaterelationships?view=graph-rest-beta)を追加しました。<br/> [ mobileApp ](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)に対するアクション<br/> |
|追加|ベータ版|[ importedWindowsAutopilotDeviceIdentity ](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)に**import **アクションを追加しました。<br/> コレクション |
|追加|ベータ版|[ getRelatedAppStates ](/graph/api/intune-apps-mobileapp-getrelatedappstates?view=graph-rest-beta)を追加しました。<br/> [mobileApp ](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)の機能<br/> |
|追加|ベータ版|**kioskModeBluetoothConfigurationEnabled**, **kioskModeWiFiConfigurationEnabled**, **passwordMinimumLetterCharacters**, **passwordMinimumLowerCaseCharacters**, **passwordMinimumNonLetterCharacters**, **passwordMinimumNumericCharacters**, **passwordMinimumSymbolCharacters**, **passwordMinimumUpperCaseCharacters** および[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)への**playStoreMode**プロパティを追加しました。<br/> エンティティ|
|追加|ベータ版|[ androidForWorkCertificateProfileBase ](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)に** subjectAlternativeNameType **プロパティを追加しました。<br/> エンティティ|
|削除|ベータ版|[ androidForWorkPkcsCertificateProfile ](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)から** subjectAlternativeNameType **プロパティーを削除しました。<br/> エンティティ|
|削除|ベータ版|[ androidForWorkScepCertificateProfile ](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)から** subjectAlternativeNameType **プロパティーを削除しました。<br/> エンティティ|
|追加|ベータ版|[ androidWorkProfileCertificateProfileBase ](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)に** subjectAlternativeNameType **プロパティを追加しました。<br/> エンティティ|
|削除|ベータ版|[ androidWorkProfilePkcsCertificateProfile ](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)から** subjectAlternativeNameType **プロパティーを削除しました<br/> エンティティ|
|削除|ベータ版|[ androidWorkProfileScepCertificateProfile ](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)から** subjectAlternativeNameType **プロパティーを削除しました。<br/> エンティティ|
|追加|ベータ版|[ depEnrollmentBaseProfile ](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)に** deviceNameTemplate **プロパティーを追加しました。<br/> エンティティ|
|追加|ベータ版|[ importedWindowsAutopilotDeviceIdentity ](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)に** importId **プロパティーを追加しました。<br/> エンティティ|
|追加|ベータ版|**autoLaunchItems**, **adminShowHostInfo**, **loginWindowText**, **authorizedUsersListHidden**, **authorizedUsersListHideLocalUsers**, **authorizedUsersListHideMobileAccounts**, **authorizedUsersListIncludeNetworkUsers**, **authorizedUsersListHideAdminUsers**, **authorizedUsersListShowOtherManagedUsers**, **shutDownDisabled**, **restartDisabled**, **sleepDisabled**, **consoleAccessDisabled**, **shutDownDisabledWhileLoggedIn**, **restartDisabledWhileLoggedIn**, **powerOffDisabledWhileLoggedIn**, **logOutDisabledWhileLoggedIn**および[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)への**screenLockDisableImmediate**プロパティを追加しました。<br/> エンティティ|
|追加|ベータ版|[ mobileApp ](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)に** dependentAppCount **プロパティーを追加しました。<br/> エンティティ|
|追加|ベータ版|[ win32LobApp ](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)に** requirementsRules **プロパティーを追加しました。<br/> エンティティ|
|削除|ベータ版|[ windows10CompliancePolicy ](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)から** tpmRequired **プロパティーを削除しました。<br/> エンティティ|
|追加|ベータ版|[ windowsAutopilotDeviceIdentity ](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)に** groupTag **プロパティーを追加しました。<br/> エンティティ|
|追加|ベータ版|[ managedDevice ](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)に** users **ナビゲーションプロパティーを追加しました。<br/> エンティティ|
|追加|ベータ版|[mobileApp ](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)に**relationships**ナビゲーションプロパティを追加しました。<br/> エンティティ|
|追加|ベータ版|[ intuneBrand ](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta)に** customPrivacyMessage **プロパティーを追加しました。<br/> 複合型|
|追加|ベータ版|**dependencyFailedToInstall**, **dependencyWithRequirementsNotMet**, **dependencyPendingReboot**, **dependencyWithAutoInstallDisabled**, **autoInstallDisabled**, **installingDependencies**, **powerShellScriptRequirementNotMet**, **registryRequirementNotMet**および[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)への **fileSystemRequirementNotMet**メンバーを追加しました。<br/> enum type|
|追加|ベータ版|[ win32LobAppFileSystemDetectionType ](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)に** doesNotExist **メンバーを追加しました。<br/> enum type|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[deviceManagementAbstractComplexSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementAbstractComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance?view=graph-rest-beta)<br/>[deviceManagementBooleanSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementbooleansettinginstance?view=graph-rest-beta)<br/>[deviceManagementCollectionSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementcollectionsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementCollectionSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementcollectionsettinginstance?view=graph-rest-beta)<br/>[deviceManagementComplexSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementcomplexsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementcomplexsettinginstance?view=graph-rest-beta)<br/>[deviceManagementIntegerSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementintegersettinginstance?view=graph-rest-beta)<br/>[deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta)<br/>[deviceManagementIntentAssignment](/graph/api/resources/intune-deviceintent-devicemanagementintentassignment?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceSettingStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceState](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicestate?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicestatesummary?view=graph-rest-beta)<br/>[deviceManagementIntentSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementintentsettingcategory?view=graph-rest-beta)<br/>[deviceManagementIntentUserState](/graph/api/resources/intune-deviceintent-devicemanagementintentuserstate?view=graph-rest-beta)<br/>[deviceManagementIntentUserStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementsettingcategory?view=graph-rest-beta)<br/>[deviceManagementSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementsettinginstance?view=graph-rest-beta)<br/>[deviceManagementStringSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementstringsettinginstance?view=graph-rest-beta)<br/>[deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)<br/>[deviceManagementTemplateSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementtemplatesettingcategory?view=graph-rest-beta)<br/>[securityBaselineDeviceState](/graph/api/resources/intune-deviceintent-securitybaselinedevicestate?view=graph-rest-beta)<br/>[securityBaselineSettingState](/graph/api/resources/intune-deviceintent-securitybaselinesettingstate?view=graph-rest-beta)<br/>[securityBaselineState](/graph/api/resources/intune-deviceintent-securitybaselinestate?view=graph-rest-beta)<br/>[securityBaselineStateSummary](/graph/api/resources/intune-deviceintent-securitybaselinestatesummary?view=graph-rest-beta)<br/>[securityBaselineTemplate](/graph/api/resources/intune-deviceintent-securitybaselinetemplate?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[deviceManagementConstraint](/graph/api/resources/intune-deviceintent-devicemanagementconstraint?view=graph-rest-beta)<br/>[deviceManagementEnumConstraint](/graph/api/resources/intune-deviceintent-devicemanagementenumconstraint?view=graph-rest-beta)<br/>[deviceManagementEnumValue](/graph/api/resources/intune-deviceintent-devicemanagementenumvalue?view=graph-rest-beta)<br/>[deviceManagementSettingBooleanConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingbooleanconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingDependency](/graph/api/resources/intune-deviceintent-devicemanagementsettingdependency?view=graph-rest-beta)<br/>[deviceManagementSettingIntegerConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingintegerconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingRegexConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingregexconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingStringLengthConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingstringlengthconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingXmlConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingxmlconstraint?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[deviceManangementIntentValueType](/graph/api/resources/intune-deviceintent-devicemanangementintentvaluetype?view=graph-rest-beta)<br/>[securityBaselineComplianceState](/graph/api/resources/intune-deviceintent-securitybaselinecompliancestate?view=graph-rest-beta)<br/>|
|追加|ベータ版|[deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)に対する[createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) アクションを追加しました。 |
|追加|ベータ版|[deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta)に対する[updateSettings](/graph/api/intune-deviceintent-devicemanagementintent-updatesettings?view=graph-rest-beta) アクションを追加しました。 |
|追加|ベータ版|[deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta)に対する [assign](/graph/api/intune-deviceintent-devicemanagementintent-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに**intents**、 **settingDefinitions**、**templates** および **categories** ナビゲーション プロパティを追加しました。|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)エンティティに**securityBaselineStates** ナビゲーション プロパティを追加しました。|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |v1.0 | [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0) リソースに対するアプリケーション アクセス許可のサポートを追加しました。|
|追加 |v1.0| [channel](/graph/api/resources/channel?view=graph-rest-1.0) に、**email** および **webUrl** プロパティを追加しました。|
| 追加 | ベータ版 | [チャット](/api-reference/beta/resources/chat.md) リソースと関連メソッドが追加されました。 |
| 追加 | ベータ版 | [conversation member](/api-reference/beta/resources/conversationmember.md) リソースと関連メソッドが追加されました。 |

### <a name="onedrive-and-sharepoint-apis"></a>OneDrive と SharePoint の API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | **analytics**プロパティを[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)エンティティに追加しました。 |
| 追加        | v1.0        | **analytics**プロパティを[サイト](/graph/api/resources/site?view=graph-rest-beta)エンティティに追加しました。 |
| 追加        | v1.0        | **analytics**プロパティを[listItem](/graph/api/resources/listitem?view=graph-rest-beta)エンティティに追加しました。 |
| 追加        | v1.0        | **getActivitiesByInterval**関数を[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)エンティティに追加しました。 |
| 追加        | v1.0        | **getActivitiesByInterval**関数を[サイト](/graph/api/resources/site?view=graph-rest-beta)エンティティに追加しました。 |
| 追加        | v1.0        | **getActivitiesByInterval**関数を[リスト アイテム](/graph/api/resources/listitem?view=graph-rest-beta)エンティティに追加しました。 |
| 追加        | v1.0        | [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta)エンティティを追加しました。 |
| 追加        | v1.0        | [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta)エンティティを追加しました。 |
| 追加        | v1.0        | [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta)複合型を追加しました。 |
| 追加        | v1.0        | [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta)複合型を追加しました。 |
| 追加        | v1.0        | [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta)複合型を追加しました。 |
| 追加        | v1.0        | **アクセス**プロパティを[itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta)複合型に追加しました。 |
| 追加        | v1.0        | **location**プロパティを[itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta)複合型に追加しました。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [メッセージ一覧](/graph/api/user-list-messages?view=graph-rest-beta) と [メッセージの取得](/graph/api/message-get?view=graph-rest-beta)に、新しい[Mail.ReadBasic (プレビュー) アクセス許可](permissions-reference.md#mail-permissions)サポートが追加されました。            |
| 追加        | ベータ版          | [メッセージの MIME コンテンツを取得する](outlook-get-mime-message.md)機能が追加されました。 |
| 追加        | ベータ版          | [ファイルまたはアイテムの添付ファイルの生コンテンツを取得](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)する機能が、イベント、メッセージ、Outlook タスク、またはグループ投稿に追加されました。 |

### <a name="webhooks-change-notifications"></a>Webhook (変更通知)

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | Outlook リソースで使用可能な 2 種類のライフサイクル通知 `subscriptionRemoved` と `missed` が追加されました。 アプリのサブスクリプションによって、通知の中断を軽減するための適切なアクションを実行できます。 詳しくは、[Outlook リソースで、不足状態のサブスクリプションと通知を減らす (プレビュー)](webhooks-outlook-authz.md) をご覧ください。|


## <a name="march-2019"></a>2019 年 3 月

### <a name="directory-apis"></a>Directory API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | v1.0 | **passwordNotificationWindowInDays** と **passwordValidityPeriodInDays** プロパティを[ドメイン](/graph/api/resources/domain?view=graph-rest-1.0) リソースに追加。|
| 追加 | ベータ版および v1.0 | 追加の **complianceExpirationDateTime**、**profileType** と **systemLabels** のプロパティを[デバイス](/graph/api/resources/device?view=graph-rest-1.0)リソースに追加。|
| 追加 | ベータ版および v1.0 | **isResourceAccount** プロパティを[ユーザー](/graph/api/resources/user?view=graph-rest-1.0)リソースに追加。|

### <a name="dynamics-365-business-central-api"></a>Dynamics 365 Business Central の API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | Dynamics 365 Business Central の財務 API を追加しました。 詳細については、[財務 API のリファレンス](/graph/api/resources/dynamics-graph-reference?view=graph-rest-v1.0)を参照してください。|

### <a name="education-apis"></a>教育機関 API
| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | 新しい [educationCategory](/graph/api/resources/educationCategory?view=graph-rest-beta) リソースを追加します。|
| 追加 | ベータ版 | API を追加して、[educationClass](/graph/api/resources/educationClass?view=graph-rest-beta) と [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta) の [educationCategory](/graph/api/resources/educationCategory?view=graph-rest-beta) リソースを管理します。|
| 追加 | ベータ版 | 新しい [educationFormResource](/graph/api/resources/educationFormResource?view=graph-rest-beta) リソースを追加します。|
| 追加 | ベータ版 | [educationAssignmentIndividualRecipient](/graph/api/resources/educationAssignmentIndividualRecipient?view=graph-rest-beta) リソースに **recipients** プロパティを追加します。|


### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[windowsFirewallRule](/graph/api/resources/intune-deviceconfig-windowsfirewallrule?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[androidManagedAppSafetyNetAppsVerificationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetappsverificationtype?view=graph-rest-beta)<br/>[androidManagedAppSafetyNetDeviceAttestationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype?view=graph-rest-beta)<br/>[windowsAutopilotDeviceType](/graph/api/resources/intune-enrollment-windowsautopilotdevicetype?view=graph-rest-beta)<br/>[windowsFirewallRuleInterfaceTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallruleinterfacetypes?view=graph-rest-beta)<br/>[windowsFirewallRuleNetworkProfileTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes?view=graph-rest-beta)<br/>[windowsFirewallRuleTrafficDirectionType](/graph/api/resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype?view=graph-rest-beta)<br/>[windowsHealthMonitoringScope](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringscope?view=graph-rest-beta)<br/>[windowsUpdateNotificationDisplayOption](/graph/api/resources/intune-deviceconfig-windowsupdatenotificationdisplayoption?view=graph-rest-beta)<br/>|
|追加|ベータ版|[importedDeviceIdentity](/graph/api/resources/intune-enrollment-importeddeviceidentity?view=graph-rest-beta) コレクションに [searchExistingIdentities](o:searchExistingIdentities:Collection(microsoft.graph.importedDeviceIdentity)) アクションを追加しました |
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) に [assignResourceAccountToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) に [unassignResourceAccountFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice?view=graph-rest-beta) アクションを追加しました |
|削除|ベータ版|次の列挙型を削除しました。<br/>**defenderScheduleScanDay**<br/>|
|追加|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに **requiredAndroidSafetyNetDeviceAttestationType**、**appActionIfAndroidSafetyNetDeviceAttestationFailed**、**requiredAndroidSafetyNetAppsVerificationType**、および **appActionIfAndroidSafetyNetAppsVerificationFailed** プロパティを追加しました|
|追加|ベータ版|[androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp?view=graph-rest-beta) エンティティに **supportsOemConfig** プロパティを追加しました|
|追加|ベータ版|[androidManagedStoreAppConfiguration](/graph/api/resources/intune-apps-androidmanagedstoreappconfiguration?view=graph-rest-beta) エンティティに **appSupportsOemConfig** プロパティを追加しました|
|追加|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **requiredAndroidSafetyNetDeviceAttestationType**、**appActionIfAndroidSafetyNetDeviceAttestationFailed**、**requiredAndroidSafetyNetAppsVerificationType**、および **appActionIfAndroidSafetyNetAppsVerificationFailed** プロパティを追加しました|
|追加|ベータ版|[depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta) エンティティに、**iCloudStorageDisabled** プロパティと **chooseYourLockScreenDisabled** プロパティを追加しました|
|追加|ベータ版|[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティに **roleScopeTagIds** プロパティを追加しました|
|追加|ベータ版|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) エンティティに **allowedOutboundClipboardSharingExceptionLength** プロパティを追加しました|
|追加|ベータ版|[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) エンティティに **fastFirstSignIn** プロパティを追加しました|
|追加|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティに **tpmRequired** プロパティを追加しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **firewallRules** プロパティを追加しました|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、**authenticationWebSignIn**、**privacyDisableLaunchExperience**、および **appManagementPackageFamilyNamesToLaunchAfterLogOn** プロパティを追加しました|
|削除|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティから **defenderScheduleScanDay** プロパティを削除しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **deviceType** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) エンティティに、**resourceName**、**skuNumber**、**systemFamily**、**azureActiveDirectoryDeviceId**、および **managedDeviceId** プロパティを追加しました|
|削除|ベータ版|[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta) エンティティから **edgeKioskResetAfterIdleTimeInMinutes** プロパティを削除しました|
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティに **userWindowsUpdateScanAccess** プロパティと **updateNotificationLevel** プロパティを追加しました|
|追加|ベータ版|[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta) 複合型に **teams** プロパティを追加しました|
|追加|ベータ版|[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta) 複合型に **autoLaunch** プロパティを追加しました|
|追加|ベータ版|[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) 複合型に **allowAccessToDownloadsFolder** プロパティを追加しました|
|追加|ベータ版|[androidDeviceOwnerRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype?view=graph-rest-beta) 列挙型に **lowSecurityBiometric** メンバーを追加しました|
|追加|ベータ版|[managedAppFlaggedReason](/graph/api/resources/intune-mam-managedappflaggedreason?view=graph-rest-beta) 列挙型に、**androidBootloaderUnlocked** および **androidFactoryRomModified** メンバーを追加しました|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|削除 |ベータ版| [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) から **deleted** プロパティを削除しました。 代わりに **deletedDateTime** を使用します。 |
| 追加 | ベータ版 | [schedule](/api-reference/beta/resources/schedule.md)、[schedulingGroup](/api-reference/beta/resources/schedulinggroup.md)、[shift](/api-reference/beta/resources/shift.md)、[timeOffReason](/api-reference/beta/resources/timeoffreason.md)、[timeOff](/api-reference/beta/resources/timeoff.md) のリソースと関連するメソッドを追加しました。 |

### <a name="onedrive-and-sharepoint-apis"></a>OneDrive と SharePoint の API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [driveItem](/graph/api/resources/driveItem?view=graph-rest-1.0) エンティティに **subscriptions** ナビゲーション プロパティを追加しました |
| 追加        | ベータ版        | [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) DateTimeOffset 型に **expirationDateTime** プロパティを追加しました。 |
| 追加        | ベータ版        | [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) 文字列型に **password** プロパティを追加しました。 |

### <a name="outlook-calendar"></a>Outlook カレンダー
| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 | v1.0 | [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) アクション、および [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-1.0)、[scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-1.0)、[scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-1.0) 複合型が追加され、[ユーザーの空き時間情報、配布リスト、および一定期間のリソースの取得](outlook-get-free-busy-schedule.md)がサポートされるようになりました。 |
|変更 | ベータ版 | [2019 年 2 月](#february-2019)に文書化された [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) に関連する種類の変更をロールバックしました。 特定の変更は、次の行に一覧表示されます。|
|変更 | ベータ版 | 次の [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) のパラメーターのデータ型を変更しました。 <br>**attendees**: **attendeeDataModel** から [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-beta) に戻す <br>**locationConstraint**: **locationConstraints** から [locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-beta) に戻す <br> **timeConstraint**: **findMeetingTimesTimeConstraints** から [timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-beta) に戻す|
|変更 | ベータ版 | **findMeetingTimes** の戻り値の型を **findMeetingTimesResponse** から [meetingTimeSuggestionsResult](/graph/api/resources/meetingTimeSuggestionsResult?view=graph-rest-beta) に戻しました |
|変更 | ベータ版 | [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) の基本型を **locationDataModel** から [location](/graph/api/resources/location?view=graph-rest-beta) に戻しました |
|変更 | ベータ版 | 次の [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) のプロパティのデータ型を変更しました。 <br> **attendeeAvailability**: **attendeeAvailabilityDataModel** のコレクションから [attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-beta) のコレクションに戻す <br> **locations**: **locationDataModel** のコレクションから[location](/graph/api/resources/location?view=graph-rest-beta) のコレクションに戻す <br> **meetingTimeSlot**: **meetingTimeSlotDataModel** から [timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) に戻す <br> **organizerAvailability**: **availabilityStatus** から **freeBusyStatus** に戻す |
|削除 | ベータ版 | 複合型: <br> **attendeeAvailabilityDataModel** <br> **attendeeDataModel** <br> **findMeetingTimesResponse** <br> **findMeetingTimesTimeConstraints** <br> **locationConstraints** <br> **meetingTimeSlotDataModel** <br> **searchWindowTimeSlot**|
|削除 | ベータ版 | 列挙型: <br> **addressType** <br> **availabilityStatus** |
|追加 | ベータ版 | 次の複合型を復元しました。 <br> [attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-beta) <br> [locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-beta) <br> [meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-beta) <br>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-beta) |

### <a name="risky-users-api"></a>リスクの高いユーザーの API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |ベータ版| 導入された[riskyUsers が侵害された事を確認する](/graph/api/resources/riskyusers-confirmcompromised?view=graph-rest-beta)方法で、管理者は Azure AD Identity Protection によりユーザーが侵害されていることを確認することができます。 |
|追加 |ベータ版| 導入された[riskyUsers を無視する](/graph/api/resources/riskyusers-dismiss?view=graph-rest-beta)方法で、管理者は Azure Active Directory Identity Protection によりリスクの高いユーザーを無視することができます。 |
|追加 |ベータ版| **isProcessing** プロパティを [riskyUser](/graph/api/resources/riskyuser?view=graph-rest-beta) リソースに導入しました。 |


## <a name="february-2019"></a>2019 年 2 月

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | v1.0 | 新しいリソースの種類 [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-1.0) を追加します。 |
| 追加 | ベータ版および v1.0 | **createdDateTime** プロパティを [organization](/graph/api/resources/organization?view=graph-rest-1.0) に追加します。 |
| 変更 | ベータ版および v1.0 | 書き込み可能になるように、[user](/graph/api/resources/user?view=graph-rest-1.0) リソースの **companyName** プロパティを更新しました。 |
| 変更 | ベータ版 | [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta) の種類には以前は派生型で使用可能だったものの、現在はサポートされていないプロパティが含まれています。 |
| 削除 | ベータ版 | 次の派生型はすでにサポートされておらず、削除されました:**targetResourceDevice**、**targetResourceDirectory**、**targetResourceGroup**、**targetResourcePolicy**、**targetResourceRole**、**targetResourceServicePrincipal**、**targetResourceUser**、**targetResourceOther**。 |
| 追加 |ベータ版 | **passwordNotificationWindowInDays** と **passwordValidityPeriodInDays** プロパティを[ドメイン](/graph/api/resources/domain?view=graph-rest-beta) リソースに追加してください。|

### <a name="dynamics-365-business-central-api"></a>Dynamics 365 Business Central の API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | Dynamics 365 Business Central の財務 API を追加しました。 詳細については、[財務 API のリファレンス](/graph/api/resources/dynamics-graph-reference?view=graph-rest-v1.0)を参照してください。|

### <a name="education-apis"></a>教育機関 API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |ベータ版|relatedContacts という新しいプロパティを [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta) に導入しました。|
|追加 |v1.0|relatedContacts という新しいプロパティを [educationUser](/graph/api/resources/educationUser?view=graph-rest-v1.0) に導入しました。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidOmaCpConfiguration](/graph/api/resources/intune-deviceconfig-androidomacpconfiguration?view=graph-rest-beta)<br/>[managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[deliveryOptimizationBandwidth](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidth?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthBusinessHoursLimit](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthHoursWithPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthhourswithpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdCustom](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidcustom?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSource](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsource?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSourceOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsourceoptions?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSize](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesize?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizeAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizeabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizePercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizepercentage?view=graph-rest-beta)<br/>[encryptionReportPolicyDetails](/graph/api/resources/intune-deviceconfig-encryptionreportpolicydetails?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[advancedBitLockerState](/graph/api/resources/intune-deviceconfig-advancedbitlockerstate?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdOptionsType](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype?view=graph-rest-beta)<br/>[deliveryOptimizationRestrictPeerSelectionByOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions?view=graph-rest-beta)<br/>[deviceTypes](/graph/api/resources/intune-deviceconfig-devicetypes?view=graph-rest-beta)<br/>[edgeKioskModeRestrictionType](/graph/api/resources/intune-deviceconfig-edgekioskmoderestrictiontype?view=graph-rest-beta)<br/>[encryptionReadinessState](/graph/api/resources/intune-deviceconfig-encryptionreadinessstate?view=graph-rest-beta)<br/>[encryptionState](/graph/api/resources/intune-deviceconfig-encryptionstate?view=graph-rest-beta)<br/>|
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) エンティティに **roleScopeTagIds** プロパティを追加しました|
|追加|ベータ版|[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **autoFillForceAuthentication**、**cellularBlockPlanModification**、**classroomForceAutomaticallyJoinClasses**、**classroomForceUnpromptedAppAndDeviceLock**、**esimBlockModification**、**proximityBlockSetupToNewDevice**、**softwareUpdatesEnforcedDelayInDays**、**softwareUpdatesForceDelayed** の各プロパティを追加しました|
|追加|ベータ版|[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **softwareUpdatesEnforcedDelayInDays**、**softwareUpdatesForceDelayed**、**contentCachingBlocked** の各プロパティを追加しました|
|追加|ベータ版|[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta) エンティティに **licensingType** プロパティを追加しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **defenderSecurityCenterDisableClearTpmUI**、**defenderSecurityCenterDisableNotificationAreaUI**、**defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI**、**defenderAdobeReaderLaunchChildProcess**、**defenderOfficeCommunicationAppsLaunchChildProcess** の各プロパティを追加しました|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **edgeKioskModeRestriction**、**edgeKioskResetAfterIdleTimeInMinutes**、**defenderScheduleScanEnableLowCpuPriority**、**defenderDisableCatchupQuickScan**、**defenderDisableCatchupFullScan**、**edgeBlockSearchEngineCustomization** の各プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **enableWhiteGlove** プロパティを追加しました|
|追加|ベータ版|[windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta) エンティティに **restrictPeerSelectionBy**、**groupIdSource**、**bandwidthMode**、**backgroundDownloadFromHttpDelayInSeconds**、**foregroundDownloadFromHttpDelayInSeconds**、**minimumRamAllowedToPeerInGigabytes**、**minimumDiskSizeAllowedToPeerInGigabytes**、**minimumFileSizeToCacheInMegabytes**、**minimumBatteryPercentageAllowedToUpload**、**modifyCacheLocation**、**maximumCacheAgeInDays**、**maximumCacheSize**、**vpnPeerCaching** の各プロパティを追加しました|
|追加|ベータ版|[windowsInformationProtectionWipeAction](/graph/api/resources/intune-mam-windowsinformationprotectionwipeaction?view=graph-rest-beta) エンティティに **lastCheckInDateTime** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **managedDeviceEncryptionStates** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta) 複合型に **endpointProtection** プロパティと **officeApps** プロパティを追加しました|
|追加|ベータ版|[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta) 複合型に **productName** プロパティと **publisher** プロパティを追加しました|
|追加|ベータ版|[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta) 列挙型に **warn** メンバーを追加しました|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |ベータ版および v1.0| **internalId** プロパティを[チーム](/graph/api/resources/team?view=graph-rest-v1.0)のリソースに追加しました。|
|追加 |ベータ版および v1.0| Word、Excel、PowerPoint、PDF、およびドキュメント ライブラリの[タブ](teams-configuring-builtin-tabs.md)の設定に対するサポートを追加しました。 |
|追加 |ベータ版| [チャネルへのメッセージの送信](/graph/api/channel-post-chatmessage?view=graph-rest-beta) API を導入しました。 |
|追加 |ベータ版| [チャネル内のメッセージへの返信](/graph/api/channel-post-messagereply?view=graph-rest-beta) API を導入しました。 |
|削除 |ベータ版| POST /teams/{id}/channels/{id}/chatThreads API は削除されました。 代わりに[チャネル内のメッセージの作成](/graph/api/channel-post-chatmessage?view=graph-rest-beta)を使用してください。 |
|追加 |ベータ版 | [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) リソースに対するアプリケーション アクセス許可のサポートを追加しました。|

### <a name="onedrive-and-sharepoint-apis"></a>OneDrive と SharePoint の API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) DateTimeOffset 型に **expirationDateTime** プロパティを追加しました。 |
| 追加        | ベータ版        | [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta) 文字列型に **password** プロパティを追加しました。 |

### <a name="onenote"></a>OneNote

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版および v1.0 | [getNotebookFromWebUrl](/graph/api/notebook-getnotebookfromweburl?view=graph-rest-1.0) メソッドを追加しました。 |

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|変更 | ベータ版 | 次の [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta) のパラメーターのデータ型を変更しました。 <br>**attendees**:**attendeeBase** から [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) に変更 <br>**locationConstraint**:**locationConstraint** から [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) に変更 <br> **timeConstraint**:**timeConstraint** から [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta) に変更|
|変更 | ベータ版 | **findMeetingTimes** の戻り値の型を **meetingTimeSuggestionsResult** から [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) に変更しました |
|変更 | ベータ版 | 出席者が必須なのか任意なのか、またはリソースであるかどうかを識別する各出席者の**型**を除外するため、**findMeetingTimes** の応答ペイロードを変更しました |
|変更 | ベータ版 | [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) の基本型を [location](/graph/api/resources/location?view=graph-rest-beta) から [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) に変更しました |
|変更 | ベータ版 | 次の [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) のプロパティのデータ型を変更しました。 <br> **attendeeAvailability**:**attendeeAvailability** のコレクションから [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) のコレクションに変更 <br> **locations**:[location](/graph/api/resources/location?view=graph-rest-beta) のコレクションから[locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) のコレクションに変更 <br> **meetingTimeSlot**:[timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta)から[meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) に変更 <br> **organizerAvailability**:**freeBusyStatus** から **availabilityStatus** に変更 |
|追加 | ベータ版 | 新しい複合型: <br> [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br> [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) <br> [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta) <br> [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> [PostalAddress](/graph/api/resources/postaladdress?view=graph-rest-beta) <br> [searchWindowTimeSlot](/graph/api/resources/searchwindowtimeslot?view=graph-rest-beta)|
|追加 | ベータ版 | 新しい列挙体: <br> **addressType** <br> **availabilityStatus** |
|追加 | ベータ版 | **order** プロパティを [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) に追加しました |
|削除 | ベータ版 | 次の複合型を削除しました。 <br> **attendeeAvailability** <br> **locationConstraint** <br> **meetingTimeSuggestionsResult** <br>**timeConstraint** |

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | 脅威インテリジェンス (TI) インジケーター API を [セキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-beta) に追加しました。これには次のリソースと操作が含まれています。<br/>[tiindicator](/graph/api/resources/tiindicator?view=graph-rest-beta) (および関連するエンティティ)<br/> [Get tiIndicator](/graph/api/tiindicator-get?view=graph-rest-beta)<br/>[Create tiIndicator](/graph/api/tiindicators-post?view=graph-rest-beta)<br/>[List tiIndicators](/graph/api/tiindicators-list?view=graph-rest-beta)<br/>[Update tiIndicator](/graph/api/tiindicator-update?view=graph-rest-beta) <br/>[Delete tiIndicator](/graph/api/tiindicator-delete?view=graph-rest-beta) <br/>[deleteTiIndicators](/graph/api/tiindicator-deletetiindicators?view=graph-rest-beta) <br/>[deleteTiIndicatorsByExternalId](/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta) <br/>[submitTiIndicators](/graph/api/tiindicator-submittiindicators?view=graph-rest-beta) <br/>[updateTiIndicators](/graph/api/tiindicator-updatetiindicators?view=graph-rest-beta)|
| 追加        | ベータ版       | セキュリティ アクション API を [セキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-beta) に追加しました。これには次のリソースと操作が含まれています。<br/>[securityAction](/graph/api/resources/securityaction?view=graph-rest-beta) (および関連するエンティティ)<br/> [Get securityAction](/graph/api/securityaction-get?view=graph-rest-beta)<br/>[Create securityAction](/graph/api/securityactions-post?view=graph-rest-beta)<br/>[List securityAction](/graph/api/securityactions-list?view=graph-rest-beta)<br/>[Cancel securityAction](/graph/api/securityaction-cancelsecurityaction?view=graph-rest-beta)
| 追加        | ベータ版        | 新しい複合型 [historyStates](/graph/api/resources/alerthistorystate?view=graph-rest-beta) コレクションをアラートに導入しました。 </br>1 つの要求で複数のアラートを更新する [updateAlerts](/graph/api/alert-updatealerts?view=graph-rest-beta) 機能を追加しました。 |

## <a name="january-2019"></a>2019 年 1 月

### <a name="azure-ad-b2c-apis"></a>Azure AD B2C APIs

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |v1.0|新しいリソースの種類である [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-v1.0) エンティティと、[作成](/graph/api/identityprovider-post-identityproviders?view=graph-rest-v1.0)、[一覧表示](/graph/api/identityprovider-list?view=graph-rest-v1.0)、[取得](/graph/api/identityprovider-get?view=graph-rest-v1.0)、[更新](/graph/api/identityprovider-update?view=graph-rest-v1.0)、[削除](/graph/api/identityprovider-delete?view=graph-rest-v1.0)の各操作を導入しました。|

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | v1.0 | transitiveMembers という新しいメソッドを[グループ](/graph/api/group-list-transitivemembers?view=graph-rest-1.0)に追加しました。 このメソッドでは、入れ子になったメンバーを含むメンバーのフラット リストが返されます。|
| 追加 | v1.0 | [ユーザー](/graph/api/user-list-transitivemembersof?view=graph-rest-1.0)、[グループ](/graph/api/group-list-transitivemembersof?view=graph-rest-beta)、[デバイス](/graph/api/device-list-transitivemembersof?view=graph-rest-1.0)に transitiveMemberOf という新しいメソッドを追加しました。|
| 追加 | v1.0 | **employeeId**、**faxNumber**、**onPremisesDistinguishedName**、**showInAddressList**、**otherMails** という新しいプロパティを[ユーザー](/graph/api/resources/user?view=graph-rest-1.0)に追加しました。|
| 追加 | v1.0 | **forceChangePasswordNextSignInWithMfa** プロパティを [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-v1.0) 複合型に追加しました。|
| 追加 | v1.0 | [グループベースのライセンス](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)の [User](/graph/api/resources/user?view=graph-rest-1.0) エンティティに、**licenseAssignmentStates** プロパティを追加しました。|
| 追加 | v1.0 | [グループベースのライセンス](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)の **licenseAssignmentState** リソースを追加しました。| 
| 追加 | v1.0 | [グループベースのライセンス](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)の [Group](/graph/api/resources/group?view=graph-rest-1.0) エンティティに、**assignedLicenses** プロパティ、**licenseProcessingState** プロパティ、**hasMembersWithLicenseErrors** プロパティ、**membersWithLicenseErrors** リレーションシップを追加しました。|
| 追加 | ベータ版 | **createdDateTime** プロパティを [user](/graph/api/resources/user?view=graph-rest-beta) リソースに追加しました。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[appleVppTokenTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-applevpptokentroubleshootingevent?view=graph-rest-beta)<br/>[appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta)<br/>[windowsUpdateState](/graph/api/resources/intune-deviceconfig-windowsupdatestate?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[appLogCollectionDownloadDetails](/graph/api/resources/intune-devices-applogcollectiondownloaddetails?view=graph-rest-beta)<br/>**deviceManagementTroubleshootingErrorDetails**<br/>[deviceManagementTroubleshootingErrorResource](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource?view=graph-rest-beta)<br/>[win32LobAppAssignmentSettings](/graph/api/resources/intune-apps-win32lobappassignmentsettings?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[appLogDecryptionAlgorithm](/graph/api/resources/intune-devices-applogdecryptionalgorithm?view=graph-rest-beta)<br/>[appLogUploadState](/graph/api/resources/intune-devices-apploguploadstate?view=graph-rest-beta)<br/>[win32LobAppNotification](/graph/api/resources/intune-apps-win32lobappnotification?view=graph-rest-beta)<br/>[windowsUpdateStatus](/graph/api/resources/intune-deviceconfig-windowsupdatestatus?view=graph-rest-beta)<br/>|
|追加|ベータ版|**createDownloadUrl** アクションを[appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta) に追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**deviceManagementApplicabilityRuleOsEdition**<br/>**deviceManagementApplicabilityRuleOsVersion**<br/>|
|追加|ベータ版|**passwordSignInFailureCountBeforeFactoryReset** プロパティを [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**passwordSignInFailureCountBeforeFactoryReset** プロパティを [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**passwordSignInFailureCountBeforeFactoryReset** プロパティを [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) エンティティに追加しました|
|削除|ベータ版|**defaultProfileDisplayName** プロパティを [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) エンティティから削除しました|
|追加|ベータ版|**runAs32Bit** プロパティを [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**troubleshootingErrorDetails** プロパティ、**eventName** プロパティ、および **additionalInformation** プロパティを [deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta) エンティティに追加しました|
|変更|ベータ版|[macOSCertificateProfileBase](/graph/api/resources/intune-deviceconfig-macoscertificateprofilebase?view=graph-rest-beta) エンティティで次のプロパティを変更しました。<br/>**subjectAlternativeNameType**を必須からオプションに変更しました<br/>|
|追加|ベータ版|**certificateStore** プロパティおよび **customSubjectAlternativeNames** プロパティを [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**officeConfigurationXml** プロパティを [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**createdDateTime** プロパティを [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**bitLockerAllowStandardUserEncryption** プロパティを [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに追加しました|
|削除|ベータ版|**localSecurityOptionsEnableAdministratorAccount** プロパティ、**localSecurityOptionsEnableGuestAccount** プロパティ、および **lanManagerWorkstationEnableInsecureGuestLogons** プロパティを [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティから削除しました|
|追加|ベータ版|**useSecurityKeyForSignin**プロパティを[windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**mobileAppTroubleshootingEvents** ナビゲーション プロパティを [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに追加しました|
|追加|ベータ版|**appLogCollectionRequests** ナビゲーション プロパティを [mobileAppTroubleshootingEvent](/graph/api/resources/intune-devices-mobileapptroubleshootingevent?view=graph-rest-beta) エンティティに追加しました|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |ベータ版| EducationStandard、educationClass、educationProfessionalLearningCommunity、educationStaff、unknownFutureValue を [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) 列挙値に追加しました。|

### <a name="reports-apis"></a>レポート API

| **変更の種類** | **バージョン** | **説明**                  |
|:----------------|:------------|:-----------------------------------------|
| 追加        | ベータ版  | **office365Active** プロパティおよび **office365Inactive** プロパティを [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta) エンティティに追加しました。|

## <a name="december-2018"></a>2018 年 12 月

### <a name="data-policy-api"></a>データ ポリシー API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|追加 |v1.0| 新しいエンティティ [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-1.0) を追加しました。 これは、追跡のために送信されたデータ ポリシー操作を表します。
|追加 |v1.0| [users](/graph/api/resources/users?view=graph-rest-1.0) に [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-1.0) アクションを追加しました。 このアクションは、Microsoft がユーザー用に保存している個人データをエクスポートするためのデータ ポリシー操作要求を送信します。 |
|追加 |v1.0| メソッド [dataPolicyOperations](/graph/api/datapolicyoperation-get?view=graph-rest-1.0) を追加しました。 これは dataPolicyOperation オブジェクトのプロパティを取得します。|

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | 
  [グループ](https://docs.microsoft.com/ja-JP/graph/api/group-list-transitivemembers?view=graph-rest-beta)に、[グループの有効期限](https://docs.microsoft.com/ja-JP/azure/active-directory/users-groups-roles/groups-lifecycle)に関する新しいプロパティ `expirationDateTime` を追加しました。|
| 追加 | ベータ版 | 新しいリソースの種類 [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta) を追加します。|
| 追加 | ベータ版 | [organization](/graph/api/resources/organization?view=graph-rest-beta) リソースに `createdDateTime` プロパティを追加しました。|
| 追加 | v1.0 | [デバイス](/graph/api/resources/device?view=graph-rest-1.0)のダイレクト [メンバーシップ](/graph/api/device-list-memberOf?view=graph-rest-1.0)を取得する `memberOf` メソッドを追加しました。 このメソッドは、入れ子になったメンバーシップを含むメンバーシップのリストを取得するために追加されました。|
| 変更    | ベータ版 | [組織の連絡先](/graph/api/resources/orgcontact?view=graph-rest-beta)のリソースを再構成しました。 物理アドレスのプロパティ (`city`、`country`、`postalCode`、`streetAddress`、`state`) と `officeLocation` が `addresses` コレクション (新しい [physicalOfficeAddress](/graph/api/resources/physicalofficeaddress?view=graph-rest-beta) リソース タイプ) に含められ、`mobilePhone`、`businessPhones`、`faxNumber` が `phones` コレクションに含められるようになりました。 また、`companyName` と `imAddresses` が追加されました。|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |ベータ版| [teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta) という新しいリソースの種類を導入しました。|
|追加 |ベータ版| [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) という新しいリソースの種類を導入しました。|
|追加 |ベータ版| [channel](/graph/api/resources/channel?view=graph-rest-beta) に、isFavoriteByDefault、email、および webUrl プロパティを追加しました。|
|追加 |ベータ版| displayName プロパティを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| description プロパティを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| classification プロパティを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| [specialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) プロパティを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| [visibility](/graph/api/resources/teamvisibilitytype?view=graph-rest-beta) プロパティを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| [template](/graph/api/resources/teamstemplate?view=graph-rest-beta) プロパティを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| 所有者のコレクションを [team](/graph/api/resources/team?view=graph-rest-beta) に追加しました。|
|追加 |ベータ版| unknownFutureValue という新しい列挙メンバーを teamVisibilityType に導入しました。|
|追加 |ベータ版| unknownFutureValue という新しい列挙メンバーを giphyRatingType に導入しました。|
|追加 |ベータ版| unknownFutureValue という新しい列挙メンバーを teamsAsyncOperationType に導入しました。|
|追加 |ベータ版| unknownFutureValue という新しい列挙メンバーを teamsAsyncOperationStatus に導入しました。|
|追加 |ベータ版| unknownFutureValue という新しい列挙メンバーを teamsAppDistributionMethod に導入しました。|
|追加 |ベータ版| [/teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta) という新しいリソースを導入しました。|
|追加 | v1.0 | 管理者のアクセス許可のサポートを [team](/graph/api/resources/team?view=graph-rest-1.0)、[channel](/graph/api/resources/channel?view=graph-rest-1.0)、および [tab](/graph/api/resources/teamstab?view=graph-rest-1.0) 操作に追加しました。 |

### <a name="privileged-identity-management-apis"></a>Privileged Identity Management API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) エンティティにプロパティ `registeredRoot` を追加しました。|
| 変更 | ベータ版 | [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) エンティティのプロパティ `onboardDateTime` を `registeredDateTime` に名前変更しました。|
| 追加 | ベータ版 | 新しいアクション [register resource](/graph/api/governanceresource-register?view=graph-rest-beta) を追加しました。|
| 削除 | ベータ版 | [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) エンティティの `isPermanent` プロパティを削除しました。|
| 削除 | ベータ版 | [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) エンティティの `roleAssignmentStartDateTime` プロパティを削除しました。|
| 削除 | ベータ版 | [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) エンティティの `roleAssignmentEndDateTime` プロパティを削除しました。|

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [complianceInformation](/graph/api/complianceInformation/team?view=graph-rest-beta) という新しい複合型を導入しました。|
| 追加        | ベータ版        | [certificationControl](/graph/api/certificationControl/team?view=graph-rest-beta) という新しい複合型を導入しました。|

## <a name="november-2018"></a>2018 年 11 月

### <a name="data-policy-operations-api"></a>データ ポリシー操作 API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [dataPolicyOperation](/graph/api/resources/dataPolicyOperation?view=graph-rest-beta) に新しい **progress** プロパティを追加しました。 これは、操作の進捗状況を指定します。

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | v1.0 | [ドメイン](/graph/api/resources/domain?view=graph-rest-1.0)に [forceDelete](/graph/api/domain-forcedelete?view=graph-rest-1.0) アクションを追加しました。|
| 追加 | ベータ版 | transitiveMembers という新しいメソッドを[グループ](/graph/api/group-list-transitivemembers?view=graph-rest-beta)に追加しました。 このメソッドでは、入れ子になったメンバーを含むメンバーのフラット リストが返されます。|
| 追加 | ベータ版 | [ユーザー](/graph/api/user-list-transitivemembersof?view=graph-rest-beta)、[グループ](/graph/api/group-list-transitivemembersof?view=graph-rest-beta)、[デバイス](/graph/api/device-list-transitivemembersof?view=graph-rest-beta)、および[サービス プリンシパル](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta)に transitiveMemberOf という新しいメソッドを追加しました。|
| 追加 | ベータ版 | デバイスのダイレクト [メンバーシップ](/graph/api/device-list-members?view=graph-rest-beta)を取得する memberOf メソッドを追加しました。 このメソッドは、入れ子になったメンバーシップを含むメンバーシップのリストを取得するために追加されました。|
| 追加 | ベータ版 | **faxNumber**、**onPremisesDistinguishedName**、および **otherMails[ という新しいプロパティを](/graph/api/resources/user?view=graph-rest-beta)ユーザー**に追加しました。|
| 追加 | ベータ版 | **forceChangePasswordNextSignInWithMfa** プロパティを [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-beta) 複合型に追加しました。|
| 追加    | ベータ版 | 'externalUserState' および 'externalUserStateChangeDateTime' プロパティを [user](/graph/api/resources/user?view=graph-rest-beta) オブジェクトに追加しました。|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |v1.0| [team](/graph/api/resources/team?view=graph-rest-1.0) という新しいリソースの種類を導入しました。|
|追加 |v1.0| [channel](/graph/api/resources/channel?view=graph-rest-1.0) という新しいリソースの種類を導入しました。|
|追加 |v1.0| [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-1.0) という新しいリソースの種類を導入しました。|
|追加 |v1.0| [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-1.0) という新しいリソースの種類を導入しました。|
|追加 |v1.0| [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0) という新しいリソースの種類を導入しました。|
|追加 |v1.0| [teamsAsyncOperation](/graph/api/resources/teamsasyncoperation?view=graph-rest-1.0) という新しいリソースの種類を導入しました。 |
|追加 |v1.0| [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-1.0) という新しい複合型を導入しました。 |
|追加 |v1.0| [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-1.0) という新しい複合型を導入しました。 |
|追加 |v1.0| [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-1.0) という新しい複合型を導入しました。 |
|追加 |v1.0| [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-1.0) という新しい複合型を導入しました。 |
|追加 |v1.0| [チームの複製](/graph/api/team-clone?view=graph-rest-1.0)という新しいアクションを導入しました。 |
|追加 |v1.0| [チームのアーカイブ](/graph/api/team-archive?view=graph-rest-1.0)という新しいアクションを導入しました。|
|追加 |v1.0| [チームのアーカイブ解除](/graph/api/team-unarchive?view=graph-rest-1.0)という新しいアクションを導入しました。 |
|追加         | ベータ版          | [チームの複製](/graph/api/team-clone?view=graph-rest-beta)にアプリケーション アクセス許可のサポートを追加しました。 |
|追加 |ベータ版| [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) を導入しました。これにより、ペイロードの一部が異なる /teams/{id}/apps が置き換えられます。 |
|追加 |ベータ版| [/appCatalogs/teamsApps/{id}/appDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta) を導入しました。これにより、[/appCatalogs/teamsApps/{id}](/graph/api/resources/teamsapp?view=graph-rest-beta) のバージョン プロパティが置き換えられます。 |
|変更   |ベータ版| [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) の種類の名前を teamsCatalogApp から teamsApp に変更しました。 |
|変更   |ベータ版| [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) の distributionMethod プロパティの種類の名前を teamsCatalogAppDistributionMethod から teamsAppDistributionMethod に変更しました  |
|削除 |ベータ版| teamsCatalogAppDistributionMethod が teamsAppDistributionMethod という名前に変更されました  |
|追加 |ベータ版| [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) を導入しました。これにより、ペイロードの一部が異なる /teams/{id}/apps が置き換えられます。 |
|追加 |ベータ版| displayName プロパティを [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) に追加しました |
|追加 |ベータ版| messageId プロパティを [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) に追加しました |
|追加 |ベータ版| teamsApp プロパティを [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) に追加しました |
|追加 |ベータ版| [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) という新しいリソースの種類を導入しました。|
|追加 |ベータ版| [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) という新しいリソースの種類を導入しました。|
|追加 |ベータ版| [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta) という新しいリソースの種類を導入しました。|
|追加 |ベータ版| hiddenMembership という新しい列挙メンバーを teamVisibilityType に導入しました。|
|追加 |ベータ版| createTeam という新しい列挙メンバーを teamsAsyncOperationType に導入しました。|
|追加 |ベータ版| teamsAppDistributionMethod という新しい列挙メンバーを導入しました。|
|追加 |ベータ版| [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) にアプリのアップグレードという新しいアクションを導入しました。 |

### <a name="reports-apis"></a>レポート API

| 変更の種類 | バージョン                                    | 説明                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| 追加    | 21Vianet によって運営されている Microsoft Graph China のベータ版 | 以下の API を追加しました。<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta)。 |

## <a name="october-2018"></a>2018 年 10 月

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | transitiveMembers という新しいメソッドを[グループ](/graph/api/group-list-transitivemembers?view=graph-rest-beta)に追加しました。 このメソッドでは、入れ子になったメンバーを含むメンバーのフラット リストが返されます。|
| 追加 | ベータ版 | [ユーザー](/graph/api/user-list-transitivemembersof?view=graph-rest-beta)、[グループ](/graph/api/group-list-transitivemembersof?view=graph-rest-beta)、[デバイス](/graph/api/device-list-transitivemembersof?view=graph-rest-beta)、および[サービス プリンシパル](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta)に transitiveMemberOf という新しいメソッドを追加しました。|
| 追加 | ベータ版 | デバイスのダイレクト [メンバーシップ](/graph/api/device-list-members?view=graph-rest-beta)を取得する memberOf メソッドを追加しました。 このメソッドは、入れ子になったメンバーシップを含むメンバーシップのリストを取得するために追加されました。|
| 追加 | ベータ版 | **faxNumber**、**onPremisesDistinguishedName**、および **otherMails[ という新しいプロパティを](/graph/api/resources/user?view=graph-rest-beta)ユーザー**に追加しました。|

### <a name="riskyusers-apis"></a>RiskyUsers API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加 |ベータ版| [riskyUsers API](/graph/api/resources/riskyuser?view=graph-rest-beta) を導入しました。これは、Azure AD Identity Protection によって検出される、危険な状態の Azure AD ユーザーを表します。 |


### <a name="signin-apis"></a>サインイン API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|変更   |ベータ版| `conditionalAccessPolicies` プロパティを `appliedConditionalAccessPolicy` という名前に変更しました。|
|追加 |ベータ版| `riskDetail`、`riskLevelAggregated`、`riskLevelDuringSignIn`、`riskEventTypes`、および `riskState` を含む、追加のリスク プロパティを[サインイン API](/graph/api/resources/signin?view=graph-rest-beta) に導入しました。|
|追加 |ベータ版| `authenticationProcessingDetails`、`originalRequestID`、`isInteractive`、`tokenIssuerName`、`tokenIssuerType`、`correlationId`、および `processingTimeinMilliseconds` を含む、追加のサインイン プロパティを[サインイン API](/graph/api/resources/signin?view=graph-rest-beta) に導入しました。|
|削除   |ベータ版| `isRisky` プロパティを削除しました。|

## <a name="october-2018"></a>2018 年 10 月

### <a name="delta-query"></a>デルタ クエリ

| **変更の種類** | **バージョン** | **説明**                  |
|:------------|:--------|:-----------------------------------------|
| 追加    | ベータ版   | [directoryObject](/graph/api/directoryobject-delta?view=graph-rest-beta) の[デルタ クエリ](delta-query-overview.md)機能を追加しました |
| 変更      | v1.0 およびベータ版  | [ユーザー](/graph/api/user-delta?view=graph-rest-1.0)と[グループ](/graph/api/group-delta?view=graph-rest-1.0)の JSON 応答で変更されたプロパティのみを返す代替動作。 |
| 追加    | v1.0   | [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) の[デルタ](/graph/api/directoryrole-delta?view=graph-rest-1.0)関数が追加され、[デルタ クエリを使用する変更の追跡](delta-query-overview.md)がサポートされるようになりました。 |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [グループベースのライセンス](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)の [User](/graph/api/resources/user?view=graph-rest-beta) エンティティに、**licenseAssignmentStates** プロパティを追加しました。|
| 追加 | ベータ版 | [グループベースのライセンス](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)の **licenseAssignmentState** リソースを追加しました。|
| 追加 | ベータ版 | [グループベースのライセンス](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)の [Group](/graph/api/resources/group?view=graph-rest-beta) エンティティに、**assignedLicenses**、**licenseProcessingState**、**hasMembersWithLicenseErrors**、および **membersWithLicenseErrors** プロパティを追加しました。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0) エンティティに **tenantLockdownRequireNetworkDuringOutOfBoxExperience** プロパティを追加しました。|
|追加|v1.0|[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0) 複合型に **v12_0** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **lastReportAggregationDateTime** プロパティを追加しました|
|追加|ベータ版|以下の新しいエンティティを追加しました。<br/>[intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)<br/>|
|追加|ベータ版|以下の新しい複合型を追加しました。<br/>[deviceAndAppManagementAssignedRoleIds](/graph/api/resources/intune-rbac-deviceandappmanagementassignedroleids?view=graph-rest-beta)<br/>|
|追加|ベータ版|以下の新しい列挙型を追加しました。<br/>[applicationGuardEnabledOptions](/graph/api/resources/intune-deviceconfig-applicationguardenabledoptions?view=graph-rest-beta)<br/>[autoRestartNotificationDismissalMethod](/graph/api/resources/intune-deviceconfig-autorestartnotificationdismissalmethod?view=graph-rest-beta)<br/>[meteredConnectionLimitType](/graph/api/resources/intune-deviceconfig-meteredconnectionlimittype?view=graph-rest-beta)<br/>|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) に [enableLegacyPcManagement](/graph/api/intune-deviceconfig-devicemanagement-enablelegacypcmanagement?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) に [extendFeatureUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) に [extendQualityUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) に [unassignUserFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) に [getAssignedRoleIdsForLoggedInUser](/graph/api/intune-rbac-devicemanagement-getassignedroleidsforloggedinuser?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) に [getManagedDevicesWithAppFailures](/graph/api/intune-troubleshooting-user-getmanageddeviceswithappfailures?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentAbandonmentSummary](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentsummary?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentAbandonmentDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentdetails?view=graph-rest-beta) 関数を追加しました |
|削除|ベータ版|[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta) エンティティから **subjectAlternativeNameType** プロパティを削除しました|
|追加|ベータ版|[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) エンティティに **subjectAlternativeNameType** プロパティを追加しました|
|追加|ベータ版|[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) エンティティに、**certificateStore**、**customSubjectAlternativeNames**、および **subjectAlternativeNameType** プロパティを追加しました|
|削除|ベータ版|[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta) エンティティから **subjectAlternativeNameType** プロパティを削除しました|
|追加|ベータ版|[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta) エンティティに **subjectAlternativeNameType** プロパティを追加しました|
|追加|ベータ版|[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta) エンティティに、**certificateStore**、**customSubjectAlternativeNames**、および **subjectAlternativeNameType** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **legacyPcManangementEnabled** プロパティを追加しました|
|削除|ベータ版|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) エンティティから **pinRequiredOnLaunchInsteadOfBiometric** プロパティを削除しました|
|追加|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティに **roleScopeTagIds** プロパティを追加しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **applicationGuardEnabledOptions** プロパティを追加しました|
|追加|ベータ版|[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) エンティティに **selectedMobileAppIds** プロパティを追加しました|
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティに、**engagedRestartDeadlineInDays**、**engagedRestartSnoozeScheduleInDays**、**engagedRestartTransitionScheduleInDays**、**autoRestartNotificationDismissal**、**scheduleRestartWarningInHours**、および **scheduleImminentRestartWarningInMinutes** プロパティを追加しました|
|追加|ベータ版|[windowsWifiConfiguration](/graph/api/resources/intune-deviceconfig-windowswificonfiguration?view=graph-rest-beta) エンティティに **preSharedKey** および **meteredConnectionLimit** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **intuneBrandingProfiles** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-beta) 複合型に、**v6_0**、**v7_0**、**v7_1**、**v8_0**、**v8_1**、および **v9_0** プロパティを追加しました|
|追加|ベータ版|[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta) 複合型に **v12_0** プロパティを追加しました|
|削除|ベータ版|[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta) 複合型から **runAsLoggedOnUser** プロパティを削除しました|
|追加|ベータ版|[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta) 複合型に **lastUpdateDateTime** プロパティを追加しました|
|追加|ベータ版|[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta) 複合型に **lastUpdateDateTime** プロパティを追加しました|
|追加|ベータ版|[windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta) 複合型に **lastUpdateDateTime** プロパティを追加しました|
|追加|ベータ版|[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta) 複合型に **lastUpdateDateTime** プロパティを追加しました|
|追加|ベータ版|[windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta) 複合型に **lastUpdateDateTime** プロパティを追加しました|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加|ベータ版|[チームのアーカイブ](/graph/api/team-archive?view=graph-rest-beta)および[チームのアーカイブ解除](/graph/api/team-unarchive?view=graph-rest-beta) API にアプリケーション アクセス許可のサポートを追加しました。|

### <a name="outlook-contacts"></a>Outlook の連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 削除         | v1.0        | これはドキュメントに対する修正です。[contact](/graph/api/resources/contact?view=graph-rest-1.0) エンティティのトピックから **flag** プロパティを削除しました。 このプロパティが **contact** エンティティで使用可能になったことはありません。|

### <a name="privileged-identity-management-apis"></a>特権 ID 管理 API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更 | ベータ版 | [privilegedapproval](/graph/api/resources/privilegedapproval?view=graph-rest-beta) エンティティを変更します。|
| 追加 | ベータ版 | [privilegedroleassignmentrequest](/graph/api/resources/privilegedroleassignmentrequest?view=graph-rest-beta) エンティティ、および次のメソッドとアクションを追加しました。<br> [List](/graph/api/privilegedroleassignmentrequest-list?view=graph-rest-beta) <br> [作成](/graph/api/privilegedroleassignmentrequest-post?view=graph-rest-beta) <br> [キャンセル](/graph/api/privilegedroleassignmentrequest-cancel?view=graph-rest-beta) <br> [My](/graph/api/privilegedroleassignmentrequest-my?view=graph-rest-beta) |
| 追加 | ベータ版 | [privilegedRoleSettings](/graph/api/resources/privilegedrolesettings?view=graph-rest-beta) の[更新](/graph/api/privilegedrolesettings-update?view=graph-rest-beta)を追加しました|
| 削除 |ベータ版| [自分でロールの割り当てをアクティブにする](/graph/api/privilegedrole_selfactivate?view=graph-rest-beta)を廃止しました。|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | v1.0    | [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0) に **Site ID** プロパティが追加されました。 |

## <a name="september-2018"></a>2018 年 9 月

### <a name="calls-and-online-meetings-api"></a>通話とオンライン会議の API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [application](/graph/api/resources/application?view=graph-rest-beta) リソースが更新され、通話コレクションが追加されました。 |
| 変更          | ベータ版        | [operation](/graph/api/resources/operation?view=graph-rest-beta) リソースが更新され、長時間実行される通話と会議の API がサポートされるようになりました。 |
| 追加        | ベータ版        | [通話の作成](/graph/api/application-post-calls?view=graph-rest-beta)、[通話の取得](/graph/api/call-get?view=graph-rest-beta)、[通話の削除 (電話を切る)](/graph/api/call-delete?view=graph-rest-beta)、[通話への応答](/graph/api/call-answer?view=graph-rest-beta)、[通話の拒否](/graph/api/call-reject?view=graph-rest-beta)、[通話のリダイレクト](/graph/api/call-redirect?view=graph-rest-beta)、[通話の転送](/graph/api/call-transfer?view=graph-rest-beta)用の API を含む、(最初は Microsoft Teams で) オーディオ/ビデオ通話を管理するための [call](/graph/api/resources/call?view=graph-rest-beta) リソースを追加しました。 また、[IVR シナリオ](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)をサポートするために、[プロンプトの再生](/graph/api/call-playprompt?view=graph-rest-beta)、[通話の記録](/graph/api/call-record?view=graph-rest-beta)、[メディア処理の取り消し](/graph/api/call-cancelmediaprocessing?view=graph-rest-beta)、および[タッチ トーン通知のサブスクライブ](/graph/api/call-subscribetotone?view=graph-rest-beta)用の API も追加しました。 |
| 追加        | ベータ版        | [参加者オブジェクトの取得](/graph/api/participant-get?view=graph-rest-beta)、[参加者用のオーディオ ミキサーの構成](/graph/api/participant-configuremixer?view=graph-rest-beta)、[1 人](/graph/api/participant-mute?view=graph-rest-beta)または[すべて](/graph/api/participant-muteall?view=graph-rest-beta)の参加者のミュート、通話/会議の[参加者リストの取得](/graph/api/call-list-participants?view=graph-rest-beta)、通話/会議への[参加者の招待](/graph/api/participant-invite?view=graph-rest-beta)を含む、オーディオ/ビデオ通話と会議の参加者を管理するための [participant](/graph/api/resources/call?view=graph-rest-beta) リソースと API を追加しました。 |
| 追加        | ベータ版        | [コンテンツの共有](/graph/api/call-changescreensharingrole?view=graph-rest-beta)、[それ自体のミュートとミュート解除](/graph/api/call-unmute?view=graph-rest-beta)、[通話に関連付けられているメタデータの更新](/graph/api/call-updatemetadata?view=graph-rest-beta)機能を含む、通話と会議の管理および参加のためのアプリケーションの API を追加しました。 |
| 追加        | ベータ版        | [オーディオ ルーティング グループの作成](/graph/api/call-post-audioroutinggroups?view=graph-rest-beta)、[それらのリストの取得](/graph/api/audioroutinggroup-get?view=graph-rest-beta)、[更新](/graph/api/audioroutinggroup-update?view=graph-rest-beta)および[削除](/graph/api/audioroutinggroup-delete?view=graph-rest-beta)を含む、マルチパーティ会話への参加者間のプライベート オーディオ ルートを管理するための [audio routing group](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) リソースと API を追加しました。 |
| 追加        | ベータ版        | Microsoft Teams オンライン会議を管理するための [online meeting](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) リソースと API を追加しました。 最初は、[オンライン会議のオブジェクトを取得する](/graph/api/onlinemeeting-get?view=graph-rest-beta)ための、オンライン会議の API は 1 つだけです。 会議に関連付けられている[オーディオ会議情報](/graph/api/resources/audioconferencing?view=graph-rest-beta) (ダイヤルイン URL、パスコード、電話番号など) の関連リソースも追加されました。 |
| 追加        | ベータ版        | 通話および会議 API の多くは完了するまで時間がかかるため、[通話固有の操作](/graph/api/resources/commsoperation?view=graph-rest-beta)、[オーディオ プロンプトの再生](/graph/api/resources/playpromptoperation?view=graph-rest-beta)、および[記録](/graph/api/resources/recordoperation?view=graph-rest-beta)という、長時間実行される操作のリソースが追加されました。  |

### <a name="dynamics-365-business-central-api"></a>Dynamics 365 Business Central の API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | Dynamics 365 Business Central の財務 API を追加しました。 詳細については、[財務 API のリファレンス](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)を参照してください

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph データ接続

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加         | 該当なし| 一括で Office 365 データにアクセスする機能が導入されました。 詳細については、「[Microsoft Graph データ接続の概要 (プレビュー)](data-connect-overview.md)」を参照してください。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) に [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|ベータ版|以下の新しいエンティティを追加しました。<br/>[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)<br/>[officeClientConfigurationAssignment](/graph/api/resources/intune-cirrus-officeclientconfigurationassignment?view=graph-rest-beta)<br/>[officeConfiguration](/graph/api/resources/intune-cirrus-officeconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientSecurityConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientsecurityconfiguration?view=graph-rest-beta)<br/>|
|追加|ベータ版|以下の新しい複合型を追加しました。<br/>[officeClientCheckinStatus](/graph/api/resources/intune-cirrus-officeclientcheckinstatus?view=graph-rest-beta)<br/>[officeConfigurationAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationassignmenttarget?view=graph-rest-beta)<br/>[officeConfigurationGroupAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationgroupassignmenttarget?view=graph-rest-beta)<br/>[officeUserCheckinSummary](/graph/api/resources/intune-cirrus-officeusercheckinsummary?view=graph-rest-beta)<br/>|
|追加|ベータ版|[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-cirrus-officeclientconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) コレクションに **updatePrioritie** アクションを追加しました |
|追加|ベータ版|以下の新しいエンティティを追加しました。<br/>[deviceConfigurationConflictSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationconflictsummary?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/>|
|追加|ベータ版|以下の新しい複合型を追加しました。<br/>[deviceConfigurationTargetedUserAndDevice](/graph/api/resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice?view=graph-rest-beta)<br/>[win32LobAppDetection](/graph/api/resources/intune-apps-win32lobappdetection?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetection](/graph/api/resources/intune-apps-win32lobappfilesystemdetection?view=graph-rest-beta)<br/>[win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)<br/>[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)<br/>[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)<br/>[win32LobAppProductCodeDetection](/graph/api/resources/intune-apps-win32lobappproductcodedetection?view=graph-rest-beta)<br/>[win32LobAppRegistryDetection](/graph/api/resources/intune-apps-win32lobappregistrydetection?view=graph-rest-beta)<br/>[win32LobAppReturnCode](/graph/api/resources/intune-apps-win32lobappreturncode?view=graph-rest-beta)<br/>[windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10appsforceupdateschedule?view=graph-rest-beta)<br/>|
|追加|ベータ版|以下の新しい列挙型を追加しました。<br/>[administratorConfiguredDeviceComplianceState](/graph/api/resources/intune-deviceconfig-administratorconfigureddevicecompliancestate?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[microsoftStoreForBusinessPortalSelectionOptions](/graph/api/resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions?view=graph-rest-beta)<br/>[win32LobAppDetectionOperator](/graph/api/resources/intune-apps-win32lobappdetectionoperator?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/>[win32LobAppMsiPackageType](/graph/api/resources/intune-apps-win32lobappmsipackagetype?view=graph-rest-beta)<br/>[win32LobAppRegistryDetectionType](/graph/api/resources/intune-apps-win32lobappregistrydetectiontype?view=graph-rest-beta)<br/>[win32LobAppReturnCodeType](/graph/api/resources/intune-apps-win32lobappreturncodetype?view=graph-rest-beta)<br/>[windows10AppsUpdateRecurrence](/graph/api/resources/intune-deviceconfig-windows10appsupdaterecurrence?view=graph-rest-beta)<br/>[windowsAppStartLayoutTileSize](/graph/api/resources/intune-deviceconfig-windowsappstartlayouttilesize?view=graph-rest-beta)<br/>[windowsAutopilotProfileAssignmentDetailedStatus](/graph/api/resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus?view=graph-rest-beta)<br/>|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に **overrideComplianceState** アクションを追加しました |
|追加|ベータ版|[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) コレクションに **getTargetedUsersAndDevices** アクションを追加しました |
|追加|ベータ版|[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) に [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティに **restrictedApps** プロパティを追加しました|
|追加|ベータ版|[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) エンティティに **tokenCreationDateTime** プロパティを追加しました|
|削除|ベータ版|[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) エンティティから **restrictedApps** プロパティを削除しました|
|削除|ベータ版|[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) エンティティから **restrictedApps** プロパティを削除しました|
|変更|ベータ版|[appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) エンティティで次のプロパティを変更しました。<br/>**enablePerApp** を必須から省略可能に変更しました<br/>|
|追加|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに、**disableProtectionOfManagedOutboundOpenInData** および **protectInboundDataFromUnknownSources** プロパティを追加しました|
|追加|ベータ版|[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-beta) エンティティに **microsoftStoreForBusinessPortalSelection** プロパティを追加しました|
|追加|ベータ版|[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) エンティティに **passcodeMinutesOfInactivityBeforeScreenTimeout** プロパティを追加しました|
|追加|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティに **useOAuth** プロパティを追加しました|
|追加|ベータ版|[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**kioskModeBlockVolumeButtons**、**classroomForceRequestPermissionToLeaveClasses**、**keychainBlockCloudSync**、**pkiBlockOTAUpdates**、**privacyForceLimitAdTracking**、**enterpriseBookBlockBackup**、**enterpriseBookBlockMetadataSync**、**airPrintBlocked**、**airPrintBlockCredentialsStorage**、**airPrintForceTrustedTLS**、**airPrintBlockiBeaconDiscovery**、**blockSystemAppRemoval**、および **vpnBlockCreation** プロパティを追加しました|
|追加|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに、**disableProtectionOfManagedOutboundOpenInData** および **protectInboundDataFromUnknownSources** プロパティを追加しました|
|追加|ベータ版|[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) エンティティに **gatekeeperAllowedAppSource** プロパティを追加しました|
|追加|ベータ版|[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**keychainBlockCloudSync**、**airPrintBlocked**、**airPrintForceTrustedTLS**、および **airPrintBlockiBeaconDiscovery** プロパティを追加しました|
|追加|ベータ版|[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) エンティティに、**deviceModel** および **deviceManufacturer** プロパティを追加しました|
|追加|ベータ版|[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) エンティティに **enabledForScopeValidation** プロパティを追加しました|
|追加|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) エンティティに **claimTokenManagementFromExternalMdm** プロパティを追加しました|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **windows10AppsForceUpdateSchedule** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) エンティティに **deploymentProfileAssignmentDetailedStatus** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、**deviceConfigurationConflictSummary** および **importedWindowsAutopilotDeviceIdentityUploads** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) エンティティに **intendedDeploymentProfile** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta) 複合型に **startLayoutTileSize** および **name** プロパティを追加しました|
|追加|ベータ版|[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta) 複合型に **desktopApplicationId** および **desktopApplicationLinkPath** プロパティを追加しました|
|削除|ベータ版|[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta) 複合型から **name** プロパティを削除しました|
|追加|ベータ版|[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) 複合型に **disallowDesktopApps** プロパティを追加しました|
|変更|ベータ版|[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta) 複合型で次のプロパティを変更しました。<br/>**startMenuLayoutXml** を必須から省略可能に変更しました<br/>|
|追加|ベータ版|[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta) 複合型に、**v10_1607**、**v10_1703**、**v10_1709**、および **v10_1803** プロパティを追加しました|
|追加|ベータ版|[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-beta) 列挙型に **remoteLock** メンバーを追加しました|


### <a name="microsoft-teams-apis"></a>Microsoft Teams API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加|ベータ版|[タブ](/graph/api/resources/teamstab?view=graph-rest-beta)の API を追加しました。|
|追加|ベータ版|[組織のアプリを発行する](/graph/api/resources/teamsapp?view=graph-rest-beta)ための API を追加しました。|
|追加|ベータ版|[GET /teams/{id}](/graph/api/team-get?view=graph-rest-beta) にアプリケーション アクセス許可のサポートを追加しました。 |
|追加|ベータ版|[GET /teams/{id}/channels](/graph/api/group-list-channels?view=graph-rest-beta) にアプリケーション アクセス許可のサポートを追加しました。 |
|追加|ベータ版|[GET /teams/{id}/channels/{id}](/graph/api/channel-get?view=graph-rest-beta) にアプリケーション アクセス許可のサポートを追加しました。 |
|追加|ベータ版|[PUT /groups/{id}/team](/graph/api/team-put-teams?view=graph-rest-beta) にアプリケーション アクセス許可のサポートを追加しました。 |
|追加|ベータ版|[PATCH /teams/{id}](/graph/api/team-update?view=graph-rest-beta) にアプリケーション アクセス許可のサポートを追加しました。 |
|追加|ベータ版|[チャネルの作成](/graph/api/channel-post?view=graph-rest-beta)、[チャネルの更新](/graph/api/channel-patch?view=graph-rest-beta)、および[チャネルの削除](/graph/api/channel-delete?view=graph-rest-beta)にアプリケーション アクセス許可のサポートを追加しました。 |
|削除|ベータ版| [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) から isBlocks および installedState プロパティを削除しました。|
|変更| ベータ版 | [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) のコンテキスト プロパティの名前が distributionMethod に変更されました。|

### <a name="onedrive-and-sharepoint-apis"></a>OneDrive と SharePoint の API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) に [createUploadSession](/graph/api/driveitem-createuploadsession?view=graph-rest-beta) アクションに対する **deferCommit** 引数を追加しました|
| 追加        | ベータ版        | [storagePlanInformation](/graph/api/resources/storageplaninformation?view=graph-rest-beta) 複合型を追加しました |
| 追加        | ベータ版        | [quota](/graph/api/resources/quota?view=graph-rest-beta) 複合型に **storagePlanInformation** プロパティを追加しました |
| 追加        | ベータ版        | [drive](/graph/api/resources/drive?view=graph-rest-beta) エンティティに **following** ナビゲーション プロパティを追加しました |
| 追加        | ベータ版        | [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) に [follow](/graph/api/driveitem-follow?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-beta) API を追加しました |
| 追加        | ベータ版        | [permission](/graph/api/resources/permission?view=graph-rest-beta) エンティティに **hasPassword** プロパティを追加しました |
| 追加        | ベータ版        | [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta) 複合型に **preventsDownload** プロパティを追加しました |
| 追加        | ベータ版        | [sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-beta) エンティティに **permission** ナビゲーション プロパティを追加しました |
| 追加        | ベータ版        | [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta) エンティティに **geolocation** プロパティを追加しました |
| 追加        | ベータ版        | [geolocationColumn](/graph/api/resources/geolocationcolumn?view=graph-rest-beta) 複合型を追加しました |
| 追加        | ベータ版        | [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) エンティティに **analytics** プロパティを追加しました |
| 追加        | ベータ版        | [site](/graph/api/resources/site?view=graph-rest-beta) エンティティに **analytics** プロパティを追加しました |
| 追加        | ベータ版        | [listItem](/graph/api/resources/listitem?view=graph-rest-beta) エンティティに **analytics** プロパティを追加しました |
| 追加        | ベータ版        | [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) エンティティに **getActivitiesByInterval** 関数を追加しました |
| 追加        | ベータ版        | [site](/graph/api/resources/site?view=graph-rest-beta) エンティティに **getActivitiesByInterval** 関数を追加しました |
| 追加        | ベータ版        | [listItem](/graph/api/resources/listitem?view=graph-rest-beta) エンティティに **getActivitiesByInterval** 関数を追加しました |
| 追加        | ベータ版        | [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta) エンティティを追加しました |
| 追加        | ベータ版        | [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta) エンティティを追加しました |
| 追加        | ベータ版        | [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) 複合型を追加しました |
| 追加        | ベータ版        | [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) 複合型を追加しました |
| 追加        | ベータ版        | [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta) 複合型を追加しました |
| 追加        | ベータ版        | [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) 複合型に **access** プロパティを追加しました |
| 追加        | ベータ版        | [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) 複合型に **location** プロパティを追加しました |
| 追加        | v1.0        | [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) エンティティに **preview** アクションを追加しました |
| 追加        | v1.0        | [itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-1.0) 複合型を追加しました |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | メッセージの作成時に、[message](/graph/api/resources/message?view=graph-rest-1.0) エンティティの **internetMessageHeaders** プロパティを書き込めるようになりました。 |


### <a name="project-rome-notifications-api"></a>Project Rome 通知 API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加          | ベータ版        | [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta) というリソースの種類を追加しました。 |
| 追加          | ベータ版        | [通知の作成と発行] (/graph/api/projectrome_notification_post?view=graph-rest-beta) API を追加しました。|

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | セキュア スコア API を [セキュリティ API](/graph/api/resources/securescore-api-overview?view=graph-rest-beta) に追加しました。これには次のリソースと操作が含まれています。<br/>[secureScores](/graph/api/resources/securescores?view=graph-rest-beta) (および関連するエンティティ)<br/>[secureScores のリスト](/graph/api/securescores-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta)<br/>[secureScoreControlProfiles のリスト](/graph/api/securescorecontrolprofiles-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles の更新](/graph/api/securescorecontrolprofiles-update?view=graph-rest-beta) |
| 追加        | ベータ版        | [secureScoreControlStateUpdate](/graph/api/resources/securescorecontrolstateupdate?view=graph-rest-beta) という新しい複合型を導入しました |


## <a name="august-2018"></a>2018 年 8 月

### <a name="delta-query"></a>デルタ クエリ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Azure AD の次のエンティティに、[デルタ クエリ](delta-query-overview.md)機能を追加しました。<br/>[application](/graph/api/application-delta?view=graph-rest-beta)<br/>[directoryRole](/graph/api/directoryrole-delta?view=graph-rest-beta)<br/>[servicePrincipal](/graph/api/serviceprincipal-delta?view=graph-rest-beta) |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | v1.0 | テナントで複数地域機能が有効かどうかをアプリで検証できるようにする、isMultipleDataLocationsForServicesEnabled プロパティが [Organization](/graph/api/resources/organization?view=graph-rest-beta) リソースに追加されました。 ユーザーとグループのために優先されるデータの場所を設定できるようにする、preferredDataLocation プロパティが [user](/graph/api/resources/user?view=graph-rest-beta) および [group](/graph/api/resources/group?view=graph-rest-beta) リソースに追加されました。|
| 追加 | v1.0 | Microsoft 同期製品 (Azure AD Connect、DirSync、および MIM + Connector を含む) を使用して Azure Active Directory にオンプレミス ディレクトリを同期するときのディレクトリ同期エラーを表す、[onPremisesProvisioningErrors](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-1.0) プロパティを [User](/graph/api/resources/user?view=graph-rest-1.0) および [Group](/graph/api/resources/group?view=graph-rest-1.0) エンティティに追加しました。|
| 追加 | v1.0 | 15 個のカスタム拡張属性プロパティを含む、[onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-1.0) プロパティを [User](/graph/api/resources/user?view=graph-rest-1.0) エンティティに追加しました。 onPremisesSyncEnabled ユーザーの場合、このプロパティ セットはオンプレミスの Active Directory でマスター管理され、Azure AD に同期され、読み取り専用となります。 クラウド専用ユーザー (onPremisesSyncEnabled が false) の場合、これらのプロパティは作成時または更新時に設定される可能性があります。|
|追加|v1.0|[User](/graph/api/resources/user?view=graph-rest-1.0) エンティティに、**onPremisesDomainName**、**onPremisesSamAccountName**、および **onPremisesUserPrincipalName** プロパティを追加しました|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-1.0)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-1.0)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-1.0)<br/>|
|追加|v1.0|新しい列挙型を追加しました。<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-1.0)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-1.0)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-1.0)<br/>|
|追加|v1.0|[reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) に [managedDeviceEnrollmentFailureDetails](/graph/api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) に [managedDeviceEnrollmentTopFailures](/graph/api/intune-shared-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0) エンティティに **kioskModeBuiltInAppId** プロパティを追加しました|
|追加|v1.0|[complianceStatus](/graph/api/resources/intune-shared-compliancestatus?view=graph-rest-1.0) 列挙型に **notAssigned** メンバーを追加しました|
|追加|v1.0|[deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-1.0) 列挙型に **pushNotification** メンバーを追加しました|
|追加|v1.0|[deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-1.0) 列挙型に **userAbandonment** メンバーを追加しました|
|追加|v1.0|[managedDevicePartnerReportedHealthState](/graph/api/resources/intune-devices-manageddevicepartnerreportedhealthstate?view=graph-rest-1.0) 列挙型に、**compromised** および **misconfigured** メンバーを追加しました|
|追加|v1.0|[vppTokenState](/graph/api/resources/intune-onboarding-vpptokenstate?view=graph-rest-1.0) 列挙型に **assignedToExternalMDM** メンバーを追加しました|
||
|追加|ベータ版|以下の新しいエンティティを追加しました。<br/>[advancedThreatProtectionOnboardingDeviceSettingState](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate?view=graph-rest-beta)<br/>[advancedThreatProtectionOnboardingStateSummary](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary?view=graph-rest-beta)<br/>[depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)<br/>[depEnrollmentProfile](/graph/api/resources/intune-enrollment-depenrollmentprofile?view=graph-rest-beta)<br/>[depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile?view=graph-rest-beta)<br/>[depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)<br/>[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta)<br/>[importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta)<br/>[importedAppleDeviceIdentityResult](/graph/api/resources/intune-enrollment-importedappledeviceidentityresult?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)<br/>[windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)<br/>|
|追加|ベータ版|以下の新しい複合型を追加しました。<br/>[configurationManagerClientHealthState](/graph/api/resources/intune-devices-configurationmanagerclienthealthstate?view=graph-rest-beta)<br/>[customSubjectAlternativeName](/graph/api/resources/intune-deviceconfig-customsubjectalternativename?view=graph-rest-beta)<br/>[deviceManagementUserRightsLocalUserOrGroup](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup?view=graph-rest-beta)<br/>[deviceManagementUserRightsSetting](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightssetting?view=graph-rest-beta)<br/>[managementCertificateWithThumbprint](/graph/api/resources/intune-enrollment-managementcertificatewiththumbprint?view=graph-rest-beta)<br/>[mobileAppSupportedDeviceType](/graph/api/resources/intune-troubleshooting-mobileappsupporteddevicetype?view=graph-rest-beta)<br/>[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)<br/>[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)<br/>[windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)<br/>[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta)<br/>[windowsMalwareOverview](/graph/api/resources/intune-devices-windowsmalwareoverview?view=graph-rest-beta)<br/>[windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[configurationManagerClientState](/graph/api/resources/intune-devices-configurationmanagerclientstate?view=graph-rest-beta)<br/>[depTokenType](/graph/api/resources/intune-enrollment-deptokentype?view=graph-rest-beta)<br/>[discoverySource](/graph/api/resources/intune-enrollment-discoverysource?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[iTunesPairingMode](/graph/api/resources/intune-enrollment-itunespairingmode?view=graph-rest-beta)<br/>[lanManagerAuthenticationLevel](/graph/api/resources/intune-deviceconfig-lanmanagerauthenticationlevel?view=graph-rest-beta)<br/>[localSecurityOptionsMinimumSessionSecurity](/graph/api/resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity?view=graph-rest-beta)<br/>[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/>[vpnProviderType](/graph/api/resources/intune-deviceconfig-vpnprovidertype?view=graph-rest-beta)<br/>[windowsMalwareThreatState](/graph/api/resources/intune-devices-windowsmalwarethreatstate?view=graph-rest-beta)<br/>|
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) に [uploadDepToken](/graph/api/intune-enrollment-deponboardingsetting-uploaddeptoken?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) に [syncWithAppleDeviceEnrollmentProgram](/graph/api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) に [setDefaultProfile](/graph/api/intune-enrollment-enrollmentprofile-setdefaultprofile?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) コレクションに **importAppleDeviceIdentityList** アクションを追加しました |
|追加|ベータ版|[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) に [updateDeviceProfileAssignment](/graph/api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) アクションを追加しました。 |
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) に [shareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) に [unshareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice?view=graph-rest-beta) アクションを追加しました。 |
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) に [assignUserToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) に [getRoleScopeTagsByResource](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyresource?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) に [getRoleScopeTagsByIds](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyids?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) に [getEncryptionPublicKey](/graph/api/intune-enrollment-deponboardingsetting-getencryptionpublickey?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) に [exportMobileConfig](/graph/api/intune-enrollment-enrollmentprofile-exportmobileconfig?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) に [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) 関数を追加しました |
|削除|ベータ版|**uploadDepToken** コレクションを削除しました |
|削除|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) コレクションの **syncWithAppleDeviceEnrollmentProgram** アクションを削除しました |
|削除|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) コレクションの **getEncryptionPublicKey** 関数を削除しました |
|追加|ベータ版|[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) エンティティに **restrictedApps** プロパティを追加しました|
|追加|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **vpnAlwaysOnPackageIdentifier** および **vpnEnableAlwaysOnLockdownMode** プロパティを追加しました|
|削除|ベータ版|[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta) エンティティから **packageName** プロパティを削除しました|
|追加|ベータ版|[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta) エンティティに **restrictedApps** プロパティを追加しました|
|追加|ベータ版|[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **vpnAlwaysOnPackageIdentifier** および **vpnEnableAlwaysOnLockdownMode** プロパティを追加しました|
|追加|ベータ版|[appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) エンティティに **optInToDeviceIdSharing** プロパティを追加しました|
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) エンティティに、**tokenType**、**tokenName**、**syncedDeviceCount**、**defaultProfileDisplayName**、および **dataSharingConsentGranted** を追加しました|
|追加|ベータ版|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティに **roleScopeTagIds** プロパティを追加しました|
|追加|ベータ版|[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティに **roleScopeTagIds** および **supportsScopeTags** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **windowsMalwareOverview** プロパティを追加しました|
|変更|ベータ版|[iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) エンティティで次のプロパティを変更しました。<br/>**subjectAlternativeNameType** を必須から省略可能に変更しました<br/>|
|追加|ベータ版|[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) エンティティに **restrictedApps** プロパティを追加しました|
|追加|ベータ版|[iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) エンティティに、**certificateStore** および **customSubjectAlternativeNames** プロパティを追加しました|
|追加|ベータ版|[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) エンティティに **enforcedSoftwareUpdateDelayInDays** プロパティを追加しました|
|追加|ベータ版|[iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta) エンティティに、**providerType****userDomain**、**strictEnforcement**、**cloudName**、および **excludeList** プロパティを追加しました|
|追加|ベータ版|[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**safariBlockAutofill**、**cameraBlocked**、**iTunesBlockMusicService**、**spotlightBlockInternetResults**、**keyboardBlockDictation**、**definitionLookupBlocked**、**appleWatchBlockAutoUnlock**、**iTunesBlockFileSharing**、**iCloudBlockDocumentSync**、**iCloudBlockMail**、**iCloudBlockAddressBook**、**iCloudBlockCalendar**、**iCloudBlockReminders**、**iCloudBlockBookmarks**、**iCloudBlockNotes**、**airDropBlocked**、**passwordBlockModification**、および **passwordBlockFingerprintUnlock** プロパティを追加しました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、**roleScopeTagIds**、**windowsActiveMalwareCount**、**windowsRemediatedMalwareCount**、**notes**、および **configurationManagerClientHealthState** プロパティを追加しました|
|追加|ベータ版|[mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティに **installStateDetail** プロパティを追加しました|
|追加|ベータ版|[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) エンティティに **roleScopeTagIds** プロパティを追加しました|
|追加|ベータ版|[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティに **targetVersion** および **updateVersion** プロパティを追加しました|
|追加|ベータ版|[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) エンティティに **resource** プロパティを追加しました|
|追加|ベータ版|[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) エンティティに、**localStorage**、**setPowerPolicies**、および **signInOnResume** プロパティを追加しました|
|追加|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティに **configurationManagerComplianceRequired** プロパティを追加しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに、**userRightsAccessCredentialManagerAsTrustedCaller**、**userRightsAllowAccessFromNetwork**、**userRightsBlockAccessFromNetwork**、**userRightsActAsPartOfTheOperatingSystem**、**userRightsLocalLogOn**、**userRightsBackupData**、**userRightsChangeSystemTime**、**userRightsCreateGlobalObjects**、**userRightsCreatePageFile**、**userRightsCreatePermanentSharedObjects**、**userRightsCreateSymbolicLinks**、**userRightsCreateToken**、**userRightsDebugPrograms**、**userRightsRemoteDesktopServicesLogOn**、**userRightsDelegation**、**userRightsGenerateSecurityAudits**、**userRightsImpersonateClient**、**userRightsIncreaseSchedulingPriority**、**userRightsLoadUnloadDrivers**、**userRightsLockMemory**、**userRightsManageAuditingAndSecurityLogs**、**userRightsManageVolumes**、**userRightsModifyFirmwareEnvironment**、**userRightsModifyObjectLabels**、**userRightsProfileSingleProcess**、**userRightsRemoteShutdown**、**userRightsRestoreData**、**userRightsTakeOwnership**、**userRightsRegisterProcessAsService**、**localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients**、**localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers**、**lanManagerAuthenticationLevel**、および **lanManagerWorkstationEnableInsecureGuestLogons** プロパティを追加しました|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、**passwordMinimumAgeInDays**、**tenantLockdownRequireNetworkDuringOutOfBoxExperience**、および **dataProtectionBlockDirectMemoryAccess** プロパティを追加しました|
|追加|ベータ版|[windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) エンティティに **extendedKeyUsages** プロパティを追加しました|
|追加|ベータ版|[windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) エンティティに **enableDnsRegistration** および **dnsSuffixes** プロパティを追加しました|
|追加|ベータ版|[windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta) エンティティに **customSubjectAlternativeNames** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **extractHardwareHash** および **deviceNameTemplate** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) エンティティに **addressableUserName** および **userPrincipalName** エンティティを追加しました|
|追加|ベータ版|[windowsDeviceMalwareState](/graph/api/resources/intune-devices-windowsdevicemalwarestate?view=graph-rest-beta) エンティティに **threatState** プロパティを追加しました|
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティに、**qualityUpdatesPauseStartDateTime**、**featureUpdatesPauseStartDateTime**、**featureUpdatesRollbackWindowInDays**、**qualityUpdatesWillBeRolledBack**、**featureUpdatesWillBeRolledBack****qualityUpdatesRollbackStartDateTime**、および **featureUpdatesRollbackStartDateTime** プロパティを追加しました|
|追加|ベータ版|[windowsWifiEnterpriseEAPConfiguration](/graph/api/resources/intune-deviceconfig-windowswifienterpriseeapconfiguration?view=graph-rest-beta) エンティティに **trustedServerCertificateNames** プロパティを追加しました|
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) エンティティに、**defaultIosEnrollmentProfile**、**defaultMacOsEnrollmentProfile**、**enrollmentProfiles**、および **importedAppleDeviceIdentities** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) エンティティに **roleScopeTags** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに、**advancedThreatProtectionOnboardingStateSummary**、**roleScopeTags**、および **importedWindowsAutopilotDeviceIdentityUploads** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta) 複合型に **supportedDeviceTypes** プロパティを追加しました|
|追加|ベータ版|[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 複合型に **hideEscapeLink** プロパティを追加しました|
|追加|ベータ版|[appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) 列挙型に、**zscalerPrivateAccess**、**f5Access2018**、**citrixSso**、および **paloAltoGlobalProtectV2** メンバーを追加しました|
|追加|ベータ版|[deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-beta) 列挙型に **userAbandonment** メンバーを追加しました|
|追加|ベータ版|[enrollmentState](/graph/api/resources/intune-enrollment-enrollmentstate?view=graph-rest-beta) 列挙型に **blocked** メンバーを追加しました|
|追加|ベータ版|[managementAgentType](/graph/api/resources/intune-devices-managementagenttype?view=graph-rest-beta) 列挙型に **microsoft365ManagedMdm** メンバーを追加しました|
|追加|ベータ版|[subjectAlternativeNameType](/graph/api/resources/intune-deviceconfig-subjectalternativenametype?view=graph-rest-beta) 列挙型に **domainNameService** メンバーを追加しました|
|追加|ベータ版|[wiFiSecurityType](/graph/api/resources/intune-deviceconfig-wifisecuritytype?view=graph-rest-beta) 列挙型に **wpa2Personal** および **wpa2Enterprise** メンバーを追加しました|
|追加|ベータ版|[windowsMalwareCategory](/graph/api/resources/intune-devices-windowsmalwarecategory?view=graph-rest-beta) 列挙型に **enterpriseUnwantedSoftware**、**ransom**、および **hipsRule** メンバーを追加しました|

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) アクション、および [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-beta)、[scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-beta)、[scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-beta) 複合型が追加され、[ユーザーの空き時間情報、配布リスト、および一定期間のリソースの取得](outlook-get-free-busy-schedule.md)がサポートされるようになりました。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0        | [getMailTips](/graph/api/user-getmailtips?view=graph-rest-1.0) アクションのサポートが追加され、特定の受信者のすべてのメール ヒントを取得できるようになりました。 次のリソースが追加されました: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-1.0)、[mailTips](/graph/api/resources/mailtips?view=graph-rest-1.0)、[mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-1.0)。 |

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | v1.0    | [getoffice365activationsuserdetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0) に **Activated On Shared Computer** プロパティを追加しました。 |
| 追加    | v1.0    | [getoffice365activationsusercounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0) に **Shared Computer Activation** プロパティを追加しました。 |

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | [alert](/graph/api/resources/alert?view=graph-rest-beta ) に、**activityGroupName**、**cloudAppStates**、**confidence**、および **registryKeyStates** プロパティを追加しました。 |
|削除|ベータ版| [alert](/graph/api/resources/alert?view=graph-rest-beta ) から、**activityGroupStates**、**applicationStates**、**malwareWasRunning**、**riskScore**、および **type** プロパティを削除しました。 |
|変更|ベータ版| [alert](/graph/api/resources/alert?view=graph-rest-beta)で、**comments** 型を `String` から `String collection` に、**severity** 型を `String` から [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) 列挙型に変更しました。 |
| 追加        | ベータ版       | 次のリソースの種類を追加しました。 <br/> [cloudAppSecurityState](/graph/api/resources/cloudappsecuritystate?view=graph-rest-beta) <br/> [fileHash](/graph/api/resources/filehash?view=graph-rest-beta) <br/> [registryKeyState](/graph/api/resources/registrykeystate?view=graph-rest-beta) |
|削除|ベータ版| 次のリソースの種類を削除しました。 <br/> **activityGroupState**  <br/> **applicationSecurityState** |
| 追加        | ベータ版       | 次の列挙型を追加しました。 <br/> [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) <br/> [connectionDirection](/graph/api/resources/connectiondirectionenumtype?view=graph-rest-beta) <br/> [connectionStatus](/graph/api/resources/connectionstatusenumtype?view=graph-rest-beta) <br/> [emailRole](/graph/api/resources/emailroleenumtype?view=graph-rest-beta) <br/> [fileHashType](/graph/api/resources/filehashtypeenumtype?view=graph-rest-beta) <br/> [registryHive](/graph/api/resources/registryhiveenumtype?view=graph-rest-beta)  <br/> [registryOperation](/graph/api/resources/registryoperationenumtype?view=graph-rest-beta) <br/> [registryValueType](/graph/api/resources/registryvaluetypeenumtype?view=graph-rest-beta)|
|削除|ベータ版| 次の列挙型を削除しました。 <br/> **alertType** <br/> **applicationPermissionsRequired** |
| 追加        | ベータ版       | [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta ) に **fileHash** プロパティを追加しました。|
|削除|ベータ版| [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta) から **authenticodeHash256** および **sha256** プロパティを削除しました。 |
| 追加 | ベータ版 | [hostSecurityState](/graph/api/resources/hostsecuritystate?view=graph-rest-beta) に **os** プロパティを追加しました。|
| 追加 | ベータ版 | [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) に、**category**、**family**、および **wasRunning** プロパティを追加しました。|
|削除|ベータ版| [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) から **aliases** プロパティを削除しました。 |
|変更|ベータ版| **malwareWasRunning** プロパティを [alert](/graph/api/resources/alert?view=graph-rest-beta ) から [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) に移動し、名前を **wasRunning** に変更しました。 |
| 追加        | ベータ版       | [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ) に、**applicationName**、**destinationDomain**、**direction**、**domainRegisteredDateTime**、**localDnsName**、**natDestinationAddress**、**natDestinationPort**、**natSourceAddress**、**natSourcePort**、**riskScore**、**status**、および **urlParameters** プロパティを追加しました。|
|変更|ベータ版| [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ) で、**uri** プロパティを **destinationUrl** に変更しました。 |
| 追加        | ベータ版       | [process](/graph/api/resources/process?view=graph-rest-beta ) に **fileHash** プロパティを追加しました。|
|削除|ベータ版| [process](/graph/api/resources/process?view=graph-rest-beta ) から **authenticodeHash256** および **sha256** プロパティを削除しました。 |
| 追加        | ベータ版       | [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta) に、**aadUserId**、**emailRole**、**isVpn**、および **logonIp** プロパティを追加しました。|
|変更|ベータ版| [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta) で、**logonIpAddress** プロパティを **logonIp** に変更しました。 |
| 追加        | ベータ版       | [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta) に **wasRunning** プロパティを追加しました。|
|削除|ベータ版| [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta) から **name** プロパティを削除しました。 |

## <a name="july-2018"></a>2018 年 7 月

### <a name="application-and-serviceprincipal-api-changes"></a>application API と servicePrincipal API の変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [application](/graph/api/resources/application?view=graph-rest-beta) API と [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) API は、プレビュー (ベータ版) で更新されます。 最初の一連の変更は、2018 年 7 月 16 日に適用されます。 変更には、プロパティの名前変更と再構築が含まれます。 既存のプロパティのほとんどは、変更が完了するまで使用可能になりません。 新しいプロパティがいくつか追加される予定です。 変更は、v1.0 へのリリース前にプレビュー (ベータ版) でリリースされます。 |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|変更|ベータ版|[chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta) リソースを更新しました|
|追加|ベータ版|[Chat attachment](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) というリソースの種類が追加されました|
|追加|ベータ版|[Chat mention](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) というリソースの種類が追加されました|
|追加|ベータ版|[Chat reaction](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) というリソースの種類が追加されました|
|追加|ベータ版|[全チャネル メッセージ取得 API](/graph/api/channel-list-messages?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[チャネル メッセージ取得 API](/graph/api/channel-get-message?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[全メッセージ返信取得 API](/graph/api/channel-list-messagereplies?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[メッセージへの返信取得 API](/graph/api/channel-get-messagereply?view=graph-rest-beta) が追加されました |

### <a name="microsoft-teams-apis"></a>Microsoft Teams API
| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加|ベータ版|[/users/{id}/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta) にアプリケーション アクセス許可のサポートが追加されました |
|追加|ベータ版|[全チャネル メッセージ取得 API](/graph/api/channel-list-messages?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[チャネル メッセージ取得 API](/graph/api/channel-get-message?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[全メッセージ返信取得 API](/graph/api/channel-list-messagereplies?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[メッセージへの返信取得 API](/graph/api/channel-get-messagereply?view=graph-rest-beta) が追加されました |
|追加|ベータ版|[Chat attachment](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) というリソースの種類が追加されました|
|追加|ベータ版|[Chat mention](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) というリソースの種類が追加されました|
|追加|ベータ版|[Chat reaction](/graph/api/resources/chatmessageattachment?view=graph-rest-beta) というリソースの種類が追加されました|
|変更|ベータ版|[chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta)) リソースが更新されました|
|削除|ベータ版|DELETE /groups/{id}/team/channels/{id} は削除されました。代わりに DELETE /teams/{id}/channels/{id} を使用してください。 |
|削除|ベータ版|GET /groups/{id}/team/channels/{id} は削除されました。代わりに　GET /teams/{id}/channels/{id} を使用してください。 |
|削除|ベータ版|PATCH /groups/{id}/team/channels/{id} は削除されました。代わりに PATCH /teams/{id}/channels/{id} を使用してください。 |
|削除|ベータ版|POST /groups/{id}/team/channels/{id}/chatthreads は削除されました。代わりに POST /teams/{id}/channels/{id}/chatthreads を使用してください。 |
|削除|ベータ版|GET /groups/{id}/team/channels は削除されました。代わりに GET /teams/{id}/channels を使用してください。 |
|削除|ベータ版|DELETE /groups/{id}/channels/{id} は削除されました。代わりに DELETE /teams/{id}/channels/{id} を使用してください。 |
|削除|ベータ版|GET /groups/{id}/channels/{id} は削除されました。代わりに GET /teams/{id}/channels/{id} を使用してください。 |
|削除|ベータ版|PATCH /groups/{id}/channels/{id} は削除されました。代わりに PATCH /teams/{id}/channels/{id} を使用してください。 |
|削除|ベータ版|POST /groups/{id}/channels/{id}/chatthreads は削除されました。代わりに POST /teams/{id}/channels/{id}/chatthreads を使用してください。 |
|削除|ベータ版|GET /groups/{id}/channels は削除されました。代わりに GET /teams/{id}/channels を使用してください。 |
|削除|ベータ版|POST /groups/{id}/team/channels は削除されました。代わりに POST /teams/{id}/channels を使用してください。 |
|削除|ベータ版|GET /groups/{id}/team は削除されました。代わりに GET /teams/{id} を使用してください。 |
|削除|ベータ版|PATCH /groups/{id}/team は削除されました。代わりに PATCH /teams/{id} を使用してください。 |
|追加|ベータ版|[組織内のすべてのチームをリスト](teams-list-all-teams.md)する API が追加されました。 |

### <a name="outlook-contacts"></a>Outlook の連絡先
| **変更の種類** | **バージョン**   | **説明**                          |
|:--------------- |:------------- |:---------------------------------------- |
|追加 |ベータ版 | 複合型 [typedEmailAddress](/graph/api/resources/typedemailaddress?view=graph-rest-beta) が追加されました。 |
|変更 | ベータ版 | [contact](/graph/api/resources/contact?view=graph-rest-beta) の **emailAddresses** プロパティの型を **typedEmailAddress** インスタンスのコレクションに変更しました。|

### <a name="synchronization-apis"></a>同期 API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [sychronizationStatus](/graph/api/resources/synchronization-synchronizationstatus?view=graph-rest-beta) に **progress** プロパティが追加され、クライアントでの同期ジョブの進行状況の監視が許可されるようになりました。|

### <a name="webhooks"></a>Webhook
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 重大な変更 | ベータ版および v1.0 | ドライブ ルート項目の [webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) [サブスクリプション有効期限の最大長](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) を 3 日に短縮。 |


## <a name="june-2018"></a>2018 年 6 月

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | すべて | クライアント アプリによるアプリケーションおよびサービス プリンシパルの作成、読み取り、更新、削除を許可する新しいアプリケーション アクセス許可 _Application.ReadWrite.All_ および _Application.ReadWrite.OwnedBy_ ([アクセス許可のトピック](permissions-reference.md#application-resource-permissions)を参照)。 |
| 追加 | v1.0 | [user](/graph/api/resources/user?view=graph-rest-1.0) リソースに、**ageGroup**、**legalAgeGroupClassification**、および **ConsentRequiredForMinor** プロパティが追加されました

### <a name="identity-and-access-apis"></a>ID およびアクセス API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-beta) に[アクセスの確認](/graph/api/resources/accessreviews-root?view=graph-rest-beta)機能が追加されました。 |

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) エンティティに **connectorServerName** プロパティが追加されました|
|追加|v1.0|[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0) エンティティに **firewallEnabled**、**firewallBlockAllIncoming**、および **firewallEnableStealthMode** のプロパティが追加されました|
|追加|v1.0|[iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-1.0) 列挙型に **unknown** メンバーが追加されました|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidDeviceOwnerWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerwificonfiguration?view=graph-rest-beta)<br/>[iosVppAppAssignedDeviceLicense](/graph/api/resources/intune-apps-iosvppappassigneddevicelicense?view=graph-rest-beta)<br/>[iosVppAppAssignedLicense](/graph/api/resources/intune-apps-iosvppappassignedlicense?view=graph-rest-beta)<br/>[iosVppAppAssignedUserLicense](/graph/api/resources/intune-apps-iosvppappassigneduserlicense?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationstate?view=graph-rest-beta)<br/>[userPFXCertificate](/graph/api/resources/intune-raimportcerts-userpfxcertificate?view=graph-rest-beta)<br/>[vppTokenLicenseSummary](/graph/api/resources/intune-onboarding-vpptokenlicensesummary?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[iosVppAppRevokeLicensesActionResult](/graph/api/resources/intune-apps-iosvppapprevokelicensesactionresult?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[androidDeviceOwnerSystemUpdateInstallType](/graph/api/resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype?view=graph-rest-beta)<br/>[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)<br/>[userPfxIntendedPurpose](/graph/api/resources/intune-raimportcerts-userpfxintendedpurpose?view=graph-rest-beta)<br/>[userPfxPaddingScheme](/graph/api/resources/intune-raimportcerts-userpfxpaddingscheme?view=graph-rest-beta)<br/>|
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) に [createGooglePlayWebToken](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken?view=graph-rest-beta) アクションが追加されました |
|追加|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) に [revokeAllLicenses](/graph/api/intune-apps-iosvppapp-revokealllicenses?view=graph-rest-beta) アクションが追加されました |
|追加|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) に [revokeUserLicense](/graph/api/intune-apps-iosvppapp-revokeuserlicense?view=graph-rest-beta) アクションが追加されました |
|追加|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) に [revokeDeviceLicense](/graph/api/intune-apps-iosvppapp-revokedevicelicense?view=graph-rest-beta) アクションが追加されました |
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) に [sendCustomNotificationToCompanyPortal](/graph/api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal?view=graph-rest-beta) アクションが追加されました |
|追加|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) コレクションに **getLicensesForApp** 関数が追加されました |
|削除|ベータ版|次の列挙型を削除しました。<br/>**windowsUpdateInsiderBuildControl**<br/>|
|追加|ベータ版|[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **systemUpdateWindowStartMinutesAfterMidnight**、**systemUpdateWindowEndMinutesAfterMidnight**、および **systemUpdateInstallType** のプロパティが追加されました|
|変更|ベータ版|[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) エンティティの次のプロパティの型が変更されました:<br/>**passwordMinutesOfInactivityBeforeScreenTimeout** が Int64 から Int32 へ<br/>|
|追加|ベータ版|[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta) エンティティに **customKeyValueData** プロパティが追加されました|
|追加|ベータ版|[androidVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidvpnconfiguration?view=graph-rest-beta) エンティティに **customKeyValueData** プロパティが追加されました|
|追加|ベータ版|[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta) エンティティに **customKeyValueData** プロパティが追加されました|
|追加|ベータ版|[appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) エンティティに **customKeyValueData** プロパティが追加されました|
|追加|ベータ版|[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta) エンティティに **userId** および **userPrincipalName** のプロパティが追加されました|
|追加|ベータ版|[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta) エンティティに **userId** および **userPrincipalName** のプロパティが追加されました|
|追加|ベータ版|[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) エンティティに **connectorServerName** プロパティが追加されました|
|削除|ベータ版|[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) エンティティから **settingXml** プロパティが削除されました|
|追加|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) エンティティに **vppTokenId** および **revokeLicenseActionResults** のプロパティが追加されました|
|追加|ベータ版|[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) エンティティに **firewallEnabled**、**firewallBlockAllIncoming**、および **firewallEnableStealthMode** のプロパティが追加されました|
|削除|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティから **remoteAssistanceSessionErrorString** プロパティが削除されました|
|追加|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティに **antivirusRequired** および **antiSpywareRequired** のプロパティが追加されました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **defenderOfficeAppsOtherProcessInjection**、**defenderOfficeAppsExecutableContentCreationOrLaunch**、**defenderOfficeAppsLaunchChildProcess**、**defenderOfficeMacroCodeAllowWin32Imports**、**defenderScriptObfuscatedMacroCode**、**defenderScriptDownloadedPayloadExecution**、**defenderProcessCreation**、**defenderUntrustedUSBProcess**、**defenderUntrustedExecutable**、および **defenderEmailContentExecution** のプロパティが追加されました|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **searchDisableLocation**、**inkWorkspaceAccessState**、**defenderPotentiallyUnwantedAppActionSetting**、および **defenderCloudExtendedTimeoutInSeconds** のプロパティが追加されました|
|追加|ベータ版|[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-beta) エンティティに **updatesMinimumAutoInstallClassification** プロパティが追加されました|
|削除|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティから **previewBuildSetting** プロパティが削除されました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **userPfxCertificates** ナビゲーション プロパティが追加されました|
|追加|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) エンティティに **assignedLicenses** ナビゲーション プロパティが追加されました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **managedDeviceMobileAppConfigurationStates** ナビゲーション プロパティが追加されました|
|追加|ベータ版|[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta) 複合型に **websiteList** プロパティが追加されました|
|追加|ベータ版|[devicePlatformType](/graph/api/resources/intune-deviceconfig-deviceplatformtype?view=graph-rest-beta) 列挙型に **androidWorkProfile** メンバーが追加されました|
|追加|ベータ版|[editionUpgradeLicenseType](/graph/api/resources/intune-deviceconfig-editionupgradelicensetype?view=graph-rest-beta) 列挙型に **notConfigured** メンバーが追加されました|
|追加|ベータ版|[iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-beta) 列挙型に **unknown** メンバーが追加されました|
|追加|ベータ版|[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta) 列挙型に **userRequestedInstall** メンバーが追加されました|
|追加|ベータ版|[windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta) 列挙型に **notConfigured** メンバーが追加されました

### <a name="microsoft-teams-apis"></a>Microsoft Teams API
| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
|追加         | ベータ版          | チーム [archive](/graph/api/team-archive?view=graph-rest-beta) および [unarchive](/graph/api/team-unarchive?view=graph-rest-beta) API が追加されました。|
|追加         | ベータ版          | チーム [clone](/graph/api/team-clone?view=graph-rest-beta) 操作が追加されました。 |
|追加         | ベータ版          | チームの [apps](/graph/api/resources/teamsapp?view=graph-rest-beta) を追加したり削除したりする API が追加されました。 |
|変更|ベータ版|[team](/graph/api/resources/team?view=graph-rest-beta) エンティティのパスが更新されました。|
|変更|ベータ版|[channel](/graph/api/resources/channel?view=graph-rest-beta) エンティティへのパスを更新しました。|


### <a name="privileged-identity-management-apis"></a>特権 ID 管理 API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加 | ベータ版 | [privilegedAccess](/graph/api/resources/privilegedaccess?view=graph-rest-beta) エンティティが追加されました。|
| 追加 | ベータ版 | [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) エンティティ、および次のメソッドとアクションが追加されました: <br> [List](/graph/api/governanceresource-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceresource-get?view=graph-rest-beta)<br>|
| 追加 | ベータ版 | [governanceSubject](/graph/api/resources/governancesubject?view=graph-rest-beta) エンティティが追加されました。|
| 追加 | ベータ版 | [governanceRoleDefinition](/graph/api/resources/governanceroledefinition?view=graph-rest-beta) エンティティ、および次のメソッドとアクションが追加されました:<br> [List](/graph/api/governanceroledefinition-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroledefinition-get?view=graph-rest-beta) |
| 追加 | ベータ版 | [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) エンティティ、および次のメソッドとアクションが追加されました:<br> [List](/graph/api/governanceroleassignment-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignment-get?view=graph-rest-beta) <br> [Export](/graph/api/governanceroleassignment-export?view=graph-rest-beta) |
| 追加 | ベータ版 | [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) エンティティ、および次のメソッドとアクションが追加されました:<br> [List](/graph/api/governanceroleassignmentrequest-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignmentrequest-get?view=graph-rest-beta) <br> [Create](/graph/api/governanceroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/governanceroleassignmentrequest-cancel?view=graph-rest-beta) <br> [Update](/graph/api/governanceroleassignmentrequest-update?view=graph-rest-beta) |
| 追加 | ベータ版 | [governanceRoleSetting](/graph/api/resources/governancerolesetting?view=graph-rest-beta) エンティティ、および次のメソッドとアクションが追加されました:<br> [List](/graph/api/governancerolesetting-list?view=graph-rest-beta) <br> [Get](/graph/api/governancerolesetting-get?view=graph-rest-beta) <br> [Update](/graph/api/governancerolesetting-update?view=graph-rest-beta) |
| 追加 | ベータ版 | 次の複合型を追加しました。 <br> [governancePermission](/graph/api/resources/governancepermission?view=graph-rest-beta) <br> [governanceRoleAssignmentRequestStatus](/graph/api/resources/governanceroleassignmentrequeststatus?view=graph-rest-beta) <br> [governanceRuleSetting](/graph/api/resources/governancerulesetting?view=graph-rest-beta) <br> [governanceSchedule](/graph/api/resources/governanceschedule?view=graph-rest-beta)|

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版        | 新しい列挙型を追加しました。<br/>[alertFeedback](/graph/api/resources/alertfeedbackenumtype?view=graph-rest-beta)<br/>[alertStatus](/graph/api/resources/alertstatusenumtype?view=graph-rest-beta)<br/>[alertType](/graph/api/resources/alerttypeenumtype?view=graph-rest-beta)<br/>[applicationPermissionsRequired](/graph/api/resources/applicationpermissionsrequiredenumtype?view=graph-rest-beta)<br/>[logonType](/graph/api/resources/logontypeenumtype?view=graph-rest-beta)<br/>[processIntegrityLevel](/graph/api/resources/processintegritylevelenumtype?view=graph-rest-beta)<br/>[securityNetworkProtocol](/graph/api/resources/securitynetworkprotocolenumtype?view=graph-rest-beta)<br/>[userAccountSecurityType](/graph/api/resources/useraccountsecuritytypeenumtype?view=graph-rest-beta)<br/>

## <a name="may-2018"></a>2018 年 5 月

### <a name="azure-ad-apis"></a>Azure AD API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更           | ベータ版          | 意味をより的確に反映するために、[subscription](/graph/api/resources/subscription?view=graph-rest-beta) エンティティの **creatorUserId** プロパティの名前を **creatorId** に変更しました。 |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0        | [ディレクトリ (削除済みアイテム)](/graph/api/resources/directory?view=graph-rest-1.0) リソースに[ユーザーが所有する削除済みアイテムの一覧表示](/graph/api/directory-deleteditems-user-owned?view=graph-rest-1.0)アクションを追加しました |
| 追加 | ベータ版 | 特定のユーザーが所有している削除済みのグループを一覧表示できるように、[getUserOwnedObjects](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) 関数を [directory](/graph/api/resources/directory?view=graph-rest-beta) リソースに追加しました。 |

### <a name="education-api"></a>教育機関 API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | アプリ専用のトークンを使用して [educationClass](/graph/api/resources/educationclass?view=graph-rest-1.0) エンティティで **Members** コレクションを読み込む、または更新するには、スコープ **Members.Read.Hidden** が必要になりました。 |
|変更           |ベータ版           |[educationsubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) の status プロパティの **educationSubmissionStatus** タイプで使用できる値を更新しました。|
|変更           |ベータ版           |[educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta) の assignTo プロパティに **educationAssignmentIndividualRecipient** 複合型を追加しました。|
|変更           |ベータ版           |[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) のプロパティ **unsubmittedBy**、**unsubmittedDate**、**returnedBy**、**returnedDate** を追加しました。|
|追加         |ベータ版           |[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) に [return](/graph/api/educationsubmission-return?view=graph-rest-beta) および [unsubmit](/graph/api/educationsubmission-unsubmit?view=graph-rest-beta) アクションを追加しました。|
|変更           |ベータ版           |[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta) の release および recall アクションを削除しました。|

### <a name="groups"></a>グループ

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | [post](/graph/api/resources/post?view=graph-rest-1.0) エンティティに **importance** プロパティが追加されました。 |

### <a name="insights-api"></a>Insights API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [settings](/graph/api/resources/user-settings?view=graph-rest-beta) エンティティと次の CRUD メソッドを追加しました。 <br> [Get](/graph/api/user-get-settings?view=graph-rest-beta) <br> [Update](/graph/api/user-update-settings?view=graph-rest-beta) |

### <a name="microsoft-bookings-api"></a>Microsoft Bookings API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [bookingBusiness](/graph/api/resources/bookingbusiness?view=graph-rest-beta) エンティティと次の CRUD メソッドおよび操作を追加しました。 <br> [List](/graph/api/bookingbusiness-list?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-bookingbusinesses?view=graph-rest-beta) <br> [Get](/graph/api/bookingbusiness-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingbusiness-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingbusiness-delete?view=graph-rest-beta) <br> [Publish](/graph/api/bookingbusiness-publish?view=graph-rest-beta) <br> [Unpublish](/graph/api/bookingbusiness-unpublish?view=graph-rest-beta) <br> API の統合の詳細については、[Microsoft Bookings API](booking-concept-overview.md) を参照してください。 |
| 追加        | ベータ版          | [bookingAppointment](/graph/api/resources/bookingappointment?view=graph-rest-beta) エンティティと次の CRUD メソッドおよび操作を追加しました。 <br> [List](/graph/api/bookingbusiness-list-appointments?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) <br> [Get](/graph/api/bookingappointment-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingappointment-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingappointment-delete?view=graph-rest-beta) <br> [Cancel](/graph/api/bookingappointment-cancel?view=graph-rest-beta) |
| 追加        | ベータ版          | [bookingCurrency](/graph/api/resources/bookingcurrency?view=graph-rest-beta) エンティティと次のメソッドを追加しました。 <br> [List](/graph/api/bookingcurrency-list?view=graph-rest-beta) <br> [Get](/graph/api/bookingcurrency-get?view=graph-rest-beta) |
| 追加        | ベータ版          | [bookingCustomer](/graph/api/resources/bookingcustomer?view=graph-rest-beta) エンティティと次の CRUD メソッドを追加しました。 <br> [List](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) <br> [Get](/graph/api/bookingcustomer-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingcustomer-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingcustomer-delete?view=graph-rest-beta)|
| 追加        | ベータ版          | [bookingService](/graph/api/resources/bookingservice?view=graph-rest-beta) エンティティと次の CRUD メソッドを追加しました。 <br> [List](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-services?view=graph-rest-beta) <br> [Get](/graph/api/bookingservice-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingservice-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingservice-delete?view=graph-rest-beta)|
| 追加        | ベータ版          | [bookingStaffMember](/graph/api/resources/bookingstaffmember?view=graph-rest-beta) エンティティと次の CRUD メソッドを追加しました。 <br> [List](/graph/api/bookingbusiness-list-staffmembers?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-staffmembers?view=graph-rest-beta) <br> [Get](/graph/api/bookingstaffmember-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingstaffmember-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingstaffmember-delete?view=graph-rest-beta)|
| 追加        | ベータ版          | 次の複合型を追加しました。 <br> [bookingNamedEntity](/graph/api/resources/bookingnamedentity?view=graph-rest-beta) <br> [bookingPerson](/graph/api/resources/bookingperson?view=graph-rest-beta) <br> [bookingReminder](/graph/api/resources/bookingreminder?view=graph-rest-beta) <br> [bookingWorkHours](/graph/api/resources/bookingworkhours?view=graph-rest-beta) <br> [bookingWorkTimeSlot](/graph/api/resources/bookingworktimeslot?view=graph-rest-beta)|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)<br/>[easEmailProfileConfigurationBase](/graph/api/resources/intune-deviceconfig-easemailprofileconfigurationbase?view=graph-rest-beta)<br/>[mobileAppIntentAndState](/graph/api/resources/intune-troubleshooting-mobileappintentandstate?view=graph-rest-beta)<br/>[mobileAppTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingevent?view=graph-rest-beta)<br/>[unsupportedDeviceConfiguration](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfiguration?view=graph-rest-beta)<br/>[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[managedDeviceCleanupSettings](/graph/api/resources/intune-devices-manageddevicecleanupsettings?view=graph-rest-beta)<br/>[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppPolicyCreationHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapppolicycreationhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppStateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappstatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppTargetHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapptargethistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppUpdateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappupdatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingDeviceCheckinHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingdevicecheckinhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem?view=graph-rest-beta)<br/>[unsupportedDeviceConfigurationDetail](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail?view=graph-rest-beta)<br/>**windowsAutoPilotEnrollmentSettings**<br/>[windowsKioskActiveDirectoryGroup](/graph/api/resources/intune-deviceconfig-windowskioskactivedirectorygroup?view=graph-rest-beta)<br/>[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)<br/>[windowsKioskAppConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskappconfiguration?view=graph-rest-beta)<br/>[windowsKioskAutologon](/graph/api/resources/intune-deviceconfig-windowskioskautologon?view=graph-rest-beta)<br/>[windowsKioskAzureADGroup](/graph/api/resources/intune-deviceconfig-windowskioskazureadgroup?view=graph-rest-beta)<br/>[windowsKioskAzureADUser](/graph/api/resources/intune-deviceconfig-windowskioskazureaduser?view=graph-rest-beta)<br/>[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)<br/>[windowsKioskLocalGroup](/graph/api/resources/intune-deviceconfig-windowskiosklocalgroup?view=graph-rest-beta)<br/>[windowsKioskLocalUser](/graph/api/resources/intune-deviceconfig-windowskiosklocaluser?view=graph-rest-beta)<br/>[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)<br/>[windowsKioskProfile](/graph/api/resources/intune-deviceconfig-windowskioskprofile?view=graph-rest-beta)<br/>[windowsKioskSingleUWPApp](/graph/api/resources/intune-deviceconfig-windowskiosksingleuwpapp?view=graph-rest-beta)<br/>[windowsKioskUser](/graph/api/resources/intune-deviceconfig-windowskioskuser?view=graph-rest-beta)<br/>[windowsKioskUWPApp](/graph/api/resources/intune-deviceconfig-windowskioskuwpapp?view=graph-rest-beta)<br/>[windowsKioskVisitor](/graph/api/resources/intune-deviceconfig-windowskioskvisitor?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[defenderScheduleScanDay](/graph/api/resources/intune-deviceconfig-defenderschedulescanday?view=graph-rest-beta)<br/>[defenderSubmitSamplesConsentType](/graph/api/resources/intune-deviceconfig-defendersubmitsamplesconsenttype?view=graph-rest-beta)<br/>[domainNameSource](/graph/api/resources/intune-deviceconfig-domainnamesource?view=graph-rest-beta)<br/>[localSecurityOptionsSmartCardRemovalBehaviorType](/graph/api/resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype?view=graph-rest-beta)<br/>[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta)<br/>[mobileAppIntent](/graph/api/resources/intune-troubleshooting-mobileappintent?view=graph-rest-beta)<br/>[roleAssignmentScopeType](/graph/api/resources/intune-rbac-roleassignmentscopetype?view=graph-rest-beta)<br/>[usernameSource](/graph/api/resources/intune-deviceconfig-usernamesource?view=graph-rest-beta)<br/>[windowsDeviceUsageType](/graph/api/resources/intune-enrollment-windowsdeviceusagetype?view=graph-rest-beta)<br/>|
|追加|ベータ版|[setDeviceName](/graph/api/intune-devices-manageddevice-setdevicename?view=graph-rest-beta)<br/>アクションを [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**depEnrollmentProfile**<br/>**enrollmentProfile**<br/>**importedAppleDeviceIdentity**<br/>**importedAppleDeviceIdentityResult**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**managementCertificateWithThumbprint**<br/>|
|削除|ベータ版|次の列挙型を削除しました。<br/>**depTokenType**<br/>**discoverySource**<br/>**iTunesPairingMode**<br/>|
|削除|ベータ版|[importedAppleDeviceIdentity](/graph/api/resources/intune-corpenrollment-importedappledeviceidentity?view=graph-rest-beta) コレクションから importAppleDeviceIdentityList アクションを削除しました |
|削除|ベータ版|[enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) から [updateDeviceProfileAssignment](/graph/api/intune-corpenrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) アクションを削除しました。 |
|削除|ベータ版|[enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) から setDefaultProfile アクションを削除しました |
|削除|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) から shareForSchoolDataSyncService アクションを削除しました |
|削除|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) から unshareForSchoolDataSyncService アクションを削除しました |
|削除|ベータ版|[enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) の exportMobileConfig](/graph/api/intune_corpenrollment_enrollmentprofile_exportmobileconfig?view=graph-rest-beta) 関数を削除しました |
|追加|ベータ版|[androidEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-androideasemailprofileconfiguration?view=graph-rest-beta) エンティティに **userDomainNameSource** および **customDomainName** プロパティを追加しました|
|追加|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **workProfileBlockCamera** および **workProfileBlockCrossProfileContactsSearch** プロパティを追加しました|
|追加|ベータ版|[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **workProfileBlockCamera** および **workProfileBlockCrossProfileContactsSearch** プロパティを追加しました|
|追加|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **thirdPartyKeyboardsBlocked** および **filterOpenInToOnlyManagedApps** プロパティを追加しました|
|追加|ベータ版|[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) エンティティに **conflictCount** プロパティを追加しました|
|追加|ベータ版|[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) エンティティに **conflictCount** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **managedDeviceCleanupSettings** プロパティを追加しました|
|削除|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティから **usernameSource** プロパティを削除しました|
|追加|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに **thirdPartyKeyboardsBlocked** および **filterOpenInToOnlyManagedApps** プロパティを追加しました|
|追加|ベータ版|[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta) エンティティに **ignoreVersionDetection** プロパティを追加しました|
|追加|ベータ版|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) エンティティに **pinRequiredOnLaunchInsteadOfBiometric** および **pinRequiredInsteadOfBiometricTimeout** プロパティを追加しました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **autopilotEnrolled**、**requireUserEnrollmentApproval**、**iccid**、および **udid** プロパティを追加しました|
|削除|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティから **isAutopilotEnrolled** プロパティを削除しました|
|追加|ベータ版|[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta) エンティティに **notApplicablePlatformCount** および **conflictCount** プロパティを追加しました|
|追加|ベータ版|[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta) エンティティに、**conflictCount** プロパティを追加しました|
|追加|ベータ版|[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) エンティティに **scopeType** プロパティを追加しました|
|削除|ベータ版|[windows10EasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windows10easemailprofileconfiguration?view=graph-rest-beta) エンティティから **usernameSource** プロパティを削除しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees**、**localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers**、**localSecurityOptionsDisableServerDigitallySignCommunicationsAlways**、**localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees**、**localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares**、**localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts**、**localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares**、**localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange**、および **localSecurityOptionsSmartCardRemovalBehavior** プロパティを追加しました|
|追加|ベータ版|[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)エンティティに **showInstallationProgress**、**blockDeviceSetupRetryByUser**、**allowDeviceResetOnInstallFailure**、**allowLogCollectionOnInstallFailure**、**customErrorMessage**、**installProgressTimeoutInMinutes**、および **allowDeviceUseOnInstallFailure** プロパティを追加しました|
|削除|ベータ版|[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) エンティティから **title**、**bodyText**、**moreInfoUrl**、および **moreInfoText** プロパティを削除しました。|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **defenderBlockOnAccessProtection**、**defenderScheduleScanDay**、および **defenderSubmitSamplesConsentType** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **language** および **enrollmentSettings** プロパティを追加しました|
|追加|ベータ版|[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) エンティティに **useDeviceContext** プロパティを追加しました|
|削除|ベータ版|[windowsPhoneEASEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration?view=graph-rest-beta) エンティティから **usernameSource** プロパティを削除しました|
|削除|ベータ版|[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティから **localActions** ナビゲーション プロパティを削除しました|
|削除|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティからナビゲーション プロパティ **enrollmentProfiles** および **importedAppleDeviceIdentities** を削除しました|
|追加|ベータ版|[user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) エンティティに **mobileAppIntentAndStates** および **mobileAppTroubleshootingEvents** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 複合型に **deviceUsageType** および **skipKeyboardSelectionPage** プロパティを追加しました|
|削除|ベータ版|[androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta) 列挙型から **paloAltoGlobalProtect** メンバーを削除しました|
|追加|ベータ版|[androidUsernameSource](/graph/api/resources/intune-deviceconfig-androidusernamesource?view=graph-rest-beta) 列挙型に **samAccountName** および **primarySmtpAddress** メンバーを追加しました|
|削除|ベータ版|[androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta) 列挙型から **paloAltoGlobalProtect** メンバーを削除しました|
|追加|ベータ版|[windows10VpnConnectionType](/graph/api/resources/intune-deviceconfig-windows10vpnconnectiontype?view=graph-rest-beta) 列挙型に **paloAltoGlobalProtect** メンバーが追加されました|

## <a name="april-2018"></a>2018 年 4 月

### <a name="audit-log-api"></a>監査ログ API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい監査ログを API サポートするため、[directoryAudit](/graph/api/resources/directoryaudit?view=graph-rest-beta) および [signIn](/graph/api/resources/signin?view=graph-rest-beta) エンティティを追加しました。 |
|追加|ベータ版|監査ログ API をサポートするため、次のリソースを追加しました。[appIndentity](/graph/api/resources/appidentity?view=graph-rest-beta)、[auditActivityInitiator](/graph/api/resources/auditactivityinitiator?view=graph-rest-beta)、[conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)、[deviceDetail](/graph/api/resources/devicedetail?view=graph-rest-beta)、[mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta)、[modifiedProperty](/graph/api/resources/modifiedproperty?view=graph-rest-beta)、[signinLocation](/graph/api/resources/signinlocation?view=graph-rest-beta)、[signinStatus](/graph/api/resources/signinstatus?view=graph-rest-beta)、[targetResource](/graph/api/resources/targetresource?view=graph-rest-beta)、[targetResourceApp](/graph/api/resources/targetresourceapp?view=graph-rest-beta)、[targetResourceDevice](/graph/api/resources/targetresourcedevice?view=graph-rest-beta)、[targetResourceDirectory](/graph/api/resources/targetresourcedirectory?view=graph-rest-beta)、[targetResourceGroup](/graph/api/resources/targetresourcegroup?view=graph-rest-beta)、[targetResourceOther](/graph/api/resources/targetresourceother?view=graph-rest-beta)、[targetResourcePolicy](/graph/api/resources/targetresourcepolicy?view=graph-rest-beta)、[targetResourceRole](/graph/api/resources/targetresourcerole?view=graph-rest-beta)、[targetResourceServicePrincipal](/graph/api/resources/targetresourceserviceprincipal?view=graph-rest-beta)、[targetResourceUser](/graph/api/resources/targetresourceuser?view=graph-rest-beta)、[userIdentity](/graph/api/resources/useridentity?view=graph-rest-beta) |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [organization](/graph/api/resources/organization?view=graph-rest-1.0) エンティティに **privacyProfile** 複合型を追加しました。 |
| 追加        | v1.0        | [user](/graph/api/resources/user?view=graph-rest-1.0) エンティティに **legalAgeGroup、ageGroup、および consentProvidedForMinor** 複合型を追加しました。 |
| 追加        | v1.0        | [webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) 通知サブスクリプションにユーザーとグループのサポートを追加しました。 |
| 追加        | ベータ版        | [ディレクトリ (削除済みアイテム)](/graph/api/resources/directory?view=graph-rest-beta) リソースに[ユーザーが所有する削除済みアイテムの一覧表示](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta)アクションを追加しました |

### <a name="education-apis"></a>教育機関 API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|変更|ベータ版|[educationsynchronizationerror](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta) に reportableIdentifier プロパティを追加しました。|
|変更|ベータ版|[uploadUrl](/graph/api/educationsynchronizationprofile-uploadurl?view=graph-rest-beta) API の応答オプションを更新しました。|
|変更|ベータ版|[educationSynchronizationError](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta) リソースの種類の説明テキストを更新しました。|
|変更|ベータ版|[同期エラー取得](/graph/api/educationsynchronizationerrors-get?view=graph-rest-beta) API の説明テキストを更新しました。|


### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-1.0)<br/>|
|追加|v1.0|新しい列挙型を追加しました。<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-1.0)<br/>|
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) エンティティに **managedDeviceOwnerType** プロパティを追加しました|
|追加|v1.0|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) エンティティに **deviceStatuses** ナビゲーション プロパティを追加しました|
|追加|v1.0|[policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-1.0) 列挙型に **androidWorkProfile** メンバーを追加しました|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofileeasemailprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate?view=graph-rest-beta)<br/>[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilewificonfiguration?view=graph-rest-beta)<br/>[restrictedAppsViolation](/graph/api/resources/intune-deviceconfig-restrictedappsviolation?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[managedDeviceModelsAndManufacturers](/graph/api/resources/intune-devices-manageddevicemodelsandmanufacturers?view=graph-rest-beta)<br/>[managedDeviceReportedApp](/graph/api/resources/intune-devices-manageddevicereportedapp?view=graph-rest-beta)<br/>[windowsEnrollmentStatusScreenSettings](/graph/api/resources/intune-enrollment-windowsenrollmentstatusscreensettings?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-beta)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-beta)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-beta)<br/>[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)<br/>[bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>[localSecurityOptionsInformationShownOnLockScreenType](/graph/api/resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype?view=graph-rest-beta)<br/>[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-beta)<br/>[restrictedAppsState](/graph/api/resources/intune-deviceconfig-restrictedappsstate?view=graph-rest-beta)<br/>[windows10VpnProfileTarget](/graph/api/resources/intune-deviceconfig-windows10vpnprofiletarget?view=graph-rest-beta)<br/>|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [playLostModeSound](/graph/api/intune-devices-manageddevice-playlostmodesound?view=graph-rest-beta) アクションを追加しました |
|削除|ベータ版|次の列挙型を削除しました。<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|追加|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **workProfileBlockScreenCapture** および **workProfileBlockCrossProfileCallerId** プロパティを追加しました|
|追加|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに **minimumWipePatchVersion**、**allowedAndroidDeviceManufacturers**、および **appActionIfAndroidDeviceManufacturerNotAllowed** プロパティを追加しました|
|追加|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **minimumWipeSdkVersion**、**minimumWipePatchVersion**、**allowedIosDeviceModels**、**appActionIfIosDeviceModelNotAllowed**、**allowedAndroidDeviceManufacturers**、および **appActionIfAndroidDeviceManufacturerNotAllowed** プロパティを追加しました|
|追加|ベータ版|[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) エンティティに **notApplicablePlatformCount** および **conflictCount** プロパティを追加しました|
|追加|ベータ版|[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) エンティティに **notApplicablePlatformCount** および **conflictCount** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **accountMoveCompletionDateTime** プロパティを追加しました|
|追加|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに **minimumWipeSdkVersion**、**allowedIosDeviceModels**、および **appActionIfIosDeviceModelNotAllowed** プロパティを追加しました|
|追加|ベータ版|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) エンティティに **minimumWipeOsVersion**、**minimumWipeAppVersion**、**appActionIfDeviceComplianceRequired**、および **appActionIfMaximumPinRetriesExceeded** プロパティを追加しました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **managedDeviceOwnerType**、**preferMdmOverGroupPolicyAppliedDateTime**、**isAutopilotEnrolled**、および **requestUserEnrollmentApproval** プロパティを追加しました|
|追加|ベータ版|[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) エンティティに **managedDeviceModelsAndManufacturers** プロパティを追加しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **localSecurityOptionsMachineInactivityLimitInMinutes**、**localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**、**localSecurityOptionsInformationShownOnLockScreen**、**defenderSecurityCenterDisableAccountUI**、**defenderSecurityCenterDisableHardwareUI**、**defenderSecurityCenterDisableRansomwareUI**、**defenderSecurityCenterDisableSecureBootUI**、および **defenderSecurityCenterDisableTroubleshootingUI** プロパティを追加しました|
|追加|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **printerNames**、**printerDefaultName**、**printerBlockAddition**、および **searchBlockWebResults** プロパティを追加しました|
|追加|ベータ版|[windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) エンティティに **profileTarget**、**enableAlwaysOn**、および **enableDeviceTunnel** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **enrollmentStatusScreenSettings** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **deviceConfigurationRestrictedAppsViolations** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta) エンティティに **networkAccessConfigurations** ナビゲーション プロパティを追加しました|
|削除|ベータ版|[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta) 複合型から **permissions** プロパティを削除しました|
|変更|ベータ版|[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta) 複合型で次のプロパティの型を変更しました。<br/>**recoveryInformationToStore** の型を [bitLockerRecoveryinformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) から [bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) に変更<br/>|
|追加|ベータ版|[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型に **deviceInactivityBeforeRetirementInDay** プロパティを追加しました|
|追加|ベータ版|[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 複合型に **landingPageCustomizedImage** プロパティを追加しました|
|削除|ベータ版|[vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) 複合型から **ipAddressOrFqdn** プロパティを削除しました|
|削除|ベータ版|[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) 複合型から **restartMode** プロパティを削除しました|
|追加|ベータ版|[androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-beta) 列挙型に **androidWorkProfile** メンバーが追加されました|

### <a name="microsoft-teams"></a>Microsoft Teams

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta) エンティティを追加しました。|
|追加|ベータ版|新しい [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-beta) エンティティを追加しました。|
|追加|ベータ版|新しい [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-beta) エンティティを追加しました。|
|追加|ベータ版|新しい [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-beta) エンティティを追加しました。|
|追加|ベータ版|新しい[チャネルの削除](/graph/api/channel-delete?view=graph-rest-beta)操作を追加しました。|
|追加|ベータ版|新しい[チャネルのパッチ適用](/graph/api/channel-patch?view=graph-rest-beta)操作を追加しました。|
|追加|ベータ版|[team](/graph/api/resources/team?view=graph-rest-beta) リソースに新たに webUrl プロパティを追加しました。|
|変更|ベータ版|[channel](/graph/api/resources/channel?view=graph-rest-beta) エンティティへのパスを更新しました。|

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0          | **locations** プロパティを [event](/graph/api/resources/event?view=graph-rest-1.0) エンティティに追加しました。これにより、出席者が複数の場所から出席できるイベントを開催できるようになりました。 |
| 追加        | v1.0          | **locationType** プロパティを [location](/graph/api/resources/location?view=graph-rest-1.0) 複合型に追加しました。 |
| 追加        | v1.0          | **uniqueId** および **uniqueIdType** プロパティが [location](/graph/api/resources/location?view=graph-rest-1.0) 複合型に追加されました。 これらのプロパティは、現時点では内部使用に限られます。 |


### <a name="outlook-contacts"></a>Outlook の連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0          | **flag** プロパティを [contact](/graph/api/resources/contact?view=graph-rest-1.0) エンティティに追加しました。 共有 [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) 複合型を追加しました。|


### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0          | **flag** プロパティを [message](/graph/api/resources/message?view=graph-rest-1.0) エンティティに追加しました。 共有 [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) 複合型を追加しました。|
| 追加        | v1.0        | **internetMessageHeaders** プロパティを [message](/graph/api/resources/message?view=graph-rest-1.0) エンティティに追加しました。 |
| 追加        | v1.0        | [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-1.0) 複合型を追加しました。 |
| 追加        | v1.0        | **messageRules** ナビゲーション プロパティを [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) エンティティに追加しました。 **messageRules** は [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) インスタンスのコレクションです。 |
| 追加        | v1.0        | [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) エンティティと、[messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-1.0)、[messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0)、[sizeRange](/graph/api/resources/sizerange?view=graph-rest-1.0) 複合型を追加しました。 |
| 追加        | v1.0        | メッセージ ルールに CRUD 操作 [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0)、[list](/graph/api/mailfolder-list-messagerules?view=graph-rest-1.0)、[get](/graph/api/messagerule-get?view=graph-rest-1.0)、[update](/graph/api/messagerule-update?view=graph-rest-1.0)、[delete](/graph/api/messagerule-delete?view=graph-rest-1.0) を追加しました。 |
| 追加 | ベータ版 | [mailSearchFolder](/graph/api/resources/mailsearchfolder?view=graph-rest-beta) を追加しました。 |
| 追加 | ベータ版 | メール検索フォルダーのために次の API を追加しました: [作成](/graph/api/mailsearchfolder-post?view=graph-rest-beta)、[更新](/graph/api/mailsearchfolder-update?view=graph-rest-beta)。 |
| 変更 | ベータ版 | メール検索フォルダーのサポートを追加しました: [mailFolder の削除](/graph/api/mailfolder-delete?view=graph-rest-beta)、[mailFolder の取得](/graph/api/mailfolder-get?view=graph-rest-beta)、[子フォルダーの一覧表示](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta)。 |


### <a name="outlook-user-choices"></a>Outlook ユーザーの選択

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しい **masterCategories** ナビゲーション プロパティを [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) エンティティに追加しました。 **masterCategories** は [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) オブジェクトのコレクションです。 |
| 追加        | v1.0        | [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) エンティティを追加しました。 |
| 追加        | v1.0        | [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) に CRUD 操作 [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0)、[get](/graph/api/outlookcategory-get?view=graph-rest-1.0)、[update](/graph/api/outlookcategory-update?view=graph-rest-1.0)、[delete](/graph/api/outlookcategory-delete?view=graph-rest-1.0) を追加しました。 |
| 追加        | v1.0        | 新しい [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-1.0) 関数を [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) エンティティに追加しました。 |
| 追加        | v1.0        | 新しい [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-1.0) 関数を [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0) エンティティに追加しました。 |
|追加 | v1.0 | 新しい **workingHours** プロパティを [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) に追加しました。 サポートされるユース ケースについては、「[workingHours リソース タイプ](/graph/api/resources/workinghours?view=graph-rest-1.0)」を参照してください。|
|追加 | v1.0 | 次の新しい複合型を追加しました。 <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-1.0) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-1.0) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-1.0) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-1.0)|


### <a name="project-rome-apis"></a>Project Rome API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加 | v1.0 | [Get recent activities API](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [Get activities API](/graph/api/projectrome-get-activities?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [Delete Activity](/graph/api/projectrome-delete-activity?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [activity](/graph/api/resources/projectrome-activity?view=graph-rest-1.0) を追加しました |
| 追加 | v.10 | [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [visualInfo](/graph/api/resources/projectrome-visualinfo?view=graph-rest-1.0) を追加しました |
| 追加 | v1.0 | [imageInfo](/graph/api/resources/projectrome-imageinfo?view=graph-rest-1.0) を追加しました |
| 追加 | v.10 | [Project Rome の概要](/graph/api/resources/project-rome-overview?view=graph-rest-1.0)を追加しました |
| 変更 | ベータ版 | [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) にディープ挿入のドキュメントを追加しました |

### <a name="reports-apis"></a>レポート API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版| 委任アクセスのサポートを追加しました。 |
|追加|v1.0| 委任アクセスのサポートを追加しました。 |

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | [セキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-beta) を追加しました。これには次のリソースと操作が含まれています。<br/>[警告](/graph/api/resources/alert?view=graph-rest-beta) (および関連するエンティティ)<br/>[警告の取得](/graph/api/alert-get?view=graph-rest-beta)<br/>[警告の一覧表示](/graph/api/alert-list?view=graph-rest-beta)<br/>[警告の更新](/graph/api/alert-update?view=graph-rest-beta)<br/><br/>次の関連ドキュメントを追加しました。<br/>[エラー](/graph/api/resources/security-error-codes?view=graph-rest-beta)<br/>[SIEM との統合](security-siemintegration.md)


## <a name="march-2018"></a>2018 年 3 月

### <a name="activityfeedservice-apis"></a>ActivityFeedService API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | [Get recent activities API](/graph/api/projectrome-get-recent-activities?view=graph-rest-beta) を追加しました |
| 追加        | ベータ版       | [Get activities API](/graph/api/projectrome-get-activities?view=graph-rest-beta) を追加しました |
| 変更 | ベータ版 | [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [Delete Activity](/graph/api/projectrome-delete-activity?view=graph-rest-beta) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [activity](/graph/api/resources/projectrome-activity?view=graph-rest-beta) に **status** プロパティを追加しました |
| 変更 | ベータ版 | [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) に **activity** ナビゲーション プロパティを追加しました |
| 変更 | ベータ版 | [Project Rome の概要](/graph/api/resources/project-rome-overview?view=graph-rest-beta)に新しい API を追加しました |

### <a name="azure-ad-apis"></a>Azure AD API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|変更|ベータ版|[サブスクリプション](/graph/api/resources/subscription?view=graph-rest-beta) リソースに **applicationID** および **creatorUserID** プロパティを追加しました。 |
|変更|ベータ版|[サブスクリプション](/graph/api/resources/subscription?view=graph-rest-beta) エンティティに[一覧表示](/graph/api/subscription-list?view=graph-rest-beta)操作を追加しました。 |

### <a name="data-policy-operations"></a>データ ポリシー操作

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティ [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-beta) を追加しました。 これは、追跡のために送信されたデータ ポリシー操作を表します。
| 追加        | ベータ版        | [users](/graph/api/resources/users?view=graph-rest-beta) に [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-beta) アクションを追加しました。 このアクションは、Microsoft がユーザー用に保存している個人データをエクスポートするためのデータ ポリシー操作要求を送信します。 |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | **onPremisesExtensionAttributes** 複合型を [user](/graph/api/resources/user?view=graph-rest-beta) エンティティに追加しました。 これにはオンプレミス AD の拡張属性 1 - 15 が含まれています。 |
| 追加        | ベータ版        | **privacyProfile** 複合型を [organization](/graph/api/resources/organization?view=graph-rest-beta) エンティティに追加しました。 |
| 追加        | v1.0        | [ユーザーとグループの復元と完全削除](/graph/api/resources/directory?view=graph-rest-1.0)に関するサポートを追加しました。 |

### <a name="excel-apis"></a>Excel API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|変更|v1.0|[Excel Table](/graph/api/resources/table?view=graph-rest-1.0) エンティティに **legacyId** プロパティを追加しました。 これには任意の Excel テーブルに対して定数となる数値識別子（文字列データ型）が含まれています。 これは、アプリケーションが古いバージョンの Excel クライアント アプリケーションで使用している従来の識別子に依存していた場合は、追加のメタデータとして提供されます。 注: `id` と `legacyId` プロパティはアプリケーションで符号化文字列値として処理し、その他の型に解析すべきではありません。 |

### <a name="group-lifecycle-policy"></a>グループのライフサイクル ポリシー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-1.0) を追加しました |
| 追加        | v1.0        | グループのライフサイクル ポリシーに、次の API を追加しました: [Create](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-1.0)、[List](/graph/api/grouplifecyclepolicy-list?view=graph-rest-1.0)、[Get](/graph/api/grouplifecyclepolicy-get?view=graph-rest-1.0)、[Update](/graph/api/grouplifecyclepolicy-update?view=graph-rest-1.0)、[Delete](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-1.0)、[Add group](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-1.0)、[Remove group](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-1.0) |
| 追加        | v1.0        | [group](/graph/api/resources/group?view=graph-rest-1.0) に [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-1.0) 関数を追加しました。 |
| 変更 | v1.0 | [group](/graph/api/resources/group?view=graph-rest-1.0) に renewedDateTime プロパティと [renew](/graph/api/group-renew?view=graph-rest-1.0) を追加しました |

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-1.0)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0)<br/>|
|追加|v1.0|新しい複合型を追加しました。<br/>[appConfigurationSettingItem](/graph/api/resources/intune-apps-appconfigurationsettingitem?view=graph-rest-1.0)<br/>|
|追加|v1.0|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0) に [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0) エンティティに **vppTokens** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **managementCertificateExpirationDate** プロパティを追加しました|
|追加|ベータ版|[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型に **enhancedJailBreak** プロパティを追加しました|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)<br/>[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta)<br/>[androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta)<br/>[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta)<br/>[macOSImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-macosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>[managedEBookCategory](/graph/api/resources/intune-books-managedebookcategory?view=graph-rest-beta)<br/>[microsoftStoreForBusinessContainedApp](/graph/api/resources/intune-apps-microsoftstoreforbusinesscontainedapp?view=graph-rest-beta)<br/>[mobileContainedApp](/graph/api/resources/intune-apps-mobilecontainedapp?view=graph-rest-beta)<br/>[windowsUniversalAppXContainedApp](/graph/api/resources/intune-apps-windowsuniversalappxcontainedapp?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceAndAppManagementData](/graph/api/resources/intune-onboarding-deviceandappmanagementdata?view=graph-rest-beta)<br/>[loggedOnUser](/graph/api/resources/intune-devices-loggedonuser?view=graph-rest-beta)<br/>[macOSFirewallApplication](/graph/api/resources/intune-deviceconfig-macosfirewallapplication?view=graph-rest-beta)<br/>[macOSLobChildApp](/graph/api/resources/intune-apps-macoslobchildapp?view=graph-rest-beta)<br/>[macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsappxappassignmentsettings?view=graph-rest-beta)<br/>[windowsUniversalAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsuniversalappxappassignmentsettings?view=graph-rest-beta)<br/>|
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) に [requestSignupUrl](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) に [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) に [syncApps](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) に [unbind](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) に [revokeToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) に [createToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta) に [consentToDataSharing](/graph/api/intune-devices-datasharingconsent-consenttodatasharing?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) に [getLoggedOnManagedDevices](/graph/api/intune-devices-user-getloggedonmanageddevices?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) に [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) に [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**appleVolumePurchaseProgramToken**<br/>**mdmAppConfigGroupAssignment**<br/>**windows10KioskConfiguration**<br/>|
|削除|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) の [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) アクションを削除しました |
|削除|ベータ版|[appleVolumePurchaseProgramToken](/graph/api/resources/intune-onboarding-applevolumepurchaseprogramtoken?view=graph-rest-beta) の [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-syncapps?view=graph-rest-beta) アクションを削除しました |
|追加|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**workProfileBluetoothEnableContactSharing** プロパティを追加しました|
|追加|ベータ版|[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) エンティティに **encodedSettingXml** プロパティを追加しました|
|追加|ベータ版|[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) エンティティに **managedDeviceId** プロパティと** azureADDeviceId** プロパティを追加しました|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **usersLoggedOn** プロパティを追加しました|
|削除|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティから**lastLoggedOnUserId** プロパティを削除しました|
|追加|ベータ版|[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) エンティティに **lastModifiedDateTime** プロパティを追加しました|
|追加|ベータ版|[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) エンティティに **isDependency** プロパティを追加しました|
|追加|ベータ版|[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta) エンティティに**windowsEnabled** プロパティ、**macEnabled** プロパティ、**windowsDeviceBlockedOnMissingPartnerData** プロパティ、**macDeviceBlockedOnMissingPartnerData** プロパティを追加しました|
|追加|ベータ版|[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティに　**shouldUninstallOlderVersionsOfOffice** プロパティを追加しました|
|追加|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) エンティティに **dataSharingConsentGranted** プロパティを追加しました|
|追加|ベータ版|**localSecurityOptionsBlockRemoteLogonWithBlankPassword**, **localSecurityOptionsAdministratorAccountName**, **localSecurityOptionsEnableGuestAccount**, **localSecurityOptionsGuestAccountName**, **localSecurityOptionsAllowUndockWithoutHavingToLogon**, **localSecurityOptionsBlockUsersInstallingPrinterDrivers**, **localSecurityOptionsBlockRemoteOpticalDriveAccess**, **localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser**, **localSecurityOptionsMachineInactivityLimit**, **localSecurityOptionsDoNotRequireCtrlAltDel**, **localSecurityOptionsInformationDisplayedOnLockScreen**, **localSecurityOptionsHideLastSignedInUser**, **localSecurityOptionsHideUsernameAtSignIn**, **localSecurityOptionsLogOnMessageTitle**, **localSecurityOptionsLogOnMessageText**, **localSecurityOptionsAllowPKU2UAuthenticationRequests**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager**, **localSecurityOptionsClearVirtualMemoryPageFile**, **localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn**, **localSecurityOptionsAllowUIAccessApplicationElevation**, **localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations**, **localSecurityOptionsOnlyElevateSignedExecutables**, **localSecurityOptionsAdministratorElevationPromptBehavior**, **localSecurityOptionsStandardUserElevationPromptBehavior**, **localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation**, **localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation**, **localSecurityOptionsAllowUIAccessApplicationsForSecureLocations**, **localSecurityOptionsUseAdminApprovalMode**, **localSecurityOptionsUseAdminApprovalModeForAdministrators**, **deviceGuardLocalSystemAuthorityCredentialGuardSettings**, **deviceGuardEnableVirtualizationBasedSecurity** and **deviceGuardEnableSecureBootWithDMA** プロパティを [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに追加しました|
|削除|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティから **defenderPasswordProtectedEmailContentExecutionType** プロパティを削除しました|
|追加|ベータ版|[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta) エンティティに **intendedPurpose** プロパティを追加しました|
|削除|ベータ版|[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) エンティティから **printerNames** プロパティ、**defaultPrinterName** プロパティ、**blockAddingNewPrinter** プロパティを削除しました|
|追加|ベータ版|[windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) エンティティに **certificateStore** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) エンティティに **purchaseOrderIdentifier** プロパティを追加しました|
|変更|ベータ版|[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**subjectAlternativeNameType**を必須からオプションに変更しました<br/>|
|追加|ベータ版|[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta) エンティティに **advancedThreatProtectionOnboardingFilename** プロパティと **advancedThreatProtectionOffboardingFilename** プロパティを追加しました|
|追加|ベータ版|[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティに **skipChecksBeforeRestart** プロパティと **updateWeeks** プロパティを追加しました|
|追加|ベータ版|[deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **managedEBookCategorie** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **androidManagedStoreAccountEnterpriseSettings** ナビゲーション プロパティ、**androidManagedStoreAppConfigurationSchemas** ナビゲーション プロパティ、**androidDeviceOwnerEnrollmentProfiles** ナビゲーション プロパティ、**dataSharingConsents** ナビゲーション プロパティ、**deviceConfigurationUserStateSummaries** ナビゲーション プロパティを追加しました|
|削除|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティから**deviceSetupConfigurations** ナビゲーション プロパティを削除しました|
|削除|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|追加|ベータ版|[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) エンティティに **categories** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta) エンティティに **containedApps** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-beta) エンティティに **containedApps** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) エンティティに **committedContainedApps** ナビゲーション プロパティを追加しました|

### <a name="onedrive"></a>OneDrive
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[baseItemVersion](/graph/api/resources/baseitemversion?view=graph-rest-1.0)<br/>[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0)<br/>[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0)<br/> |
|追加|v1.0|新しい複合型を追加しました。<br/>[publicationFacet](/graph/api/resources/publicationfacet?view=graph-rest-1.0)<br/> |
|追加|v1.0|[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) エンティティに <b>publication</b> プロパティを追加しました |
|追加|v1.0|[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) エンティティに <b>versions</b> ナビゲーション プロパティを追加しました |
|追加|v1.0|[listItem](/graph/api/resources/listitem?view=graph-rest-1.0) エンティティに <b>versions</b> ナビゲーション プロパティを追加しました |
|追加|v1.0|[siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0) エンティティに <b>root</b> プロパティを追加しました |
|追加|v1.0|[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0) エンティティに [restoreVersion](/graph/api/driveitemversion-restore?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0) エンティティに [restoreVersion](/graph/api/listitemversion-restore?view=graph-rest-1.0) アクションを追加しました |


### <a name="onedrive"></a>OneDrive
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい複合型を追加しました。<br/>[itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-beta)<br/> |
|追加|ベータ版|[contentTypeInfo](/graph/api/resources/contenttypeinfo?view=graph-rest-beta) 複合型に <b>name</b> プロパティを追加しました |
|追加|ベータ版|[deleteAction](/graph/api/resources/deleteaction?view=graph-rest-beta) 複合型に <b>objectType</b> プロパティを追加しました |
|追加|ベータ版|[renameAction](/graph/api/resources/renameaction?view=graph-rest-beta) 複合型に <b>newName</b> プロパティを追加しました |
|追加|ベータ版|[SharepointIds](/graph/api/resources/renameaction?view=graph-rest-beta) 複合型に <b>tenantId</b> プロパティを追加しました |
|追加|ベータ版|[itemActivityTimeSet](/graph/api/resources/itemactivitytimeset?view=graph-rest-beta) 複合型に <b>lastRecordedDateTime</b> プロパティを追加しました |
|追加|ベータ版|[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) エンティティに [preview](/graph/api/driveitem-preview?view=graph-rest-beta) アクションを追加しました |

### <a name="reports-apis"></a>レポート API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|追加|ベータ版|[sharePointSiteUsageDetail](/graph/api/resources/sharepointsiteusagedetail?view=graph-rest-beta) エンティティに **siteId** プロパティを追加しました。|

### <a name="terms-of-use"></a>利用規約

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [agreement](/graph/api/resources/agreement?view=graph-rest-beta) と [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) リソースを追加しました。 |
| 追加        | ベータ版        | 次の [agreement](/graph/api/resources/agreement?view=graph-rest-beta) のAPI を追加しました: [Create](/graph/api/greement-post-agreements?view=graph-rest-beta), [List](/graph/api/agreement-list?view=graph-rest-beta), [Get](/graph/api/agreement-get?view=graph-rest-beta), [Update](/graph/api/agreement-update?view=graph-rest-beta), [Delete](/graph/api/agreement-delete?view=graph-rest-beta)。 |
| 追加        | ベータ版        | [user](/graph/api/resources/user?view=graph-rest-beta) リソースに [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) リレーションシップを追加しました。 |

## <a name="february-2018"></a>2018 年 2 月

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10KioskConfiguration](/graph/api/resources/intune-deviceconfig-windows10kioskconfiguration?view=graph-rest-beta)<br/>[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[importedWindowsAutopilotDeviceIdentityState](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate?view=graph-rest-beta)<br/>|
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) 機能を追加しました |
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) 機能を追加しました |
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentFailureTrends](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuretrends?view=graph-rest-beta) 機能を追加しました |
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) 機能を追加しました |
|追加|ベータ版|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) 機能を追加しました |
|変更|ベータ版|[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティから、プロパティ **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** を削除しました|
|変更|ベータ版|[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) エンティティから、プロパティ **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** を削除しました|
|変更|ベータ版|[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) エンティティから、プロパティ **name**、**modifiedDateTime**、**totalEnrollmentCount**、**qrCode** を削除しました。|
|変更|ベータ版|[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap**、**enableOuterIdentityPrivacy** を削除しました|
|変更|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**workProfileBlockAddingAccounts** プロパティを追加しました|
|変更|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから、プロパティ **blockCrossProfileCopyPaste** と **requireAppVerify** を削除しました|
|変更|ベータ版|[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) エンティティに、**deviceOwnerManagementEnabled** プロパティを追加しました|
|変更|ベータ版|[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから **requireAppVerify** プロパティを削除しました。|
|変更|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに、**exemptedAppPackages** プロパティを追加しました|
|変更|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに、プロパティ **exemptedAppProtocols** と **exemptedAppPackages** を追加しました。|
|変更|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに、プロパティ **exemptedAppProtocols**を追加しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、**lastLoggedOnUserId** プロパティを追加しました|
|変更|ベータ版|[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) エンティティに **isFrameworkFile** プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) エンティティに、**targetedAppManagementLevels** プロパティを追加しました|
|変更|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに、プロパティ **localSecurityOptionsBlockMicrosoftAccounts**、**localSecurityOptionsEnableAdministratorAccount**、**defenderPreventCredentialStealingType**、**defenderProcessCreationType**、**defenderUntrustedUSBProcessType**、**defenderUntrustedExecutableType**、**defenderPasswordProtectedEmailContentExecutionType**、**defenderAdvancedRansomewareProtectionType**、**applicationGuardAllowFileSaveOnHost** を追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、プロパティ **edgeFavoritesListLocation** と **edgeBlockEditFavorites** を追加しました|
|変更|ベータ版|[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) エンティティに、プロパティ **printerNames**、**defaultPrinterName**、**blockAddingNewPrinter** を追加しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **importedWindowsAutopilotDeviceIdentities** を追加しました|
|変更|ベータ版|[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) 複合型に、**shareAPNSData** プロパティを追加しました|
|変更|ベータ版|[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta) 複合型から、**collectFullIOSAppInventory** プロパティを削除しました|
|変更|ベータ版|[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 複合型から、**deviceUsageType** プロパティを追加しました|


### <a name="planner-apis"></a>Planner API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい複合型を追加しました。<br/>[plannerPlanContext](/graph/api/resources/plannerplancontext?view=graph-rest-beta)<br/>[plannerPlanContextDetails](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta)<br/>[plannerPlanContextCollection](/graph/api/resources/plannerplancontextcollection?view=graph-rest-beta)<br/>[plannerPlanContextDetailsCollection](/graph/api/resources/plannerplancontextdetailscollection?view=graph-rest-beta)<br/>[plannerFavoritePlanReference](/graph/api/resources/plannerfavoriteplanreference?view=graph-rest-beta)<br/>[plannerRecentPlanReference](/graph/api/resources/plannerrecentplanreference?view=graph-rest-beta)<br/>[plannerFavoritePlanReferenceCollection](/graph/api/resources/plannerfavoriteplanreferencecollection?view=graph-rest-beta)<br/>[plannerRecentPlanReferenceCollection](/graph/api/resources/plannerrecentplanreferencecollection?view=graph-rest-beta)|
|追加|ベータ版|`favoritePlanReferences` と `recentPlanReferences` プロパティを [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) エンティティに追加しました。 |
|追加|ベータ版|`favoritePlans` と `recentPlans` ナビゲーション プロパティを [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) エンティティに追加しました。 |
|追加|ベータ版|`contexts` プロパティを [plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) エンティティに追加しました。 |
|追加|ベータ版|[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) エンティティに `contextDetails` プロパティを追加しました。 |
|追加|ベータ版|Planner の[デルタ クエリ](/graph/api/planneruser-list-delta?view=graph-rest-beta)を追加しました |

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | ベータ版    | **activatedOnSharedComputer** プロパティを [userActivationCounts](/graph/api/resources/useractivationcounts?view=graph-rest-beta) エンティティに追加しました。|
| 追加    | ベータ版    | **sharedComputerActivation** プロパティを [office365ActivationsUserCounts](/graph/api/resources/office365activationsusercounts?view=graph-rest-beta) エンティティに追加しました。|

## <a name="january-2018"></a>2018 年 1 月

### <a name="education-apis"></a>教育機関 API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|[名簿 API](/graph/api/resources/education-overview?view=graph-rest-beta) の他のナビゲーション プロパティを追加し、フィルター処理のサポートを改善しました。|

### <a name="json-batching"></a>JSON バッチ処理

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|[JSON バッチ処理](json-batching.md)のサポートを追加しました。 内部要求の制限を 20 に設定しました。|
|変更|ベータ版|[JSON バッチ処理](json-batching.md)の内部要求の制限を 5 から 20 に増やしました。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-1.0)<br/>[androidCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidcustomconfiguration?view=graph-rest-1.0)<br/>[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-1.0)<br/>[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0)<br/>[androidManagedAppRegistration](/graph/api/resources/intune-mam-androidmanagedappregistration?view=graph-rest-1.0)<br/>[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-1.0)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-1.0)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0)<br/>[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-1.0)<br/>[detectedApp](/graph/api/resources/intune-devices-detectedapp?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-1.0)<br/>[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0)<br/>[deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-1.0)<br/>[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-1.0)<br/>[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-1.0)<br/>[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0)<br/>[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-1.0)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-1.0)<br/>[deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-1.0)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-1.0)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-1.0)<br/>[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-1.0)<br/>[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)<br/>[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-1.0)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-1.0)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-1.0)<br/>[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-1.0)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-1.0)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-1.0)<br/>[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0)<br/>[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-1.0)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-1.0)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)<br/>[editionUpgradeConfiguration](/graph/api/resources/intune-deviceconfig-editionupgradeconfiguration?view=graph-rest-1.0)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-1.0)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-1.0)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-1.0)<br/>[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-1.0)<br/>[iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-1.0)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-1.0)<br/>[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0)<br/>[iosManagedAppRegistration](/graph/api/resources/intune-mam-iosmanagedappregistration?view=graph-rest-1.0)<br/>[iosStoreApp](/graph/api/resources/intune-apps-iosstoreapp?view=graph-rest-1.0)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-1.0)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-1.0)<br/>[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-1.0)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-1.0)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-1.0)<br/>[localizedNotificationMessage](/graph/api/resources/intune-notification-localizednotificationmessage?view=graph-rest-1.0)<br/>[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0)<br/>[macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-1.0)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-1.0)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-1.0)<br/>[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-1.0)<br/>[managedApp](/graph/api/resources/intune-apps-managedapp?view=graph-rest-1.0)<br/>[managedAppConfiguration](/graph/api/resources/intune-mam-managedappconfiguration?view=graph-rest-1.0)<br/>[managedAppOperation](/graph/api/resources/intune-mam-managedappoperation?view=graph-rest-1.0)<br/>[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummary](/graph/api/resources/intune-mam-managedapppolicydeploymentsummary?view=graph-rest-1.0)<br/>[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0)<br/>[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0)<br/>[managedAppStatus](/graph/api/resources/intune-mam-managedappstatus?view=graph-rest-1.0)<br/>[managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-1.0)<br/>[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-1.0)<br/>[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-1.0)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-1.0)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-1.0)<br/>[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-1.0)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-1.0)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-1.0)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-1.0mwindowsinformationprotectionpolicy)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-1.0)<br/>[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-1.0)<br/>[mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-1.0)<br/>[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-1.0)<br/>[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0)<br/>[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-1.0)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-1.0)<br/>[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0)<br/>[onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0)<br/>[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-1.0)<br/>[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-1.0)<br/>[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-1.0)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-1.0)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-1.0)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-1.0)<br/>[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0)<br/>targetedManagedAppPolicyAssignment<br/>[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0)<br/>[telecomExpenseManagementPartner](/graph/api/resources/intune-tem-telecomexpensemanagementpartner?view=graph-rest-1.0)<br/>[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-1.0)<br/>[termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus?view=graph-rest-1.0)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-1.0)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-1.0)<br/>[webApp](/graph/api/resources/intune-apps-webapp?view=graph-rest-1.0)<br/>[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-1.0)<br/>[windows10CustomConfiguration](/graph/api/resources/intune-deviceconfig-windows10customconfiguration?view=graph-rest-1.0)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-1.0)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-1.0)<br/>[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)<br/>[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-1.0)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-1.0)<br/>[windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-1.0)<br/>[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-1.0)<br/>[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-1.0)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-1.0)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-1.0)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-1.0)<br/>[windowsPhone81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windowsphone81compliancepolicy?view=graph-rest-1.0)<br/>[windowsPhone81CustomConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81customconfiguration?view=graph-rest-1.0)<br/>[windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-1.0)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-1.0)<br/>[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-1.0)<br/>|
|追加|v1.0|新しい複合型を追加しました。<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-1.0)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-1.0)<br/>[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-1.0)<br/>[androidMobileAppIdentifier](/graph/api/resources/intune-mam-androidmobileappidentifier?view=graph-rest-1.0)<br/>[appListItem](/graph/api/resources/intune-deviceconfig-applistitem?view=graph-rest-1.0)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-1.0)<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-1.0)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-1.0)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devices-deleteuserfromsharedappledeviceactionresult?view=graph-rest-1.0)<br/>[deviceActionResult](/graph/api/resources/intune-devices-deviceactionresult?view=graph-rest-1.0)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-1.0)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-1.0)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-devices-deviceexchangeaccessstatesummary?view=graph-rest-1.0)<br/>[deviceGeoLocation](/graph/api/resources/intune-devices-devicegeolocation?view=graph-rest-1.0)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-1.0)<br/>[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-1.0)<br/>[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-1.0)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-1.0)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-1.0)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-1.0)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-1.0)<br/>[fileEncryptionInfo](/graph/api/resources/intune-apps-fileencryptioninfo?view=graph-rest-1.0)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-1.0)<br/>[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-1.0)<br/>[iosDeviceType](/graph/api/resources/intune-apps-iosdevicetype?view=graph-rest-1.0)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-1.0)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-1.0)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-1.0)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-1.0)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-1.0)<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-1.0)<br/>[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)<br/>[iosMobileAppIdentifier](/graph/api/resources/intune-mam-iosmobileappidentifier?view=graph-rest-1.0)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-1.0)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-1.0)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-1.0)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-1.0)<br/>[ipRange](/graph/api/resources/intune-mam-iprange?view=graph-rest-1.0)<br/>[iPv4Range](/graph/api/resources/intune-mam-ipv4range?view=graph-rest-1.0)<br/>[iPv6Range](/graph/api/resources/intune-mam-ipv6range?view=graph-rest-1.0)<br/>[keyValuePair](/graph/api/resources/intune-androidforwork-keyvaluepair?view=graph-rest-1.0)<br/>[locateDeviceActionResult](/graph/api/resources/intune-devices-locatedeviceactionresult?view=graph-rest-1.0)<br/>[managedAppDiagnosticStatus](/graph/api/resources/intune-mam-managedappdiagnosticstatus?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummaryPerApp](/graph/api/resources/intune-mam-managedapppolicydeploymentsummaryperapp?view=graph-rest-1.0)<br/>[mediaContentRatingAustralia](/graph/api/resources/intune-deviceconfig-mediacontentratingaustralia?view=graph-rest-1.0)<br/>[mediaContentRatingCanada](/graph/api/resources/intune-deviceconfig-mediacontentratingcanada?view=graph-rest-1.0)<br/>[mediaContentRatingFrance](/graph/api/resources/intune-deviceconfig-mediacontentratingfrance?view=graph-rest-1.0)<br/>[mediaContentRatingGermany](/graph/api/resources/intune-deviceconfig-mediacontentratinggermany?view=graph-rest-1.0)<br/>[mediaContentRatingIreland](/graph/api/resources/intune-deviceconfig-mediacontentratingireland?view=graph-rest-1.0)<br/>[mediaContentRatingJapan](/graph/api/resources/intune-deviceconfig-mediacontentratingjapan?view=graph-rest-1.0)<br/>[mediaContentRatingNewZealand](/graph/api/resources/intune-deviceconfig-mediacontentratingnewzealand?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedKingdom](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedkingdom?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedStates](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedstates?view=graph-rest-1.0)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-1.0)<br/>[mimeContent](/graph/api/resources/intune-shared-mimecontent?view=graph-rest-1.0)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-1.0)<br/>[mobileAppIdentifier](/graph/api/resources/intune-mam-mobileappidentifier?view=graph-rest-1.0)<br/>[omaSetting](/graph/api/resources/intune-deviceconfig-omasetting?view=graph-rest-1.0)<br/>[omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-1.0)<br/>[omaSettingBoolean](/graph/api/resources/intune-deviceconfig-omasettingboolean?view=graph-rest-1.0)<br/>[omaSettingDateTime](/graph/api/resources/intune-deviceconfig-omasettingdatetime?view=graph-rest-1.0)<br/>[omaSettingFloatingPoint](/graph/api/resources/intune-deviceconfig-omasettingfloatingpoint?view=graph-rest-1.0)<br/>[omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-1.0)<br/>[omaSettingString](/graph/api/resources/intune-deviceconfig-omasettingstring?view=graph-rest-1.0)<br/>[omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-1.0)<br/>[proxiedDomain](/graph/api/resources/intune-mam-proxieddomain?view=graph-rest-1.0)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-1.0)<br/>[resetPasscodeActionResult](/graph/api/resources/intune-devices-resetpasscodeactionresult?view=graph-rest-1.0)<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-1.0)<br/>[rgbColor](/graph/api/resources/intune-onboarding-rgbcolor?view=graph-rest-1.0)<br/>[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-1.0)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-1.0)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-1.0)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-1.0)<br/>[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-1.0)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-1.0)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-1.0)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-1.0)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-1.0)<br/>[windowsDeviceAzureADAccount](/graph/api/resources/intune-devices-windowsdeviceazureadaccount?view=graph-rest-1.0)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-1.0)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-1.0)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-1.0)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-1.0)<br/>[windowsUpdateActiveHoursInstall](/graph/api/resources/intune-deviceconfig-windowsupdateactivehoursinstall?view=graph-rest-1.0)<br/>[windowsUpdateInstallScheduleType](/graph/api/resources/intune-deviceconfig-windowsupdateinstallscheduletype?view=graph-rest-1.0)<br/>[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-1.0)<br/>|
|追加|v1.0|[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) に [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) に [commit](/graph/api/intune-apps-mobileappcontentfile-commit?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) に [renewUpload](/graph/api/intune-apps-mobileappcontentfile-renewupload?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [retire](/graph/api/intune-devices-manageddevice-retire?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [resetPasscode](/graph/api/intune-devices-manageddevice-resetpasscode?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [remoteLock](/graph/api/intune-devices-manageddevice-remotelock?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [disableLostMode](/graph/api/intune-devices-manageddevice-disablelostmode?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [locateDevice](/graph/api/intune-devices-manageddevice-locatedevice?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [bypassActivationLock](/graph/api/intune-devices-manageddevice-bypassactivationlock?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [rebootNow](/graph/api/intune-devices-manageddevice-rebootnow?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) に [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-1.0) を追加しました |
|追加|v1.0|[user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) に [removeAllDevicesFromManagement](/graph/api/intune-devices-user-removealldevicesfrommanagement?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) に [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) に [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) に [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0) に [setMobileDeviceManagementAuthority](/graph/api/intune-onboarding-organization-setmobiledevicemanagementauthority?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0) に [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) に [sync](/graph/api/intune-onboarding-devicemanagementexchangeconnector-sync?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) に [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) に [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0) に [assign](/graph/api/intune-mam-targetedmanagedappprotection-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) に [assign](/graph/api/intune-mam-targetedmanagedappconfiguration-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0) に [assign](/graph/api/intune-mam-windowsinformationprotection-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0) に [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0) に [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) に [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) に [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0) に [sendTestMessage](/graph/api/intune-notification-notificationmessagetemplate-sendtestmessage?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0) に [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) に [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) に [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-1.0) アクションを追加しました |
|追加|v1.0|[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0) に [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) に [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) に [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) に [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0) コレクションに **getUserIdsWithFlaggedAppRegistration** 関数を追加しました |
|追加|v1.0|[user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) に [getManagedAppDiagnosticStatuses](/graph/api/intune-mam-user-getmanagedappdiagnosticstatuses?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) に [getManagedAppPolicies](/graph/api/intune-mam-user-getmanagedapppolicies?view=graph-rest-1.0) 関数を追加しました |
|追加|v1.0|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) に [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-1.0) 関数を追加しました |
|変更|v1.0|[organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0) エンティティに **mobileDeviceManagementAuthority** プロパティを追加しました|
|変更|v1.0|[user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) エンティティに **deviceEnrollmentLimit** プロパティを追加しました|
|変更|v1.0|[user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) エンティティに **managedDevices**、**managedAppRegistrations**、**deviceManagementTroubleshootingEvents** ナビゲーション プロパティを追加しました|
|||
|追加|ベータ版|新しいエンティティを追加しました。<br/>[deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[revokeAppleVppLicensesActionResult](/graph/api/resources/intune-devices-revokeapplevpplicensesactionresult?view=graph-rest-beta)<br/>[vppTokenRevokeLicensesActionResult](/graph/api/resources/intune-onboarding-vpptokenrevokelicensesactionresult?view=graph-rest-beta)<br/>|
|追加|ベータ版|[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) に [revokeToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) に [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) に [assign](/graph/api/intune-devices-devicemanagementscript-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [revokeAppleVppLicenses](/graph/api/intune-devices-manageddevice-revokeapplevpplicenses?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) に [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) に [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) に [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) に [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) に [getEffectiveDeviceEnrollmentConfigurations](/graph/api/intune-onboarding-user-geteffectivedeviceenrollmentconfigurations?view=graph-rest-beta) 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**appReportingOverviewStatus**<br/>**complianceSettingStateSummary**<br/>**deviceConfigurationUserStateSummary**<br/>**eBookGroupAssignment**<br/>**eBookVppGroupAssignment**<br/>**mobileAppGroupAssignment**<br/>**mobileAppVppGroupAssignment**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**androidForWorkAppConfigurationExample**<br/>**androidForWorkAppConfigurationExampleJson**<br/>**appInstallationFailure**<br/>**appsComplianceListItem**<br/>**defaultDeviceEnrollmentRestrictions**<br/>**defaultDeviceEnrollmentWindowsHelloForBusinessSettings**<br/>**deviceEnrollmentPlatformRestrictions**<br/>|
|変更|ベータ版|[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティに **securityRequireVerifyApps**、**securityRequireSafetyNetAttestationBasicIntegrity**、**securityRequireSafetyNetAttestationCertifiedDevice**、**securityRequireGooglePlayServices**、**securityRequireUpToDateSecurityProviders**、**securityRequireCompanyPortalAppIntegrity** プロパティを追加しました|
|変更|ベータ版|[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta) エンティティに **packageId** プロパティを追加しました|
|変更|ベータ版|[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**exampleJson** を [androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta) からバイナリに変更しました<br/>|
|変更|ベータ版|[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) エンティティに **securityRequireVerifyApps**、**securityRequireSafetyNetAttestationBasicIntegrity**、**securityRequireSafetyNetAttestationCertifiedDevice**、**securityRequireGooglePlayServices**、**securityRequireUpToDateSecurityProviders**、**securityRequireCompanyPortalAppIntegrity** プロパティを追加しました|
|変更|ベータ版|[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) エンティティに **displayName**、**lastModifiedDateTime**、**enrolledDeviceCount**、**qrCodeContent**、**qrCodeImage** プロパティを追加しました|
|変更|ベータ版|[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) エンティティから **isTokenActive** プロパティを削除しました|
|変更|ベータ版|[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta) エンティティに、**innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap**、**outerIdentityPrivacyTemporaryValue** プロパティを追加しました|
|変更|ベータ版|[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、**workProfileBlockCrossProfileCopyPaste** と **securityRequireVerifyApps** プロパティを追加しました|
|変更|ベータ版|[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **securityRequireVerifyApps** プロパティを追加しました|
|変更|ベータ版|[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta) エンティティに **packageId** と **identityVersion** プロパティを追加しました|
|変更|ベータ版|[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta) エンティティに **packageId** プロパティを追加しました|
|変更|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **faceIdBlocked** プロパティを追加しました|
|変更|ベータ版|[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) エンティティに **members** プロパティを追加しました|
|変更|ベータ版|[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta) エンティティに **macOSRestriction** プロパティを追加しました|
|変更|ベータ版|[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta) エンティティに **whenPartnerDevicesWillBeRemovedDateTime** と **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** プロパティを追加しました|
|変更|ベータ版|[deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**scriptContent** を文字列からバイナリに変更しました<br/>|
|変更|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティに **smimeEnablePerMessageSwitch** プロパティを追加しました|
|変更|ベータ版|[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに **faceIdBlocked** プロパティを追加しました|
|変更|ベータ版|[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) エンティティに **packageId** と **identityVersion** プロパティを追加しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **azureADDeviceId** と **remoteAssistanceSessionErrorDetails** プロパティを追加しました|
|変更|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティから、**legacyAppConfiguration** プロパティを削除しました|
|変更|ベータ版|[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta) エンティティから **identityVersion** プロパティを削除しました|
|変更|ベータ版|[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) エンティティに **publishingState** プロパティを追加しました|
|変更|ベータ版|[mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティに **installState** プロパティを追加しました|
|変更|ベータ版|[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-beta) エンティティから **identityVersion** プロパティを削除しました|
|変更|ベータ版|[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta) エンティティに **allowPartnerToCollectIOSApplicationMetadata** プロパティを追加しました|
|変更|ベータ版|[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) エンティティから **members** プロパティを削除しました|
|変更|ベータ版|[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta) エンティティに **lastModifiedDateTime** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティに **deviceThreatProtectionEnabled** と **deviceThreatProtectionRequiredSecurityLevel** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティから **minimumUpdateAutoInstallClassification** プロパティを削除しました|
|変更|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **privacyBlockPublishUserActivities** と **privacyBlockActivityFeed** プロパティを追加しました|
|変更|ベータ版|[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) エンティティに **configurationAccountType** プロパティを追加しました|
|変更|ベータ版|[windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) エンティティから **trustedNetworkDomains** プロパティを削除しました|
|変更|ベータ版|[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta) エンティティから **minimumUpdateAutoInstallClassification** プロパティを削除しました|
|変更|ベータ版|[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta) エンティティに **daysWithoutContactBeforeUnenroll** プロパティを追加しました|
|変更|ベータ版|[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta) エンティティに **domainJoinConfiguration** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) エンティティから **notificationMessageTemplate** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **windowsInformationProtectionNetworkLearningSummaries** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティから、**deviceConfigurationUserStateSummaries** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**roleAssignments** を [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) コレクションから [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta) コレクションに変更しました<br/>|
|変更|ベータ版|[deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティに **smimeEncryptionCertificate** プロパティを追加しました|
|変更|ベータ版|[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**smimeSigningCertificate** を [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) から [iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta) に変更しました<br/>|
|変更|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) エンティティから **vppToken** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) エンティティから **depOnboardingSettings** と **appleVolumePurchaseProgramTokens** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) エンティティに **deviceEnrollmentConfigurations** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型から **windowsCommercialId** プロパティと **windowsCommercialIdLastModifiedTime** プロパティを削除しました|
|変更|ベータ版|[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta) 複合型に **showDisplayNameNextToLogo** プロパティを追加しました|
|変更|ベータ版|[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta) 複合型に **deviceUsageType** プロパティを追加しました|
|変更|ベータ版|[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-beta) 複合型に **supportsUserLicensing** と **supportsDeviceLicensing** プロパティを追加しました|
|変更|ベータ版|[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta) 複合型から **actionMessage** プロパティを削除しました|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | v1.0    | 以下の API を追加しました。<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-1.0)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-1.0)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-1.0) |

## <a name="december-2017"></a>2017 年 12 月

### <a name="delta-query"></a>デルタ クエリ

| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 変更      | v1.0    | [users](/graph/api/user-delta?view=graph-rest-1.0) と [groups](/graph/api/group-delta?view=graph-rest-1.0) に、オプションのクエリ フィルタリング機能を追加します。 |

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-beta)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-beta)<br/>[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta)<br/>[windowsDeviceAADAccount](/graph/api/resources/intune-devices-windowsdeviceaadaccount?view=graph-rest-beta)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-beta)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-beta)<br/>|
|追加|ベータ版|[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) に [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketokens?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) に [createToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-createtoken?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-beta) を追加しました |
|追加|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) に [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) コレクションに [getDevicePasscode](/graph/api/intune-deviceconfig-devicecompliancepolicy-getdevicepasscode?view=graph-rest-beta) 関数を追加しました |
|追加|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) に [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-beta) 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**windowsStoreForBusinessApp**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**windowsStoreForBusinessAppAssignmentSettings**<br/>|
|変更|ベータ版|[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **dateAndTimeBlockChanges** プロパティを追加しました|
|変更|ベータ版|[depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) エンティティから **enableAuthenticationViaCompanyPortal** プロパティを削除しました|
|変更|ベータ版|[deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティから **windowsStoreForBusinessLastSuccessfulSyncDateTime** プロパティ、**isEnabledForWindowsStoreForBusiness** プロパティ、**windowsStoreForBusinessLanguage** プロパティ、**windowsStoreForBusinessLastCompletedApplicationSyncTime** プロパティを削除しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **maximumDepTokens** プロパティと **intuneAccountId** プロパティを追加しました|
|変更|ベータ版|[enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) エンティティに **enableAuthenticationViaCompanyPortal** プロパティを追加しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **managedDeviceName** プロパティと **partnerReportedThreatState** プロパティを追加しました|
|変更|ベータ版|[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティに **installProgressDisplayLevel** プロパティを追加しました|
|変更|ベータ版|[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) エンティティに **resourceScopes** プロパティを追加しました|
|変更|ベータ版|[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-beta) エンティティに **rolePermissions** プロパティと **isBuiltIn** プロパティを追加しました|
|変更|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) エンティティに **tokenActionResults** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)エンティティに **minimumUpdateAutoInstallClassification** プロパティを追加しました|
|変更|ベータ版|[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **defenderSecurityCenterDisableAppBrowserUI** プロパティ、**defenderSecurityCenterDisableFamilyUI** プロパティ、**defenderSecurityCenterDisableHealthUI**, **defenderSecurityCenterDisableNetworkUI** プロパティ、**defenderSecurityCenterDisableVirusUI** プロパティ、**defenderSecurityCenterOrganizationDisplayName**, **defenderSecurityCenterHelpEmail** プロパティ、**defenderSecurityCenterHelpPhone** プロパティ、**defenderSecurityCenterHelpURL** プロパティ、**defenderSecurityCenterNotificationsFromApp** プロパティ、**defenderSecurityCenterITContactDisplay** プロパティ、**applicationGuardAllowVirtualGPU** プロパティを追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **enableAutomaticRedeployment** プロパティと **authenticationAllowFIDODevice** プロパティを追加しました|
|変更|ベータ版|[windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) エンティティに **trustedNetworkDomains** プロパティを追加しました|
|変更|ベータ版|[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta) エンティティに **minimumUpdateAutoInstallClassification** プロパティを追加しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **androidForWorkEnrollmentProfiles** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta) 複合型に **healthAttestationSupportedStatus** プロパティを追加しました|
|変更|ベータ版|[hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta) 複合型に **tpmSpecificationVersion** プロパティ、**operatingSystemEdition** プロパティ、**deviceFullQualifiedDomainName** プロパティ、**deviceGuardVirtualizationBasedSecurityHardwareRequirementState** プロパティ、**deviceGuardVirtualizationBasedSecurityState** プロパティ、**deviceGuardLocalSystemAuthorityCredentialGuardState** プロパティを追加しました|
|変更|ベータ版|[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta) 複合型に **vpnConfigurationId** プロパティを追加しました|
|変更|ベータ版|[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-beta) 複合型に **resourceActions** プロパティを追加しました|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | v1.0    | 以下の API を追加しました。<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-1.0)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-1.0)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-1.0)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-1.0)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-1.0)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-1.0)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-1.0)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-1.0)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-1.0)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-1.0)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-1.0)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-1.0)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-1.0)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-1.0)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-1.0)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-1.0)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-1.0)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-1.0)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-1.0)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-1.0)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-1.0)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-1.0)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-1.0)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-1.0)|
| 追加    | ベータ版    | 以下の API を追加しました。<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-beta)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-beta) |

## <a name="november-2017"></a>2017 年 11 月

### <a name="azure-ad-synchronization-apis"></a>Azure AD 同期 API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 次のリソースを含む、Azure AD ID 同期のサポートが追加されました。<br/>[Job](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)<br/>[Schema](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)<br/>[Template](/graph/api/resources/synchronization-synchronizationtemplate?view=graph-rest-beta)<br/>使用可能なメソッドの詳細については、リソースのトピックを参照してください。|

### <a name="education-apis"></a>教育機関 API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|次のリソースを含む、教育機関向けのシナリオのサポートが追加されました。<br/>[Schools](/graph/api/resources/educationschool?view=graph-rest-beta)<br/>[Classes](/graph/api/resources/educationclass?view=graph-rest-beta)<br/>[Users](/graph/api/resources/educationuser?view=graph-rest-beta)<br/>[Assignments](/graph/api/resources/educationassignment?view=graph-rest-beta)<br/>[Submissions](/graph/api/resources/educationsubmission?view=graph-rest-beta)<br/>使用可能なメソッドの詳細については、リソースのトピックを参照してください。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta)<br/>[deviceSetupConfiguration](/graph/api/resources/intune-deviceconfig-devicesetupconfiguration?view=graph-rest-beta)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-beta)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-beta)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)<br/>[ndesConnector](/graph/api/resources/intune-deviceconfig-ndesconnector?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)<br/>[auditProperty](/graph/api/resources/intune-auditing-auditproperty?view=graph-rest-beta)<br/>[auditResource](/graph/api/resources/intune-auditing-auditresource?view=graph-rest-beta)<br/>[bulkManagedDeviceActionResult](/graph/api/resources/intune-devices-bulkmanageddeviceactionresult?view=graph-rest-beta)<br/>[deviceProtectionOverview](/graph/api/resources/intune-devices-deviceprotectionoverview?view=graph-rest-beta)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>[operatingSystemVersionRange](/graph/api/resources/intune-deviceconfig-operatingsystemversionrange?view=graph-rest-beta)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-beta)<br/>|
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) コレクションに executeAction アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) に [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) に setDefaultProfile アクションを追加しました |
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) に ShareForSchoolDataSyncService アクションを追加しました |
|追加|ベータ版|[depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) に unshareForSchoolDataSyncService アクションを追加しました |
|追加|ベータ版|[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) コレクションに getAuditCategories 関数を追加しました |
|追加|ベータ版|[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) コレクションに getAuditActivityType 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**mobileAppIdentifierDeployment**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**windowsInformationProtectionCloudResource**<br/>**windowsInformationProtectionCloudResourceCollection**<br/>|
|変更|ベータ版|[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta) エンティティで次のプロパティを変更しました。<br/>**passcode** を必須から省略可能に変更しました<br/>|
|変更|ベータ版|[deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **microsoftStoreForBusinessLastSuccessfulSyncDateTime** プロパティ、**isEnabledForMicrosoftStoreForBusiness** プロパティ、**microsoftStoreForBusinessLanguage** プロパティ、**microsoftStoreForBusinessLastCompletedApplicationSyncTime** プロパティを追加しました|
|変更|ベータ版|[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta) エンティティに **target** プロパティを追加しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **deviceProtectionOverview** プロパティを追加しました|
|変更|ベータ版|[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) エンティティに **exchangeAlias** プロパティと **exchangeOrganization** プロパティを追加しました|
|変更|ベータ版|[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-beta) エンティティに **appStoreUrl** プロパティと **minimumSupportedOperatingSystem** プロパティを追加しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **remoteAssistanceSessionErrorString** プロパティを追加しました|
|変更|ベータ版|[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-beta) エンティティに **appStoreUrl** プロパティ、**applicableDeviceType** プロパティ、**minimumSupportedOperatingSystem** プロパティを追加しました|
|変更|ベータ版|[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta) エンティティに **notApplicableDeviceCount** プロパティ、**pendingInstallDeviceCount** プロパティ、**notApplicableUserCount** プロパティ、**pendingInstallUserCount** プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティから **targetedSecurityGroupIds** プロパティと **targetedSecurityGroupsCount** プロパティを削除しました|
|変更|ベータ版|[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) エンティティから **targetedSecurityGroupsCount** プロパティと **targetedSecurityGroupIds** プロパティを削除しました|
|変更|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティに **validOperatingSystemBuildRanges** プロパティを追加しました|
|変更|ベータ版|[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-beta) エンティティに **activeFirewallRequired** プロパティ、**uacRequired** プロパティ、**validOperatingSystemBuildRanges** プロパティを追加しました|
|変更|ベータ版|[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta) エンティティに **enableExpeditedTelemetryReporting** プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティから **allowedApps** プロパティ、**enterpriseCloudResources** プロパティ、**targetedSecurityGroupIds** プロパティを削除しました|
|変更|ベータ版|[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) エンティティに **ignoreVersionDetection** プロパティを追加しました|
|変更|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta) エンティティから **deviceConfiguration** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) エンティティに **deviceConfiguration** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) エンティティに **deviceSetupConfigurations** ナビゲーション プロパティ、**ndesConnectors** ナビゲーション プロパティ、**exchangeOnPremisesPolicies** ナビゲーション プロパティ、**conditionalAccessSettings** ナビゲーション プロパティ、**auditEvents** ナビゲーション プロパティ、**troubleshootingEvents** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **windowsProtectionState** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティおよび **targetedSecurityGroups** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) エンティティから **targetedSecurityGroups** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) エンティティに **deviceManagementTroubleshootingEvents** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティから **allowedAppLockerFiles** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[windowsManagedDevice](/graph/api/resources/intune-devices-windowsmanageddevice?view=graph-rest-beta) エンティティから **windowsProtectionState** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta) 複合型に **v11_0** プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta) 複合型に **denied** プロパティを追加しました|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 次の API に JSON サポートが追加されました。<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta) |

### <a name="webhooks"></a>Webhooks

| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 重大な変更 | ベータ版および v1.0 | ドライブ ルート項目の [webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) [サブスクリプション有効期限の最大長](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) の短縮。 新しい値はドライブ ルート項目用にサポートされている最大有効期限です。 |

## <a name="october-2017"></a>2017 年 10 月

### <a name="azure-ad-apis"></a>Azure AD API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
|追加|ベータ版|[identityProvider](/graph/api/resources/identityprovider?view=graph-rest-beta) エンティティと、[作成](/graph/api/identityprovider-post-identityproviders?view=graph-rest-beta)、[一覧表示](/graph/api/identityprovider-list?view=graph-rest-beta)、[取得](/graph/api/identityprovider-get?view=graph-rest-beta)、[更新](/graph/api/identityprovider-update?view=graph-rest-beta)、および[削除](/graph/api/identityprovider-delete?view=graph-rest-beta)操作を追加しました。|


### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfigurationAssignment](/graph/api/resources/intune-apps-ioslobappprovisioningconfigurationassignment?view=graph-rest-beta)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-beta)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-beta)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-beta)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-beta)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)<br/>[windows10PFXImportCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pfximportcertificateprofile?view=graph-rest-beta)<br/>[windowsAssignedAccessProfile](/graph/api/resources/intune-deviceconfig-windowsassignedaccessprofile?view=graph-rest-beta)<br/>[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)<br/>[iosSingleSignOnSettings](/graph/api/resources/intune-deviceconfig-iossinglesignonsettings?view=graph-rest-beta)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-beta)<br/>[proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-beta)<br/>[windowsStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-windowsstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>|
|追加|ベータ版|[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) に [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) に [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) に [assignedAccessMultiModeProfiles](/graph/api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) に [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) に [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) に [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) に [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-beta) アクションを追加しました |
|追加|ベータ版|[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) に [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) アクションを追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**cloudPkiSubscription**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|変更|ベータ版|[androidDeviceComplianceLocalActionBase](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionbase?view=graph-rest-beta) エンティティに **gracePeriodInMinutes** プロパティを追加しました|
|変更|ベータ版|[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta) エンティティから **enableSplitTunneling** プロパティを削除しました|
|変更|ベータ版|[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta) エンティティにプロパティ **versionName** および **versionCode** を追加しました|
|変更|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティにプロパティ **minimumRequiredPatchVersion** および **minimumWarningPatchVersion** を追加しました|
|変更|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティにプロパティ **minimumRequiredPatchVersion** および **minimumWarningPatchVersion** を追加しました|
|変更|ベータ版|[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta) エンティティに **target** プロパティを追加しました|
|変更|ベータ版|[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) エンティティに **singleSignOnSettings** プロパティを追加しました|
|変更|ベータ版|[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) エンティティにプロパティ **versionNumber** および **buildNumber** を追加しました|
|変更|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) エンティティに **bundleId** プロパティを追加しました|
|変更|ベータ版|[iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) エンティティに、プロパティ **preSharedKey** を追加しました|
|変更|ベータ版|[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) エンティティにプロパティ **versionName** および **versionCode** を追加しました|
|変更|ベータ版|[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) エンティティに **periodBeforePinReset** プロパティを追加しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティにプロパティ **subscriberCarrier**、**meid**、**totalStorageSpaceInBytes** および **freeStorageSpaceInBytes** を追加しました|
|変更|ベータ版|[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティから **enrollmentType** プロパティを削除しました|
|変更|ベータ版|[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) エンティティにプロパティ **versionNumber** および **buildNumber** を追加しました|
|変更|ベータ版|[mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティに **displayVersion** プロパティを追加しました|
|変更|ベータ版|[organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) エンティティから、プロパティ **defaultDeviceEnrollmentRestrictions**、**defaultDeviceEnrollmentWindowsHelloForBusinessSettings** および **defaultDeviceEnrollmentLimit** を削除しました|
|変更|ベータ版|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに **isAssigned** プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) エンティティに **isAssigned** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) エンティティにプロパティ **activeFirewallRequired**、**uacRequired**、**defenderEnabled**、**defenderVersion**、**signatureOutOfDate** および **rtpEnabled** を追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティにプロパティ **assignedAccessSingleModeUserName**、**assignedAccessSingleModeAppUserModelId**、**microsoftAccountSignInAssistantSettings**、**authenticationAllowSecondaryDevice**、**cryptographyAllowFipsAlgorithmPolicy**、**securityBlockAzureADJoinedDevicesAutoEncryption**、**systemTelemetryProxyServer**、**inkWorkspaceAccess**、**inkWorkspaceBlockSuggestedApps**、**defenderCloudBlockLevel** および **defenderCloudExtendedTimeout** を追加しました|
|変更|ベータ版|[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティにプロパティ **protectedApps**、**enterpriseProxiedDomains** および **isAssigned** を追加しました|
|変更|ベータ版|[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) エンティティに **productVersion** プロパティを追加しました|
|変更|ベータ版|[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **vppTokens** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta) エンティティから **deviceCompliancePolicy** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) エンティティに **deviceCompliancePolicy** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) エンティティに **identityCertificateForClientAuthentication** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **assignedAccessMultiModeProfiles** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティに **protectedAppLockerFiles** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta) 複合型にプロパティ **port** および **forceTls** を追加しました|
|変更|ベータ版|[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 複合型で次のプロパティの型を変更しました: <br/>**errorCode** を Int32 から Int64 に変更しました<br/>|
|変更|ベータ版|[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 複合型で次のプロパティの型を変更しました: <br/>**errorCode** を Int32 から Int64 に変更しました<br/>|
|変更|ベータ版|[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta) 複合型で次のプロパティの型を変更しました: <br/>**enterpriseCloudResources** を [windowsNetworkIsolationCloudResourceCollection](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationcloudresourcecollection?view=graph-rest-beta) から [proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta) コレクションに変更しました<br/>**enterpriseInternalProxyServers** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>**enterpriseIPRanges** を windowsNetworkIsolationIPRangeCollection から [ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta) コレクションに変更しました<br/>**enterpriseNetworkDomainNames** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>**enterpriseProxyServers** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>**neutralDomainResources** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新たに [team](/graph/api/resources/team?view=graph-rest-beta) エンティティを追加しました。|
|追加|ベータ版|[team](/graph/api/resources/team?view=graph-rest-beta) エンティティに [create](/graph/api/team-put-teams?view=graph-rest-beta)、[get](/graph/api/team-get?view=graph-rest-beta)、[update](/graph/api/team-update?view=graph-rest-beta) 操作を追加しました。|

### <a name="outlook-messages"></a>Outlook メッセージ

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | この動作の機能強化は、ユーザーがサインインしているユーザーとメール フォルダーを共有しているとき、またはサインインしているユーザーにユーザーのメールボックスを委任しているときに、共有のメール フォルダーやメッセージ コンテンツを取得することに関するものです。 このような状況で、アプリは、サインインしているユーザーが委任されたアクセス許可を提供している間、ユーザーの ID またはユーザー プリンシパル名を指定して、[その共有メール フォルダーを取得する](/graph/api/mailfolder-get?view=graph-rest-1.0)ことや、[その共有予定表のメッセージを取得する](/graph/api/user-list-messages?view=graph-rest-1.0)ことができます。 |


### <a name="outlook-user-choices"></a>Outlook のユーザーの選択

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
|追加 | ベータ版 | [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) に新しい **workingHours** プロパティを追加しました。 サポートされるユース ケースについては、「[workingHours リソース タイプ](/graph/api/resources/workinghours?view=graph-rest-beta)」を参照してください。|
|追加 | ベータ版 | 次の新しい複合型を追加しました。 <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-beta) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-beta) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-beta) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-beta)|


### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 変更      | ベータ版    | [getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)、[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)、および [getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) API を追加しました。 EmailActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)、[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)、[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)、および [getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta) API を追加しました。 EmailAppUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)、[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)、[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)、および [getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta) API を追加しました。 MailboxUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)、[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)、および [getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta) API を追加しました。 Office365Activations API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)、[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)、および [getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta) API を追加しました。 Office365ActiveUser API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)、[getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)、[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)、[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)、および [getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta) API を追加しました。 Office365GroupsActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)、[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)、および [getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta) API を追加しました。 OneDriveActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)、[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta), [getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)、および [getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta) API を追加しました。 OneDriveUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)、[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)、[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)、および [getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta) API を追加しました。 SharePointActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)、[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)、[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)、[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)、および [getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta) API を追加しました。 SharePointSiteUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)、[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)、および [getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta) API を追加しました。 SfbActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)、[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)、および [getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta) API を追加しました。 SfbDeviceUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)、[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)、および [getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta) API を追加しました。 SfbOrganizerActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)、[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)、および [getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta) API を追加しました。 SfbParticipantActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)、[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)、および [getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta) API を追加しました。 SfbP2PActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta)、[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta)、および [getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta) API を追加しました。 YammerActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta)、[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta)、および [getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta) API を追加しました。 YammerDeviceUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta)、[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta)、および [getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta) API を追加しました。 YammerGroupsActivity API は、これらにより置き換えられました。 |



## <a name="september-2017"></a>2017 年 9 月

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[azureADWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)<br/>[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)<br/>[windows10NetworkBoundaryConfiguration](/graph/api/resources/intune-deviceconfig-windows10networkboundaryconfiguration?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-beta)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-beta)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-beta)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-beta)<br/>[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-beta)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta)<br/>windowsNetworkIsolationResourceCollection<br/> |
| 追加    | ベータ版    | [windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta) に [sync](/graph/api/intune-enrollment-windowsautopilotsettings-sync?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) に [assign](/graph/api/intune-enrollment-windowsautopilotdeploymentprofile-assign?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) に localActions アクションを追加しました |
| 追加    | ベータ版    | [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) に [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) コレクションに uploadDepToken アクションを追加しました |
| 追加    | ベータ版    | [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) コレクションに syncWithAppleDeviceEnrollmentProgram アクションを追加しました |
| 追加    | ベータ版    | [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) に updateMobileAppIdentifierDeployments アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) に assign アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) に assign アクションを追加しました |
| 追加    | ベータ版    | [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) に assign アクションを追加しました |
| 追加    | ベータ版    | [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) コレクションに getEncryptionPublicKey 関数を追加しました |
| 変更      | ベータ版    | [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティに、プロパティ **requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity**、**conditionStatementId** を追加しました |
| 変更      | ベータ版    | [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) エンティティに、プロパティ **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** を追加しました |
| 変更      | ベータ版    | [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、プロパティ **blockCrossProfileCopyPaste** と **requireAppVerify** を追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、プロパティ **kioskModeApps** と **requireAppVerify** を追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから、プロパティ **kioskModeManagedApps** を削除しました |
| 変更      | ベータ版    | cloudPkiSubscription エンティティから、プロパティ **cloudPkiProvider**、**createdDateTime**、**description**、**lastModifiedDateTime**、**displayName**、**syncStatus**、**lastSyncError**、**lastSyncDateTime**、**credentials**、**trustedRootCertificate**、**version** を削除しました |
| 変更      | ベータ版    | [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティから、プロパティ **assignmentStatus**、**assignmentProgress**、**assignmentErrorMessage** を削除しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、**adminConsent** プロパティを追加しました |
| 変更      | ベータ版    | [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) エンティティに、プロパティ **vppTokenOrganizationName**、**vppTokenAccountType**、**vppTokenAppleId** を追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、プロパティ **deviceEnrollmentType**、**wiFiMacAddress**、**deviceHealthAttestationState** を追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティに、プロパティ **legacyAppConfiguration** を追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta) エンティティに、プロパティ **notApplicableCount** を追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta) エンティティに、プロパティ **notApplicableCount** を追加しました |
| 変更      | ベータ版    | [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに、プロパティ **firewallBlockStatefulFTP**、**firewallIdleTimeoutForSecurityAssociationInSeconds**、**firewallPreSharedKeyEncodingMethod**、**firewallIPSecExemptionsAllowNeighborDiscovery**、**firewallIPSecExemptionsAllowICMP**、**firewallIPSecExemptionsAllowRouterDiscovery**、**firewallIPSecExemptionsAllowDHCP**、**firewallCertificateRevocationListCheckMethod**、**firewallMergeKeyingModuleSettings**、**firewallPacketQueueingMethod**、**firewallProfileDomain**、**firewallProfilePublic**、**firewallProfilePrivate**、**defenderAttackSurfaceReductionExcludedPaths**、**defenderOfficeAppsOtherProcessInjectionType**、**defenderOfficeAppsExecutableContentCreationOrLaunchType**、**defenderOfficeAppsLaunchChildProcessType**、**defenderOfficeMacroCodeAllowWin32ImportsType**、**defenderScriptObfuscatedMacroCodeType**、**defenderScriptDownloadedPayloadExecutionType**、**defenderEmailContentExecutionType**、**defenderGuardMyFoldersType**、**defenderGuardedFoldersAllowedAppPaths**、**defenderAdditionalGuardedFolders**、**defenderNetworkProtectionType**、**defenderExploitProtectionXml**、**defenderExploitProtectionXmlFileName**、**defenderSecurityCenterBlockExploitProtectionOverride**、**appLockerApplicationControl**、**applicationGuardBlockClipboardSharing**、**applicationGuardAllowPrintToPDF**、**applicationGuardAllowPrintToXPS**、**applicationGuardAllowPrintToLocalPrinters**、**applicationGuardAllowPrintToNetworkPrinters**、**bitLockerDisableWarningForOtherDiskEncryption** を追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、プロパティ **displayAppListWithGdiDPIScalingTurnedOn**、**displayAppListWithGdiDPIScalingTurnedOff**、**messagingBlockSync**、**messagingBlockMMS**、**messagingBlockRichCommunicationServices** を追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティから、プロパティ **bluetoothDeviceName** を削除しました |
| 変更      | ベータ版    | [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) エンティティから、プロパティ **deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation**、**deviceAccountSessionInitiationProtocolAddress** を削除しました |
| 変更      | ベータ版    | [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **localActions** を追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **windowsAutopilotSettings**、**windowsAutopilotDeviceIdentities**、**windowsAutopilotDeploymentProfiles**、**deviceEnrollmentConfigurations**、**deviceManagementPartners**、**depOnboardingSettings** を追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティから、ナビゲーション プロパティ **cloudPkiSubscriptions** を削除しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **assignments** を追加しました |
| 変更      | ベータ版    | [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **assignments** を追加しました |
| 変更      | ベータ版    | [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **assignments** を追加しました |

### <a name="onedrive"></a>OneDrive

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [Drive][] リソースに、プロパティ **system** を追加しました。 |
| 追加        | v1.0        | [Drive][] リソースに、リレーションシップ **list** を追加しました。 |
| 追加        | v1.0        | [DriveItem][] リソースに、リレーションシップ **listItem** を追加しました。 |
| 追加        | v1.0        | [SharedDriveItem][] リソースに、リレーションシップ **list** と **listItem** を追加しました。 |
| 追加        | v1.0        | 新しい複合型を追加しました。[FolderView][]  |
| 追加        | v1.0        | [Folder][] 複合型に、プロパティ **view** を追加しました。 |
| 追加        | v1.0        | [ItemReference][] 複合型に、プロパティ **driveType**を追加しました。 |
| 追加        | v1.0        | [Video][] 複合型に、プロパティ **audioBitsPerSample**、**audioChannels**、**audioFormat**、**audioSamplesPerSecond**、**fourCC**、**frameRate** を追加しました。 |
| 追加        | ベータ版        | [Drive][Drive-beta] リソースに、プロパティ **system** を追加しました。 |
| 追加        | ベータ版        | [Drive][Drive-beta] リソースに、リレーションシップ **activities** を追加しました。 |
| 追加        | ベータ版        | [DriveItem][DriveItem-beta] リソースに、プロパティ **publication** を追加しました。 |
| 追加        | ベータ版        | [DriveItem][DriveItem-beta] リソースに、リレーションシップ **activities** と **versions** を追加しました。 |
| 追加        | ベータ版        | 新しいエンティティを追加しました。[DriveItemVersion][DriveItemVersion-beta]、[ItemActivity][ItemActivity-beta]。 |
| 追加        | ベータ版        | 新しい複合型を追加しました。[CommentAction][CommentAction-beta]、[CreateAction][CreateAction-beta]、[DeleteAction][DeleteAction-beta]、[EditAction][EditAction-beta]、[ItemActionSet][ItemActionSet-beta]、[ItemActivityTimeSet][ItemActivityTimeSet-beta]、[MentionAction][MentionAction-beta]、[MoveAction][MoveAction-beta]、[PublicationFacet][PublicationFacet-beta]、[RenameAction][RenameAction-beta]、[RestoreAction][RestoreAction-beta]、[ShareAction][ShareAction-beta]、[VersionAction][VersionAction-beta]。 |
| 追加        | ベータ版        | [ItemReference][ItemReference-beta] 複合型に、プロパティ **driveType** を追加しました。 |
| 削除        | ベータ版        | [SharepointIds][SharepointIds-beta] 複合型から、プロパティ **tenantId** を削除しました。 |
| 追加        | v1.0        | [Video][Video-beta] 複合型に、プロパティ **audioBitsPerSample**、**audioChannels**、**audioFormat**、**audioSamplesPerSecond**、**fourCC**、**frameRate** を追加しました。 |
| 追加        | ベータ版        | [DriveItem][DriveItem-beta] リソースに、アクション [CheckIn][CheckIn-beta] と [CheckOut][CheckOut-beta] を追加しました。 |
| 追加        | ベータ版        | [DriveItem][DriveItem-beta] リソースのアクション [CreateLink][CreateLink-beta] に、プロパティ **expirationDateTime**、**password**、**message**、**recipients** を追加しました。 |

[Drive]: /graph/api/resources/drive?view=graph-rest-1.0
[DriveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[SharedDriveItem]: /graph/api/resources/shareddriveitem?view=graph-rest-1.0
[FolderView]: /graph/api/resources/folderview?view=graph-rest-1.0
[Folder]: /graph/api/resources/folder?view=graph-rest-1.0
[ItemReference]: /graph/api/resources/itemreference?view=graph-rest-1.0
[Video]: /graph/api/resources/video?view=graph-rest-1.0
[Drive-beta]: /graph/api/resources/drive?view=graph-rest-beta
[DriveItem-beta]: /graph/api/resources/driveitem?view=graph-rest-beta
[DriveItemVersion-beta]: /graph/api/resources/driveitemversion?view=graph-rest-beta
[ItemActivity-beta]: /graph/api/resources/itemactivity?view=graph-rest-beta
[CommentAction-beta]: /graph/api/resources/commentaction?view=graph-rest-beta
[CreateAction-beta]: /graph/api/resources/createaction?view=graph-rest-beta
[DeleteAction-beta]: /graph/api/resources/deleteaction?view=graph-rest-beta
[EditAction-beta]: /graph/api/resources/editaction?view=graph-rest-beta
[ItemActionSet-beta]: /graph/api/resources/itemactionset?view=graph-rest-beta
[ItemActivityTimeSet-beta]: /graph/api/resources/itemactivitytimeset?view=graph-rest-beta
[MentionAction-beta]: /graph/api/resources/mentionaction?view=graph-rest-beta
[MoveAction-beta]: /graph/api/resources/moveaction?view=graph-rest-beta
[PublicationFacet-beta]: /graph/api/resources/publicationfacet?view=graph-rest-beta
[RenameAction-beta]: /graph/api/resources/renameaction?view=graph-rest-beta
[RestoreAction-beta]: /graph/api/resources/restoreaction?view=graph-rest-beta
[ShareAction-beta]: /graph/api/resources/shareaction?view=graph-rest-beta
[VersionAction-beta]: /graph/api/resources/versionaction?view=graph-rest-beta
[ItemReference-beta]: /graph/api/resources/itemreference?view=graph-rest-beta
[SharepointIds-beta]: /graph/api/resources/sharepointids?view=graph-rest-beta
[Video-beta]: /graph/api/resources/video?view=graph-rest-beta
[CheckIn-beta]: /graph/api/driveitem-checkin?view=graph-rest-beta
[CheckOut-beta]: /graph/api/driveitem-checkout?view=graph-rest-beta
[CreateLink-beta]: /graph/api/driveitem-createlink?view=graph-rest-beta


### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [user](/graph/api/resources/user?view=graph-rest-beta) エンティティに、関数 [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) と [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) を追加しました。 |
| 追加        | ベータ版          | **locations** プロパティが [event](/graph/api/resources/event?view=graph-rest-beta) エンティティに追加され、出席者が複数の場所から出席できるイベントを編成できるようになりました。 |
| 追加        | ベータ版          | **locationType** プロパティが [location](/graph/api/resources/location?view=graph-rest-beta) 複合型に追加されました。 |
| 追加        | ベータ版          | **uniqueId** および **uniqueIdType** プロパティが [location](/graph/api/resources/location?view=graph-rest-beta) 複合型に追加されました。 これらのプロパティは、現時点では内部使用に限られます。 |
| 変更          | v1.0 およびベータ版 | この動作の機能強化は、ユーザーがサインインしているユーザーと予定表を共有しているとき、またはサインインしているユーザーにユーザーのメールボックスを委任しているときに、共有の予定表やイベント コンテンツを取得することに関するものです。 このような状況で、アプリは、サインインしているユーザーが委任されたアクセス許可を提供している間、ユーザーの ID またはユーザー プリンシパル名を指定して、[その共有予定表を取得する](/graph/api/calendar-get?view=graph-rest-1.0)ことや、[その共有予定表のイベントを取得する](/graph/api/user-list-events?view=graph-rest-1.0)ことができます。 |

### <a name="outlook-contacts"></a>Outlook の連絡先

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | この動作の機能強化は、ユーザーがサインインしているユーザーと連絡先フォルダーを共有しているとき、またはサインインしているユーザーにユーザーのメールボックスを委任しているときに、共有の連絡先フォルダーや連絡先コンテンツを取得することに関するものです。 このような状況で、アプリは、サインインしているユーザーが委任されたアクセス許可を提供している間、ユーザーの ID またはユーザー プリンシパル名を指定して、[その共有連絡先フォルダーを取得する](/graph/api/contactfolder-get?view=graph-rest-1.0)ことや、[その共有フォルダーの連絡先を取得する](/graph/api/user-list-contacts?view=graph-rest-1.0)ことができます。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [message](/graph/api/resources/message?view=graph-rest-beta) エンティティに、プロパティ **internetMessageHeaders** を追加しました。 |
| 追加        | ベータ版        | [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-beta) 複合型を追加しました。 |
| 追加        | ベータ版        | [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **messageRules** を追加しました。 **messageRules** は [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) インスタンスのコレクションです。 |
| 追加        | ベータ版        | [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) エンティティと、[messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-beta)、[messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-beta)、[sizeRange](/graph/api/resources/sizerange?view=graph-rest-beta) 複合型が追加されました。 |
| 追加        | ベータ版        | メッセージ ルールに次の CRUD 操作が追加されました: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-beta)、[list](/graph/api/mailfolder-list-messagerules?view=graph-rest-beta)、[get](/graph/api/messagerule-get?view=graph-rest-beta)、[update](/graph/api/messagerule-update?view=graph-rest-beta)、[delete](/graph/api/messagerule-delete?view=graph-rest-beta)。 |


### <a name="outlook-user-choices"></a>Outlook のユーザーの選択

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) エンティティに、新しい **masterCategories** ナビゲーション プロパティを追加しました。 **masterCategories** は [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) オブジェクトのコレクションです。 |
| 追加        | ベータ版        | [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) エンティティを追加しました。 |
| 追加        | ベータ版        | [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) に次の CRUD 操作を追加しました: [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-beta)、[get](/graph/api/outlookcategory-get?view=graph-rest-beta)、[update](/graph/api/outlookcategory-update?view=graph-rest-beta)、[delete](/graph/api/outlookcategory-delete?view=graph-rest-beta)。 |
| 追加        | ベータ版        | 新しい [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-beta) 関数が [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) エンティティに追加されました。 |
| 追加        | ベータ版        | [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta) エンティティに、新しい [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-beta) 関数を追加しました。 |


### <a name="sharepoint-lists"></a>SharePoint リスト

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しいエンティティを追加しました。[ColumnDefinition][]、[ColumnLink][]、[ContentType][]、[List][]、[ListItem][]。 |
| 追加        | v1.0        | [Site][] リソースに、リレーションシップ **columns**、**contentTypes**、**items**、**lists** を追加しました。 |
| 追加        | v1.0        | 新しい複合型を追加しました。[BooleanColumn][]、[CalculatedColumn][]、[ChoiceColumn][]、[ContentTypeInfo][]、[ContentTypeOrder][]、[CurrencyColumn][]、[DateTimeColumn][]、[DefaultColumnValue][]、[ListInfo][]、[LookupColumn][]、[NumberColumn][]、[PersonOrGroupColumn][]、[SystemFacet][]、[TextColumn][]。 |
| 追加        | ベータ版        | 新しいエンティティを追加しました。[BaseItemVersion][BaseItemVersion-beta]、[ColumnLink][ColumnLink-beta]、[ContentType][ContentType-beta]、[ListItemVersion][ListItemVersion-beta]、 |
| 追加        | ベータ版        | [ColumnDefinition][ColumnDefinition-beta] に、プロパティ **columnGroup**、**currency**、**defaultValue**、**displayName** を追加しました。 |
| 追加        | ベータ版        | [List][List-beta] リソースに、プロパティ **displayName** と **system** を追加しました。 |
| 追加        | ベータ版        | [List][List-beta] リソースに、リレーションシップ **activities** と **contentTypes** を追加しました。 |
| 追加        | ベータ版        | [ListItem][ListItem-beta] リソースに、プロパティ **contentType** を追加しました。 |
| 追加        | ベータ版        | [ListItem][ListItem-beta] リソースに、リレーションシップ **activities** と **versions** を追加しました。 |
| 追加        | ベータ版        | [Site][Site-beta] リソースに、リレーションシップ **contentTypes** を追加しました。 |
| 追加        | ベータ版        | [BooleanColumn][BooleanColumn-beta] 型に、プロパティ **outputType** を追加しました。 |
| 追加        | ベータ版        | 新しい複合型を追加しました。[ContentTypeInfo][ContentTypeInfo-beta]、[ContentTypeOrder][ContentTypeOrder-beta]、[CurrencyColumn][CurrencyColumn-beta]、[SystemFacet][SystemFacet-beta]。 |
| 追加        | ベータ版        | [ListInfo][ListInfo-beta] 複合型に、プロパティ **contentTypesEnabled** を追加しました。 |
| 追加        | ベータ版        | [LookupColumn][LookupColumn-beta] 複合型に、プロパティ **allowUnlimitedLength** を追加しました。 |
| 変更          | ベータ版        | [LookupColumn][LookupColumn-beta] 複合型のプロパティ **allowMultipleValue** の名前を **allowMultipleValues** に変更しました。 |
| 変更          | ベータ版        | [PersonOrGroupColumn][PersonOrGroupColumn-beta] 複合型のプロパティ **chooseFrom** の名前を **chooseFromType** に変更しました。 |
| 削除        | ベータ版        | [NumberColumn][NumberColumn-beta] 複合型から、プロパティ **locale** を削除しました。 |
| 削除        | ベータ版        | [PersonOrGroupColumn][PersonOrGroupColumn-beta] 複合型から、プロパティ **enforceUniqueValues** を削除しました。 |

[BaseItemVersion-beta]: /graph/api/resources/baseitemversion?view=graph-rest-beta
[BooleanColumn-beta]:  /graph/api/resources/booleanColumn?view=graph-rest-beta
[BooleanColumn]: /graph/api/resources/booleancolumn?view=graph-rest-1.0
[CalculatedColumn]: /graph/api/resources/calculatedcolumn?view=graph-rest-1.0
[ChoiceColumn]: /graph/api/resources/choicecolumn?view=graph-rest-1.0
[ColumnDefinition-beta]: /graph/api/resources/columndefinition?view=graph-rest-beta
[ColumnDefinition]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[ColumnLink-beta]: /graph/api/resources/columnlink?view=graph-rest-beta
[ColumnLink]: /graph/api/resources/columnlink?view=graph-rest-1.0
[ContentType-beta]: /graph/api/resources/contenttype?view=graph-rest-beta
[ContentType]: /graph/api/resources/contenttype?view=graph-rest-1.0
[ContentTypeInfo-beta]: /graph/api/resources/contenttypeinfo?view=graph-rest-beta
[ContentTypeInfo]: /graph/api/resources/contenttypeinfo?view=graph-rest-1.0
[ContentTypeOrder-beta]: /graph/api/resources/contenttypeorder?view=graph-rest-beta
[ContentTypeOrder]: /graph/api/resources/contenttypeorder?view=graph-rest-1.0
[CurrencyColumn-beta]: /graph/api/resources/currencycolumn?view=graph-rest-beta
[CurrencyColumn]: /graph/api/resources/currencycolumn?view=graph-rest-1.0
[DateTimeColumn]: /graph/api/resources/datetimecolumn?view=graph-rest-1.0
[DefaultColumnValue]: /graph/api/resources/defaultcolumnvalue?view=graph-rest-1.0
[List-beta]: /graph/api/resources/list?view=graph-rest-beta
[List]: /graph/api/resources/list?view=graph-rest-1.0
[ListInfo-beta]: /graph/api/resources/listinfo?view=graph-rest-beta
[ListInfo]: /graph/api/resources/listinfo?view=graph-rest-1.0
[ListItem-beta]: /graph/api/resources/listitem?view=graph-rest-beta
[ListItem]: /graph/api/resources/listitem?view=graph-rest-1.0
[ListItemVersion-beta]: /graph/api/resources/listitemversion?view=graph-rest-beta
[LookupColumn-beta]: /graph/api/resources/lookupcolumn?view=graph-rest-beta
[LookupColumn]: /graph/api/resources/lookupcolumn?view=graph-rest-1.0
[NumberColumn-beta]: /graph/api/resources/numbercolumn?view=graph-rest-beta
[NumberColumn]: /graph/api/resources/numbercolumn?view=graph-rest-1.0
[PersonOrGroupColumn-beta]: /graph/api/resources/personorgroupcolumn?view=graph-rest-beta
[PersonOrGroupColumn]: /graph/api/resources/personorgroupcolumn?view=graph-rest-1.0
[Site-beta]: /graph/api/resources/site?view=graph-rest-beta
[Site]: /graph/api/resources/site?view=graph-rest-1.0
[SystemFacet-beta]: /graph/api/resources/systemfacet?view=graph-rest-beta
[SystemFacet]: /graph/api/resources/systemfacet?view=graph-rest-1.0
[TextColumn]: /graph/api/resources/textcolumn?view=graph-rest-1.0


### <a name="sharepoint-sites"></a>SharePoint サイト

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [SiteCollection][SiteCollection-beta] 複合型に、プロパティ **dataLocationCode** と **root** を追加しました。 |

[SiteCollection-beta]: /graph/api/resources/sitecollection?view=graph-rest-beta


## <a name="august-2017"></a>2017 年 8 月

### <a name="group-lifecycle-policy"></a>グループのライフサイクル ポリシー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-beta) エンティティを追加しました。 |
| 追加        | ベータ版        | グループのライフサイクル ポリシーに、次の API を追加しました。[create](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-beta)、[list](/graph/api/grouplifecyclepolicy-list?view=graph-rest-beta)、[get](/graph/api/grouplifecyclepolicy-get?view=graph-rest-beta)、[update](/graph/api/grouplifecyclepolicy-update?view=graph-rest-beta)、[delete](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-beta)、[add group](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-beta)、[remove group](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-beta)、および [renew a group](/graph/api/grouplifecyclepolicy-renewgroup?view=graph-rest-beta)。 |
| 追加        | ベータ版        | [group](/graph/api/resources/group?view=graph-rest-beta) エンティティに [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-beta) 関数を追加しました。 |

### <a name="intune-apis"></a>Intune API
| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 追加された新しいエンティティ:<br/>[windowsPrivacyDataAccessControlItem](/graph/api/resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | 追加された新しい複合型:<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) に [windowsPrivacyAccessControls](/graph/api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols?view=graph-rest-beta) アクションを追加しました |
| 変更      | ベータ版    | [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) エンティティに **automaticallyUpdateApps** および **countryOrRegion** プロパティを追加しました |
| 変更      | ベータ版    | [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) エンティティに **enableAuthenticationViaCompanyPortal** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) エンティティに **notificationMessageCCList** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **configurationManagerClientEnabledFeatures** プロパティを追加しました |
| 変更      | ベータ版    | [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) エンティティから **intuneBrand** プロパティを削除しました |
| 変更      | ベータ版    | [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに **smartScreenEnableInShell**、**smartScreenBlockOverrideForFiles**、**applicationGuardEnabled**、**applicationGuardBlockFileTransfer**、**applicationGuardBlockNonEnterpriseContent**、**applicationGuardAllowPersistence**、および **applicationGuardForceAuditing** プロパティを追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **searchBlockDiacritics**、**searchDisableAutoLanguageDetection**、**searchDisableIndexingEncryptedItems**、**searchEnableRemoteQueries**、**searchDisableUseLocation**、**searchDisableIndexerBackoff**、**searchDisableIndexingRemovableDrive**、**searchEnableAutomaticIndexSizeManangement**、**smartScreenEnableAppInstallControl**、および **privacyAdvertisingId** プロパティを追加しました |
| 変更      | ベータ版    | [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) エンティティから **settingsDeviceName** プロパティを削除しました |
| 変更      | ベータ版    | [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティから **restartMode** プロパティを削除しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **detectedApps** および **managedDevices** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに **privacyAccessControls** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型に **secureByDefault** プロパティを追加しました |
| 変更      | ベータ版    | [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) 複合型に **restartMode** プロパティを追加しました |

### <a name="onenote"></a>OneNote

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | [onenote](/graph/api/resources/onenote?view=graph-rest-1.0) ナビゲーション プロパティを **site** に追加しました。 |
| 追加        | ベータ版          | コピー操作用にターゲット *siteCollectionId* とターゲット *siteId* パラメーターを追加しました。次に例を示します。[CopyNotebook](/graph/api/notebook-copynotebook?view=graph-rest-1.0)。 |

### <a name="people"></a>複数のユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | v1.0 に [People API](/graph/api/resources/person?view=graph-rest-1.0) を追加しました。People API の詳細については、「[People の関連情報を取得する](people-example.md)」を参照してください。 |
| 追加        | v1.0        | People.Read.All アクセス許可を追加しました。 詳細については、「[アクセス許可](permissions-reference.md)」を参照してください。 |
| 追加        | v1.0        | [personType](/graph/api/resources/persontype?view=graph-rest-1.0) リソースを追加しました。 |
| 変更          | v1.0        | [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) リソースが **rankedEmailAddress** リソースに取って代わりました。 |
| 変更          | v1.0        | [person](/graph/api/resources/person?view=graph-rest-1.0) リソースは次のように更新されました。<ul><li>**scoredEmailAddresses** プロパティ ([scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) 型のコレクション) が **emailAddresses** プロパティに取って代わりました</li><li>**jobTitle** プロパティが **title** プロパティに取って代わりました</li><li>**sources** プロパティと **mailboxType** プロパティが削除されました</li><li>**personType** プロパティは現在、文字列型ではなく [personType](/graph/api/resources/persontype?view=graph-rest-1.0) 型であり、以前の **sources** プロパティと **mailboxType** プロパティの機能に取って代わりました</li><li>**imAddress** プロパティを追加しました</li></ul> |
| 削除        | v1.0        | **personDataSource** リソースが削除されました。 |

### <a name="user"></a>ユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | **employeeId** プロパティを [user](/graph/api/resources/user?view=graph-rest-beta) に追加しました。 |

## <a name="july-2017"></a>2017 年 7 月

### <a name="group-settings"></a>グループ設定

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | グループ設定のサポートを追加しました。<br/>新しいリソースの種類: [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0)、[groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0)、[settingValue](/graph/api/resources/settingvalue?view=graph-rest-1.0)、および [settingTemplateValue](/graph/api/resources/settingtemplatevalue?view=graph-rest-1.0) |
| 変更          | v1.0        | プロパティ **classification** とナビゲーション プロパティ **settings** を [group](/graph/api/resources/group?view=graph-rest-1.0) に追加しました |

### <a name="intune-apis"></a>Intune API

| 変更の種類&nbsp; | バージョン | 説明                              |
| :--------------- | :------ | :--------------------------------------- |
| 追加         | ベータ版    | [assign](/graph/api/intune-apps-iosmobileappconfiguration-assign?view=graph-rest-beta) アクションを [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) に追加しました |
| 追加         | ベータ版    | [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-beta) アクションを [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に追加しました |
| 変更           | ベータ版    | **appsInstallAllowList**、**appsLaunchBlockList**、**appsHideList** プロパティを [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **disableAppEncryptionIfDeviceEncryptionIsEnabled** プロパティを [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **disableAppEncryptionIfDeviceEncryptionIsEnabled** プロパティを [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **subscriptions** プロパティを [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **version** プロパティを [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **utcTimeOffsetInMinutes** プロパティを [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **preSharedKey** プロパティを [macOSWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macoswificonfiguration?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **phoneNumber**、**androidSecurityPatchLevel**、**userDisplayName** プロパティを [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **userName**、**deviceModel**、**platform**、**complianceGracePeriodExpirationDateTime** プロパティを [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **userPrincipalName** プロパティを [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **overrideDefaultRule** プロパティを [onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **userPrincipalName** プロパティを [userAppInstallStatus](/graph/api/resources/intune-apps-userappinstallstatus?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **connectAppBlockAutoLaunch**、**deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation**、**deviceAccountSessionInitiationProtocolAddress**、**settingsBlockMyMeetingsAndFiles**、**settingsBlockSessionResume**、**settingsBlockSigninSuggestions**、**settingsDefaultVolume**、**settingsScreenTimeoutInMinutes**、**settingsSessionTimeoutInMinutes**、**settingsSleepTimeoutInMinutes** プロパティを [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **deploymentSummary** ナビゲーション プロパティを [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに追加しました |
| 変更           | ベータ版    | **settingName**、**userId**、**userName**、**userEmail**、**currentValue** プロパティを[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 複合型に追加しました |
| 変更           | ベータ版    | [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 複合型に、**settingName**、**userId**、**userName**、**userEmail**、**currentValue** の各プロパティを追加しました |
| 変更           | ベータ版    | **unknownCount** プロパティを[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta) 複合型に追加しました |



## <a name="june-2017"></a>2017 年 6 月

### <a name="project-rome"></a>Project Rome

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 以下のリソースと API が追加されています。<br/>[アクティビティ](/graph/api/resources/projectrome-activity?view=graph-rest-beta)<br/>[アクティビティを作成または置換する](/graph/api/projectrome-put-activity?view=graph-rest-beta)<br/>[アクティビティを削除する](/graph/api/projectrome-delete-activity?view=graph-rest-beta)<br/>[履歴項目](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta)<br/>[履歴項目を作成または置換する](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)<br/>[履歴項目を削除する](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) |

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) の 4 つのプロパティ **canEdit**、**canShare**、**canViewPrivateItems**、および **owner** を v1.0 に昇格しました。 |


### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[defaultDeviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-defaultdevicecompliancepolicy?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementScriptDeviceState](/graph/api/resources/intune-devicefe-devicemanagementscriptdevicestate?view=graph-rest-beta)<br/>[deviceManagementScriptRunSummary](/graph/api/resources/intune-devicefe-devicemanagementscriptrunsummary?view=graph-rest-beta)<br/>[deviceManagementScriptUserState](/graph/api/resources/intune-devicefe-devicemanagementscriptuserstate?view=graph-rest-beta)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta)<br/>[windowsManagedDevice](/graph/api/resources/intune-devicefe-windowsmanageddevice?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-devicefe-windowsmanagementapphealthstate?view=graph-rest-beta)<br/>[windowsManagementAppHealthSummary](/graph/api/resources/intune-devicefe-windowsmanagementapphealthsummary?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[bitLockerFixedDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerfixeddrivepolicy?view=graph-rest-beta)<br/>[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-beta)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devicefe-deleteuserfromsharedappledeviceactionresult?view=graph-rest-beta)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-beta)<br/> |
| 削除    | ベータ版    | 次のエンティティを削除しました。<br/>**deviceManagementScriptState**<br/> |
| 削除    | ベータ版    | [user](/graph/api/resources/intune-devicefe-user?view=graph-rest-beta) の wipeByDeviceTag アクションを削除しました。 |
| 変更      | ベータ版    | [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) エンティティに、プロパティ **innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap** および **outerIdentityPrivacyTemporaryValue** を追加しました |
| 変更      | ベータ版    | [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap** および **enableOuterIdentityPrivacy** を削除しました |
| 変更      | ベータ版    | [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [complianceSettingStateSummary](/graph/api/resources/compliancesettingstatesummary?view=graph-rest-beta) エンティティから、プロパティ **instanceDisplayName** および **settingPlatform** を削除しました |
| 変更      | ベータ版    | [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) エンティティに **excludeGroup** プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta) エンティティから、プロパティ **instanceDisplayName** および **settingPlatform** を削除しました |
| 変更      | ベータ版    | [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) エントリから、プロパティ **devicePlatform** を削除しました |
| 変更      | ベータ版    | [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティに、プロパティ **assignmentStatus**、**assignmentProgress** および **assignmentErrorMessage** を追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、プロパティ **intuneBrand** を追加しました |
| 変更      | ベータ版    | [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) エンティティに、プロパティ **enforceSignatureCheck** および **fileName** を追加しました |
| 変更      | ベータ版    | [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) エンティティに、プロパティ **innerAuthenticationProtocolForEapTtls** および **outerIdentityPrivacyTemporaryValue** を追加しました |
| 変更      | ベータ版    | [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls** および **enableOuterIdentityPrivacy** を削除しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、プロパティ **classroomAppForceUnpromptedScreenObservation**、**keyboardBlockDictation**、**networkUsageRules** および **wiFiConnectOnlyToConfiguredNetworks** を追加しました |
| 変更      | ベータ版    | [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) エンティティに、プロパティ **preSharedKey** を追加しました |
| 変更      | ベータ版    | [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) エンティティに、プロパティ **innerAuthenticationProtocolForEapTtls** および **outerIdentityPrivacyTemporaryValue** を追加しました |
| 変更      | ベータ版    | [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls** および **enableOuterIdentityPrivacy** を削除しました |
| 変更      | ベータ版    | [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) エンティティから、プロパティ **lastModifiedTime** および **deployedAppCount** を削除しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、プロパティ **serialNumber** を追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティから、プロパティ **managementAgents** を削除しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) エンティティに、プロパティ **bitLockerFixedDrivePolicy** および **bitLockerRemovableDrivePolicy** を追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、プロパティ **enterpriseCloudPrintDiscoveryEndPoint**、**enterpriseCloudPrintOAuthAuthority**、**enterpriseCloudPrintOAuthClientIdentifier**、**enterpriseCloudPrintResourceIdentifier**、**enterpriseCloudPrintDiscoveryMaxLimit**、**enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**、**edgeBlockAddressBarDropdown**、**edgeBlockCompatibilityList**、**edgeClearBrowsingDataOnExit**、**edgeAllowStartPagesModification**、**edgeDisableFirstRunPage**、**edgeBlockLiveTileDataCollection** および **edgeSyncFavoritesWithInternetExplorer** を追加しました |
| 変更      | ベータ版    | [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) エンティティに、プロパティ **availableVersion** を追加しました |
| 変更      | ベータ版    | [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) エンティティから、プロパティ **onboardingStatus**、**deployedVersion** および **lastModifiedTime** を削除しました |
| 変更      | ベータ版    | [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) エンティティに、プロパティ **packageIdentityName** を追加しました |
| 変更      | ベータ版    | [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を追加しました |
| 変更      | ベータ版    | [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** を追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **deviceConfigurationUserStateSummaries** および **iosUpdateStatuses** を追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティから、ナビゲーション プロパティ **complianceSettingStateSummaries** を削除しました |
| 変更      | ベータ版    | [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **runSummary**、**deviceRunStates** および **userRunStates** を追加しました |
| 変更      | ベータ版    | [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) エンティティから、ナビゲーション プロパティ **runStates** を削除しました |
| 変更      | ベータ版    | [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を追加しました |
| 変更      | ベータ版    | [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) エンティティから、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を削除しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を追加しました |
| 変更      | ベータ版    | [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) エンティティに、ナビゲーション プロパティ **healthSummary** および **healthStates** を追加しました |
| 変更      | ベータ版    | [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) 複合型に、プロパティ **applicationId**、**appName**、**platformId**、**userFailures** および **deviceFailures** を追加しました |
| 変更      | ベータ版    | [bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy) 複合型に、プロパティ **encryptionMethod**、**startupAuthenticationRequired**、**startupAuthenticationBlockWithoutTpmChip**、**startupAuthenticationTpmUsage**、**startupAuthenticationTpmPinUsage**、**startupAuthenticationTpmKeyUsage**、**startupAuthenticationTpmPinAndKeyUsage**、**recoveryOptions** および **prebootRecoveryEnableMessageAndUrl** を追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 複合型から、プロパティ **settingName**、**userId**、**userName**、**userEmail** および **currentValue** を削除しました |
| 変更      | ベータ版    | [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 複合型から、プロパティ **settingName**、**userId**、**userName**、**userEmail** および **currentValue** を削除しました |
| 変更      | ベータ版    | [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型に、プロパティ **windowsCommercialId** および **windowsCommercialIdLastModifiedTime** を追加しました |
| 変更      | ベータ版    | [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) 複合型に、プロパティ **address** を追加しました |


## <a name="may-2017"></a>2017 年 5 月

### <a name="application-api-changes"></a>アプリケーション API の変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | アプリケーション API の更新。これはプロパティの名前変更と[アプリケーション](/graph/api/resources/application?view=graph-rest-beta) エンティティの再構築を含む最初の変更のセットです。<br/>**新しいエンティティ:** [api](/graph/api/resources/api?view=graph-rest-beta])、[informationalUrl](/graph/api/resources/informationalurl?view=graph-rest-beta)、[installedClient](/graph/api/resources/installedclient?view=graph-rest-beta)[permissionScope](/graph/api/resources/permissionscope?view=graph-rest-beta)、[preauthorizedApplication](/graph/api/resources/preauthorizedapplication?view=graph-rest-beta)、[web](/graph/api/resources/web?view=graph-rest-beta)。<br/>**削除されたプロパティ:** addIns、appRoles、availableToOtherOrganizations、knownClientApplications、oauth2AllowUrlPathMatching、recordConsentConditions。<br/>**名前が変更されたプロパティ:** appId から id、identifierUris から applicationAliases、availableToOtherTenants から orgRestrictions、mainLogo から logo、oauth2Permissions から publishedPermissionsScopes、publicClient は allowPublicClient、replyUrls から redirectUrls。<br/>**新しいプロパティ:** タグ。 |

### <a name="remove-deprecated-planner-api"></a>使用されていない Planner API の削除
| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 削除        | ベータ版        | 次のエンティティを削除しました:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Project Rome

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | プロジェクト ローマのサポートを追加しました。これには、[デバイスのリストの取得](/graph/api/user-list-devices?view=graph-rest-beta)、[デバイスへのコマンドの送信](/graph/api/send-device-command?view=graph-rest-beta)、および[コマンドのステータスの確認](/graph/api/get-device-command-status?view=graph-rest-beta)が含まれます。 |
| 追加        | ベータ版        | ユーザーの [activities](/graph/api/resources/projectrome-activity?view=graph-rest-beta) と [historyItems](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) のサポートが追加され、これには[アクティビティの upsert](/graph/api/projectrome-put-activity?view=graph-rest-beta) と[履歴項目の upsert](/graph/api/projectrome-put-historyitem?view=graph-rest-beta) が含まれます。 |

### <a name="administrative-units-property-changes"></a>管理単位のプロパティの変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [scopedRoleMembership](/graph/api/resources/scopedrolemembership?view=graph-rest-beta) エンティティの roleMemberInfo プロパティ型を [ID](/graph/api/resources/identity?view=graph-rest-1.0) に変更しました |
| 変更          | ベータ版        | [user](/graph/api/resources/user?view=graph-rest-beta) エンティティのナビゲーション プロパティ scopedAdministratorOf を scopedRoleMemberOf に変更しました |
| 変更          | ベータ版        | [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) エンティティのナビゲーション プロパティ scopedAdministrators を scopedRoleMembers に変更しました |
| 変更          | ベータ版        | [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta) エンティティのナビゲーション プロパティ scopedAdministrators を scopedMembers に変更しました |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>プレビューでのユーザーとグループの Webhook サポートの追加

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:-----------|:--------------|
| 変更        | ベータ版       | ユーザーとグループの [Webhook](/graph/api/resources/webhooks?view=graph-rest-beta) に対するサポートを追加しました。

### <a name="add-delta-query-to-v10"></a>デルタ クエリの v1.0 への追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | v1.0 にデルタ関数のサポートを追加します。 [デルタ クエリ](delta-query-overview.md)を実行するために、次のエンティティに追加します。<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>例については、以下を参照してください。<br/>[グループへの増分の変更を取得する](delta-query-groups.md)<br/>[フォルダー内のメッセージへの増分の変更を取得する](delta-query-messages.md)<br/>[ユーザーへの増分の変更を取得する](delta-query-users.md) |
| 変更          | ベータ版        | [users](/graph/api/user-delta?view=graph-rest-beta) と [groups](/graph/api/group-delta?view=graph-rest-beta) に、オプションのクエリ フィルタリング機能 (ID 別) を追加します。 |

### <a name="added-user-resource-support-for-deleted-items"></a>削除されたアイテムをサポートするユーザー リソースの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [ユーザーの復元と完全削除](/graph/api/resources/directory?view=graph-rest-beta)に関するサポートを追加しました。 |

### <a name="added-onpremisesprovisioningerror"></a>OnPremisesProvisioningError の追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティ:[OnPremisesProvisioningError](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-beta) |
| 変更          | ベータ版        | [user](/graph/api/resources/user?view=graph-rest-beta)、[group](/graph/api/resources/group?view=graph-rest-beta)、および [orgcontact](/graph/api/resources/orgcontact?view=graph-rest-beta) への OnPremisesProvisioningError プロパティの追加 |

### <a name="added-deleteddatetime-property"></a>deletedDateTime プロパティの追加

|**変更の種類**|**バージョン**|**説明**|
|:-------------|:-----------|:--------------|
|変更|ベータ版|deletedDateTime プロパティを [user](/graph/api/resources/user?view=graph-rest-beta) エンティティに追加しました。
|変更|ベータ版|deletedDateTime プロパティを [group](/graph/api/resources/group?view=graph-rest-beta) エンティティに追加しました。
|変更|ベータ版|deletedDateTime プロパティを [application](/graph/api/resources/application?view=graph-rest-beta) エンティティに追加しました。

### <a name="added-domain-operations-to-v10"></a>V1.0 に追加されたドメイン操作

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [ドメイン](/graph/api/resources/domain?view=graph-rest-1.0)に操作を追加しました。<br/>新しいエンティティ:</br>[domain](/graph/api/resources/domain?view=graph-rest-1.0)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-1.0)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-1.0)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-1.0)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-1.0)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-1.0)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-1.0)<br/>新しいアクション:</br>[verify](/graph/api/domain-verify?view=graph-rest-1.0) |

### <a name="added-contracts-to-v10"></a>V1.0 追加されたコントラクト

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しいエンティティ:</br>[コントラクト](/graph/api/resources/contract?view=graph-rest-1.0) |

### <a name="added-licensedetails-to-v10"></a>V1.0 に追加された licenseDetails

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しいエンティティ:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-1.0) |
| 変更          | v1.0        | [users](/graph/api/resources/user?view=graph-rest-1.0) における新しい [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-1.0) ナビゲーション プロパティ |


### <a name="drive-api"></a>ドライブ API

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 追加 | v1.0 | **driveItem** の基本的なプロパティで構成される、**baseItem** リソース型を追加しました。
| 追加 | v1.0 およびベータ版 | **sourceItemId** プロパティを **thumbnail** に追加しました。 <br/> **siteUrl** プロパティを **sharepointIds** に追加しました。 <br/> **sharedBy** および **sharedDateTime** プロパティを **shared** に追加しました。 <br/> **shared** プロパティを **remoteItem** に追加しました。 <br/> **sharepointIds** プロパティを **drive** および **itemReference** に追加しました。 <br/> **lastAccessedDateTime** を **fileSystemInfo** に追加しました。 <br/> **driveItem** および **site** ナビゲーション プロパティを **sharedDriveItem** に追加しました。 <br/> **parentReference** プロパティを **baseItem** に追加しました。
| 変更 | v1.0 およびベータ版 | **driveItem** と **sharedDriveItem** が **baseItem** から継承されるように変更しました。 <br/> **identity** をオープン型としてマークしました。
| 変更 | ベータ版 | **configuratorUrl** と **webHtml** プロパティを **sharingLink** に追加しました。 <br/> **folderView** リソース タイプと **view** プロパティを **folder** リソース タイプに追加しました。 <br/> **listItem** ナビゲーション プロパティを **driveItem** に追加しました。 <br/> **list** ナビゲーション プロパティを **drive** に追加しました。


### <a name="extensions-open-extensions"></a>拡張機能 (オープン拡張機能)

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0          | [device](/graph/api/resources/device?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0) リソースで [openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0) をサポートします。 |
| 追加        | v1.0 およびベータ版 | ユーザーが個人の Microsoft アカウントでサインインした場合は、event、post、group、message、contact、および user リソースでオープン拡張機能をサポートします。(これは、これらのリソースと、ユーザーが職場または学校のアカウントを使用してサインインした場合にオープン拡張機能をサポートする device、group、organization および user に追加します。) |
| 追加        | v1.0 およびベータ版 | `$expand` をサポートしました。[device](/graph/api/resources/device?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[post](/graph/api/resources/post?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0) のリソースでオープンな[拡張機能を利用できます](/graph/api/opentypeextension-get?view=graph-rest-1.0)。 |
| 追加        | ベータ版          | `$expand` をサポートしました。[administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) で[オープン拡張機能が利用できます](/graph/api/opentypeextension-get?view=graph-rest-1.0)。 |


### <a name="extensions-schema-extensions"></a>拡張機能 (スキーマ拡張機能)

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0          | 新しいリソース [schemaExtension](/graph/api/resources/schemaextension?view=graph-rest-1.0) と CRUD メソッドで、次のリソースの拡張定義を管理します: [contact](/graph/api/resources/contact?view=graph-rest-1.0)、[device](/graph/api/resources/device?view=graph-rest-1.0)、[event](/graph/api/resources/event?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[message](/graph/api/resources/message?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[post](/graph/api/resources/post?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0)。[administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) サポートは、以前と同様ベータ版に制限されていることに注意してください。 |
| 追加        | v1.0          | リソース [contact](/graph/api/resources/contact?view=graph-rest-1.0)、[device](/graph/api/resources/device?view=graph-rest-1.0)、[event](/graph/api/resources/event?view=graph-rest-1.0)、[group](/graph/api/resources/group?view=graph-rest-1.0)、[message](/graph/api/resources/message?view=graph-rest-1.0)、[organization](/graph/api/resources/organization?view=graph-rest-1.0)、[post](/graph/api/resources/post?view=graph-rest-1.0)、[user](/graph/api/resources/user?view=graph-rest-1.0) の、既存の POST、GET、および ATCH メソッドが、対応するリソース インスタンスにスキーマ拡張機能として保存されているカスタム データの追加、取得、および更新または削除をサポートするようになりました。 |
| 追加        | v1.0 およびベータ版 | `$filter` を使用して、拡張機能名など特定の拡張機能プロパティの値と一致する　プロパティを持つリソース インスタンスを検索できるようになりました。詳細については、この[例](extensibility-schema-groups.md#5-get-a-group-and-its-extension-data)を参照してください。 |
| 変更          | v1.0 およびベータ版 | [スキーマ拡張機能の定義を削除](/graph/api/schemaextension-delete?view=graph-rest-1.0)しても、その定義に基づいて追加されたカスタム データへのアクセスに影響しなくなりました。 |
| 変更          | v1.0 およびベータ版 | スキーマ拡張機能の複合型を null に設定して、リソース・インスタンスからスキーマ拡張機能を削除できるようになりました。 |


### <a name="group"></a>グループ

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 追加 | v1.0 およびベータ版 | **drives** および **sites** ナビゲーション プロパティを **group** に追加しました。

### <a name="insights-apis"></a>Insights API

|**変更の種類**|**バージョン**|**説明**|
|:-------------|:-----------|:--------------|
|追加|ベータ版|追加された[共有 API](/graph/api/resources/insights-shared?view=graph-rest-beta)。<br />新しいリソース:<br />[sharingDetail](/graph/api/resources/insights-sharingdetail?view=graph-rest-beta) <br />[insightIdentity](/graph/api/resources/insights-insightidentity?view=graph-rest-beta) <br />
|追加|ベータ版|追加された[使用 API](/graph/api/resources/insights-used?view=graph-rest-beta)。<br />新しいリソース:<br />[usageDetails](/graph/api/resources/insights-usagedetails?view=graph-rest-beta) <br />
|変更|ベータ版|次のリソースの新しい**タイプ** プロパティ:<br />[resourceVisualization](/graph/api/resources/insights-resourcevisualization?view=graph-rest-beta) リソース。 <br />
|削除|ベータ版|次のエンティティを削除しました。<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)<br/>[cartToClassAssociation](/graph/api/resources/intune-deviceconfig-carttoclassassociation?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-beta)<br/>[eBookVppGroupAssignment](/graph/api/resources/intune-books-ebookvppgroupassignment?view=graph-rest-beta)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)<br/>[windowsDeviceMalwareState](/graph/api/resources/intune-endpointprotection-windowsdevicemalwarestate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-beta)<br/>[windowsMalwareInformation](/graph/api/resources/intune-endpointprotection-windowsmalwareinformation?view=graph-rest-beta)<br/>[windowsProtectionState](/graph/api/resources/intune-endpointprotection-windowsprotectionstate?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[androidPermissionAction](/graph/api/resources/intune-apps-androidpermissionaction?view=graph-rest-beta)<br/>[bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-beta)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) に [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) に [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) に [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-beta) アクションを追加しました |
| 削除    | ベータ版    | 次のエンティティを削除しました。<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| 削除    | ベータ版    | 次の複合型を削除しました。<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| 変更      | ベータ版    | [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに、次のプロパティを追加しました。**workProfilePasswordBlockFingerprintUnlock**、**workProfilePasswordBlockTrustAgents**、**workProfilePasswordExpirationDays**、**workProfilePasswordMinimumLength**、**workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**、**workProfilePasswordPreviousPasswordBlockCount**、**workProfilePasswordSignInFailureCountBeforeFactoryReset**、**workProfilePasswordRequiredType**、**workProfileRequirePassword**。 |
| 変更      | ベータ版    | [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) エンティティに、**subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **kioskModeManagedApps** プロパティを追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから **kioskModeManagedAppId** プロパティを削除しました |
| 変更      | ベータ版    | [androidPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidpkcscertificateprofile?view=graph-rest-beta) エンティティに、**subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [calendar](/graph/api/resources/calendar?view=graph-rest-beta) エンティティから **hexColor** プロパティを削除しました |
| 変更      | ベータ版    | [complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta) エンティティに、**setting** プロパティと **platformType** プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティから **windowsManagementAppEnabled** プロパティを削除しました |
| 変更      | ベータ版    | [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) エンティティに、**userName** プロパティ、**deviceModel** プロパティ、**platform** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) エンティティに、**userPrincipalName** プロパティと **deviceModel** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) エンティティに、**platformType**、**setting**、**userId**、**userEmail** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta) エンティティに、**inGracePeriodCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) エンティティに **userName** プロパティ、**deviceModel** プロパティ、**platform** プロパティを追加しました |
| 変更      | ベータ版    | [event](/graph/api/resources/event?view=graph-rest-beta) エンティティから **creationOptions** プロパティを削除しました |
| 変更      | ベータ版    | [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta) エンティティから **isDelegated** プロパティを削除しました |
| 変更      | ベータ版    | [group](/graph/api/resources/group?view=graph-rest-beta) エンティティから、**unseenConversationsCount** プロパティと **unseenMessagesCount** プロパティを削除しました |
| 変更      | ベータ版    | [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) エンティティに **settingXml** プロパティと **settings** プロパティを追加しました |
| 変更      | ベータ版    | [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile?view=graph-rest-beta) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) エンティティに **systemIntegrityProtectionEnabled** プロパティを追加しました |
| 変更      | ベータ版    | [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、**complianceGracePeriodExpirationDateTime**、**userPrincipalName**、**imei** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティから **settingXml** プロパティと **settings** プロパティを削除しました |
| 変更      | ベータ版    | [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティに、次のプロパティを追加しました。**useSharedComputerActivation**、**updateChannel**、**officePlatformArchitecture**、**localesToInstall**。 |
| 変更      | ベータ版    | [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) エンティティから **applePushNotificationCertificateSetting** プロパティを削除しました |
| 変更      | ベータ版    | [post](/graph/api/resources/post?view=graph-rest-beta) エンティティで次のプロパティを変更しました。<br/>**sender** を省略可能から必須に変更しました<br/> |
| 変更      | ベータ版    | [softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta) エンティティに、次のプロパティを追加しました。**compliantUserCount**、**nonCompliantUserCount**、**remediatedUserCount**、**errorUserCount**、**unknownUserCount**、**conflictUserCount**、**notApplicableUserCount**。 |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、次のプロパティを追加しました。**bluetoothAllowedServices**、**bluetoothBlockPrePairing**、**cellularData**、**defenderDetectedMalwareActions**、**defenderPotentiallyUnwantedAppAction**、**lockScreenAllowTimeoutConfiguration**、**lockScreenBlockCortana**、**lockScreenBlockToastNotifications**、**lockScreenTimeoutInSeconds**、**passwordBlockSimple**、**privacyAutoAcceptPairingAndConsentPrompts**、**privacyBlockInputPersonalization**、**startMenuHideChangeAccountSettings**、**startMenuHideHibernate**、**startMenuHideLock**、**startMenuHideShutDown**、**startMenuHideSignOut**、**startMenuHideSleep**、**startMenuHideSwitchAccount**、**settingsBlockAppsPage**、**settingsBlockGamingPage**、**windowsSpotlightBlockConsumerSpecificFeatures**、**windowsSpotlightBlocked**、**windowsSpotlightBlockOnActionCenter**、**windowsSpotlightBlockTailoredExperiences**、**windowsSpotlightBlockThirdPartyNotifications**、**windowsSpotlightBlockWelcomeExperience**、**windowsSpotlightBlockWindowsTips**、**windowsSpotlightConfigureOnLockScreen**、**connectedDevicesServiceBlocked**。 |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティから次のプロパティを削除しました。**automaticUpdateMode**、**automaticUpdateSchedule**、**automaticUpdateTime**、**prereleaseFeatures**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips**、**experienceBlockConsumerSpecificFeatures**。 |
| 変更      | ベータ版    | [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティに、**indexingEncryptedStoresOrItemsBlocked** プロパティと **smbAutoEncryptedFileExtensions** プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**rightsManagementServicesTemplateId** を必須から省略可能に変更しました<br/> |
| 変更      | ベータ版    | [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**productCode** を必須から省略可能に変更しました<br/> |
| 変更      | ベータ版    | [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **mobileAppConfigurations** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、**cartToClassAssociations**、**deviceCompliancePolicySettingStateSummaries**、**remoteAssistancePartners**、**windowsInformationProtectionAppLearningSummaries**、**windowsMalwareInformation** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta) エンティティに **eBook** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **windowsProtectionState** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) エンティティに **installSummary** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) エンティティから **outlook** ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta) エンティティから **healthStates** ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [defaultDeviceEnrollmentRestrictions](/graph/api/resources/intune-onboarding-defaultdeviceenrollmentrestrictions?view=graph-rest-beta) 複合型に **androidForWorkRestrictions** プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) 複合型に **userPrincipalName** プロパティと **sources** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 複合型に **userPrincipalName** プロパティと **sources** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) 複合型に、**settingName**、**userId**、**userName**、**userEmail**、**currentValue** の各プロパティを追加しました |
| 変更      | ベータ版    | [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) 複合型から **archiveFolder** プロパティを削除しました |


### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | **findMeetingTimes**に対して、列挙型の値 **unrestricted** を追加しました。これは、**timeConstraint** パラメーターの一部である **activityDomain** プロパティとして指定します。これにより、**findMeetingTimes**はスケジュールを設定しているアクティビティの種類に適した時間を検索します。詳細については、[要求の本文](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body)セクションを参照してください。 |
| 追加        | ベータ版          | **イベント**の本文を、既定の HTML 形式の代わりにプレーン テキストで取得することをサポートします。詳細については、[get](/graph/api/event-get?view=graph-rest-beta) および [list](/graph/api/user-list-events?view=graph-rest-beta) イベントを参照してください。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | **メッセージ**の本文を、既定の HTML 形式の代わりにプレーン テキストで取得することをサポートします。詳細については、[get](/graph/api/message-get?view=graph-rest-beta) および [list](/graph/api/user-list-messages?view=graph-rest-beta) イベントを参照してください。 |


### <a name="outlook-tasks"></a>Outlook のタスク

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Outlook タスクにアクセスするために、新しい **Outlook** ナビゲーション プロパティを [user](/graph/api/resources/user?view=graph-rest-beta) に追加しました。 |
| 追加        | ベータ版        | 新しいエンティティ ([outlookuser](/graph/api/resources/outlookuser?view=graph-rest-beta)、[outlookTaskGroup](/graph/api/resources/outlooktaskgroup?view=graph-rest-beta)、[outlookTaskFolder](/graph/api/resources/outlooktaskfolder?view=graph-rest-beta)、および [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta)) とそれらのメソッドが、Outlook タスクの整理とアクセスをサポートします。 |
| 追加        | ベータ版        | Outlook タスクで添付ファイルをサポートします ([attachment](/graph/api/resources/attachment?view=graph-rest-beta)、[fileAttachment](/graph/api/resources/fileattachment?view=graph-rest-beta)、[itemAttachment](/graph/api/resources/itemattachment?view=graph-rest-beta)、および [referenceAttachment](/graph/api/resources/referenceattachment?view=graph-rest-beta) リソース)。 |
| 追加        | ベータ版        | Outlook タスクで[拡張プロパティ](/graph/api/resources/extended-properties-overview?view=graph-rest-beta)をサポートします ([singleValueLegacyExtendedProperty](/graph/api/resources/singlevaluelegacyextendedproperty?view=graph-rest-beta) および [multiValueLegacyExtendedProperty](/graph/api/resources/multivaluelegacyextendedproperty?view=graph-rest-beta) リソース)。 |

### <a name="planner-apis"></a>Planner API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [Planner API](/graph/api/resources/planner-overview?view=graph-rest-1.0) を追加しました。<br />新しいリソース:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-1.0) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-1.0) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-1.0) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-1.0) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-1.0) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-1.0) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-1.0) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-1.0) |

### <a name="sharepoint-sites"></a>SharePoint サイト

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 追加      | v1.0      | サイト リソースが v1.0 エンドポイントで使用できるようになりました。<br/> **site** および **siteCollection** リソース型を追加しました。
| 変更        | ベータ版      | **site** リソースの ID の形式を変更しました。これはベータ版 API の大きな変更点です。
| 削除       | ベータ版      | **sharePoint** エンティティをベータ版 API から削除しました。この機能は、現在 **sites**コレクションから使用できます。

### <a name="sharepoint-lists"></a>SharePoint リスト

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 変更 | ベータ版 | **Sharepoint** のナビゲーション プロパティを削除しました。サイトは、**sites** ナビゲーション プロパティから直接アクセスできるようになりました。<br/> **fieldDefinition** リソースを削除しました。これは既に **columnDefinition** に置き換えられています。<br/> **siteCollectionId** および **siteId** プロパティを **site** から削除しました。代わりに **sharepointIds** を使用します。<br/> **listItemId** プロパティを **listItem** から削除しました。代わりに **sharepointIds** を使用します。<br/> **listItem** の **columnSet** プロパティの名前を **fields** に変更しました。 <br/> **site** リソースを、ID の一部に SharePoint ホスト名を使用するように変更しました。
| 追加 | ベータ版 | **booleanColumn**、**calculatedColumn**、**choiceColumn**、**dateTimeColumn**、**lookupColumn**、**numberColumn**、**personOrGroupColumn**、および **textColumn** リソース型を追加しました。 <br/> **displayName** プロパティを **site** に追加しました。 <br/> **columns** ナビゲーション プロパティを **site** に追加しました。 <br/> **list** および **listItem** ナビゲーション プロパティを **sharedDriveItem** に追加しました。 <br/> **sharepointIds** プロパティを **list** と **listItem**、および **site** に追加しました。 <br/> **columnDefinition** リソース型を追加しました。




## <a name="april-2017"></a>2017 年 4 月

### <a name="administrative-units-property-changes"></a>管理単位のプロパティ変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | 管理単位の API がプレビュー (ベータ版) で更新されます。最初の一連の変更は、2017 年 5 月 3 日に適用されます。これには、次のプロパティ名の変更が含まれます。<br />scopedRoleMembership エンティティの - **roleMemberInfo** 複合型が **ID** 複合型に変更されます<br />user エンティティの - **scopedAdministratorOf** ナビゲーション プロパティが **scopedRoleMemberOf** に変更されます<br />administrativeUnit エンティティの - **scopedAdministrators** ナビゲーション プロパティが **scopedRoleMembers** に変更されます<br />directoryRole エンティティの - **scopedAdministrators** ナビゲーション プロパティが **scopedMembers** に変更されます |

### <a name="application-and-serviceprincipal-api-changes"></a>application API と servicePrincipal API の変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [application](/graph/api/resources/application?view=graph-rest-beta) API と [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) API は、プレビュー (ベータ版) で更新されます。最初の一連の変更は、2017 年 5 月 15 日に適用されます。変更には、プロパティの名前変更と再構築が含まれます。一部のプロパティ (appRoles、addIns など) は、変更が完了するまで利用できません。変更は、v1.0 へのリリース前にプレビュー (ベータ版) でリリースされます。 |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>クラウド ソリューション プロバイダー開発者向けプレビュー サポートの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | クラウド ソリューション プロバイダーの事前承認されたアプリケーションが Microsoft Graph を呼び出せるようにする、新しいプレビュー機能を追加し、新しい[承認トピック](auth-cloudsolutionprovider.md)に記載しました。 |

### <a name="added-onpremises-properties-to-user-entity"></a>user エンティティへの onPremises プロパティの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [user](/graph/api/resources/user?view=graph-rest-beta) エンティティに、新しい onPremises プロパティである onPremisesDomainName、OnPremisesSamAccountName、onPremisesUserPrincipalName を追加しました。 |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>新しい Planner API とグループ可視性プロパティに対する更新

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [Group](/graph/api/resources/group?view=graph-rest-beta) エンティティに、可視性プロパティの追加の値として **HiddenMembership** を追加しました |
| 追加        | ベータ版        | 新しい [Planner API](/graph/api/resources/planner-overview?view=graph-rest-beta) を追加しました。<br />新しいリソース:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-beta) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-beta) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-beta) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-beta) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-beta) |

### <a name="intune-apis"></a>Intune API
| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティを追加しました。<br/>[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-beta)<br/>[deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta)<br/>[deviceManagementScriptGroupAssignment](/graph/api/resources/intune-deviceconfig-devicemanagementscriptgroupassignment?view=graph-rest-beta)<br/>[deviceManagementScriptState](/graph/api/resources/intune-deviceconfig-devicemanagementscriptstate?view=graph-rest-beta)<br/>[eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-beta)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-beta)<br/>[windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-deviceconfig-windowsmanagementapphealthstate?view=graph-rest-beta)<br/> |
| 追加        | ベータ版        | 新しい複合型を追加しました。<br/>[dailySchedule](/graph/api/resources/intune-deviceconfig-dailyschedule?view=graph-rest-beta)<br/>[hourlySchedule](/graph/api/resources/intune-deviceconfig-hourlyschedule?view=graph-rest-beta)<br/>[iosBookmark](/graph/api/resources/intune-deviceconfig-iosbookmark?view=graph-rest-beta)<br/>[iosWebContentFilterAutoFilter](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterautofilter?view=graph-rest-beta)<br/>[iosWebContentFilterBase](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterbase?view=graph-rest-beta)<br/>[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta)<br/>[runSchedule](/graph/api/resources/intune-deviceconfig-runschedule?view=graph-rest-beta)<br/>[sharedAppleDeviceUser](/graph/api/resources/intune-deviceconfig-sharedappledeviceuser?view=graph-rest-beta)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-beta)<br/> |
| 追加        | ベータ版        | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta) に [assign](/graph/api/intune-deviceconfig-devicemanagementscript-assign?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) に [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-synclicenses?view=graph-rest-beta) アクションを追加しました |
| 追加        | ベータ版        | [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) コレクションに **getTopMobileApps** 関数を追加しました |
| 追加        | ベータ版        | [applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta) に [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-deviceconfig-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-beta) 関数を追加しました |
| 追加        | ベータ版        | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) に [getDeviceComplianceSettingStates](/graph/api/intune-deviceconfig-devicemanagement-getdevicecompliancesettingstates?view=graph-rest-beta) 関数を追加しました |
| 追加        | ベータ版        | [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-beta) 関数を追加しました |
| 追加        | ベータ版        | [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) に [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-beta) 関数を追加しました |
| 削除        | ベータ版        | 次の複合型を削除しました。<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| 変更          | ベータ版        | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **deviceSharingAllowed** プロパティを追加しました |
| 変更          | ベータ版        | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから **deviceSharingBlocked** プロパティを削除しました。 |
| 変更          | ベータ版        | [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) エンティティに **minimumRequiredSdkVersion** プロパティを追加しました |
| 変更          | ベータ版        | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **windowsManagementAppEnabled** プロパティを追加しました |
| 変更          | ベータ版        | [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) エンティティに **notificationTemplateId** プロパティを追加しました |
| 変更          | ベータ版        | [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) エンティティに **excludeGroup** プロパティを追加しました |
| 変更          | ベータ版        | [iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**payloadFileName** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) エンティティに **contentFilterSettings** プロパティを追加しました |
| 変更          | ベータ版        | [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **cellularBlockPersonalHotspot** プロパティと **passcodeBlockFingerprintModification** プロパティを追加しました |
| 変更          | ベータ版        | [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) エンティティに **minimumRequiredSdkVersion** プロパティを追加しました |
| 変更          | ベータ版        | [macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**payloadFileName** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) エンティティに、**disableAppPinIfDevicePinIsSet**、**minimumRequiredOsVersion**、**minimumWarningOsVersion**、**minimumRequiredAppVersion**、**minimumWarningAppVersion** の各プロパティを追加しました |
| 変更          | ベータ版        | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、**remoteAssistanceSessionUrl**、**isEncrypted**、**model**、**manufacturer** の各プロパティを追加しました |
| 変更          | ベータ版        | [getMobileAppCount](/graph/api/intune-apps-mobileapp-getmobileappcount?view=graph-rest-beta) エンティティで次のプロパティを変更しました。<br/>**bindingParameter** を **mobileApp** から *mobileApp* の **collection** に変更しました<br/>**status** を GUID から String に変更しました<br/> |
| 変更          | ベータ版        | [mobileAppGroupAssignment](/graph/api/resources/intune-apps-mobileappgroupassignment?view=graph-rest-beta) エンティティに **vpnConfigurationId** プロパティを追加しました |
| 変更          | ベータ版        | [notificationMessageTemplate](/graph/api/resources/intune-deviceconfig-notificationmessagetemplate?view=graph-rest-beta) エンティティから **fromEmailAddress** プロパティを削除しました |
| 変更          | ベータ版        | [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティに **excludedApps** プロパティを追加しました |
| 変更          | ベータ版        | [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) エンティティから **excludedOfficeApps** プロパティを削除しました |
| 変更          | ベータ版        | [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) エンティティに **enabled** プロパティを追加しました |
| 変更          | ベータ版        | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、**networkProxyApplySettingsDeviceWide**、**networkProxyDisableAutoDetect**、**networkProxyAutomaticConfigurationUrl**、**networkProxyServer**、**bluetoothDeviceName**、**wiFiScanInterval**、**wirelessDisplayBlockProjectionToThisDevice**、**wirelessDisplayBlockUserInputFromReceiver**、**wirelessDisplayRequirePinForPairing**、**experienceBlockDeviceDiscovery**、**experienceBlockErrorDialogWhenNoSIM**、**experienceBlockTaskSwitcher**、**startMenuPinnedFolderDocuments**、**startMenuPinnedFolderDownloads**、**startMenuPinnedFolderFileExplorer**、**startMenuPinnedFolderHomeGroup**、**startMenuPinnedFolderMusic**、**startMenuPinnedFolderNetwork**、**startMenuPinnedFolderPersonalFolder**、**startMenuPinnedFolderPictures**、**startMenuPinnedFolderSettings**、**startMenuPinnedFolderVideos**、**startMenuAppListVisibility**、**startMenuHideFrequentlyUsedApps**、**startMenuHideRecentJumpLists**、**startMenuHideRecentlyAddedApps**、**startMenuHideRestartOptions**、**startMenuHideUserTile**、**startMenuHidePowerButton**、**startMenuLayoutEdgeAssetsXml**、**personalizationDesktopImageUrl**、**personalizationLockScreenImageUrl** の各プロパティを追加しました |
| 変更          | ベータ版        | [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**productCode** を Guid から String に変更しました<br/> |
| 変更          | ベータ版        | [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**phoneProductIdentifier** を必須から省略可能に変更しました<br/>**phonePublisherId** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**appXPackageInformationList** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) エンティティに **productKey** プロパティと **licenseType** プロパティを追加しました |
| 変更          | ベータ版        | [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティに **previewBuildSetting** プロパティを追加しました |
| 変更          | ベータ版        | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **windowsManagementApp** ナビゲーション プロパティと **managedEBooks** ナビゲーション プロパティを追加しました |
| 変更          | ベータ版        | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **deviceManagementScripts**、**managedDeviceOverview**、**cloudPkiSubscriptions** の各ナビゲーション プロパティを追加しました |
| 変更          | ベータ版        | [deviceEnrollmentPlatformRestrictions](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictions?view=graph-rest-beta) 複合型に **osMinimumVersion** プロパティと **osMaximumVersion** プロパティを追加しました |
| 変更          | ベータ版        | [hardwareInformation](/graph/api/resources/intune-deviceconfig-hardwareinformation?view=graph-rest-beta) 複合型に **isSharedDevice** プロパティと **sharedDeviceCachedUsers** プロパティを追加しました |
| 変更          | ベータ版        | [omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-beta) 複合型で次のプロパティを変更しました:<br/>**fileName** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-beta) 複合型で次のプロパティを変更しました:<br/>**fileName** を必須から省略可能に変更しました<br/> |

## <a name="march-2017"></a>2017 年 3 月

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta)<br/>[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta)<br/>[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta)<br/>[complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-beta)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta)<br/>[enterpriseCodeSigningCertificate](/graph/api/resources/intune-apps-enterprisecodesigningcertificate?view=graph-rest-beta)<br/>[iosEduDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosedudeviceconfiguration?view=graph-rest-beta)<br/>[managedDeviceCertificateState](/graph/api/resources/intune-devices-manageddevicecertificatestate?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta)<br/>[mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)<br/>[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-beta)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta)<br/>[symantecCodeSigningCertificate](/graph/api/resources/intune-apps-symanteccodesigningcertificate?view=graph-rest-beta)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-beta)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationExampleJson](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexamplejson?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-deviceconfig-deviceexchangeaccessstatesummary?view=graph-rest-beta)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-beta)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-beta)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-beta)<br/>[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta)<br/>[iosEduCertificateSettings](/graph/api/resources/intune-deviceconfig-ioseducertificatesettings?view=graph-rest-beta)<br/>[ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResource](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresource?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-beta)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) に [requestSignupUrl](/graph/api/intune-androidforwork-androidforworksettings-requestsignupurl?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) に [completeSignup](/graph/api/intune-androidforwork-androidforworksettings-completesignup?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) に [syncApps](/graph/api/intune-androidforwork-androidforworksettings-syncapps?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) に [unbind](/graph/api/intune-androidforwork-androidforworksettings-unbind?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) に [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) に [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) に [removeApplePushNotificationCertificate](/graph/api/intune-onboarding-organization-removeapplepushnotificationcertificate?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) に [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-iosmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) に [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-androidmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) に [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-targetedmanagedappconfiguration-updatemobileappidentifierdeployments?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) に [updateTargetedSecurityGroups](/graph/api/intune-mam-iosmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) に [updateTargetedSecurityGroups](/graph/api/intune-mam-androidmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) に [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta) に [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy) に [updateTargetedSecurityGroups](/graph/api/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy-updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) に [wipeManagedAppRegistrationByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationbydevicetag?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) に [getTopMobileApps](/graph/api/intune-apps-mobileapp-gettopmobileapps?view=graph-rest-beta) 関数を追加しました |
| 追加    | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) に [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-corpenrollment-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-beta) 関数を追加しました |
| 削除    | ベータ版    | 次のエンティティを削除しました。<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/> |
| 削除    | ベータ版    | 次の複合型を削除しました。<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/> |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **webBrowserBlockPopups** プロパティを追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから **webBrowserAllowPopups** プロパティを削除しました |
| 変更      | ベータ版    | [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta) エンティティに **appIdentifier** プロパティを追加しました |
| 変更      | ベータ版    | [appReportingOverviewStatus](/graph/api/resources/appreportingoverviewstatus?view=graph-rest-beta) エンティティから **applicationCount**、**failedApplicationCount**、**appInstallFailures** の各プロパティを削除しました |
| 変更      | ベータ版    | [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) エンティティに **sharedIPadMaximumUserCount** プロパティと **enableSharedIPad** プロパティを追加しました |
| 変更      | ベータ版    | [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) エンティティに **shareTokenWithSchoolDataSyncService** プロパティと **lastSyncErrorCode** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) エンティティから、**numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) エンティティから、**numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) エンティティから、**numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) エンティティから、**numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに **subscriptionState** プロパティを追加しました |
| 変更      | ベータ版    | [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) エンティティに **managedEmailProfileRequired** プロパティを追加しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **appsSingleAppModeList** プロパティを追加しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティから **appsSingleAppModeBundleIds** プロパティを削除しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティに **expirationDateTime** プロパティを追加しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティから **expiration** プロパティを削除しました |
| 変更      | ベータ版    | [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) エンティティに、**passwordMinimumCharacterSetCount**、**osMinimumVersion**、**osMaximumVersion**、**deviceThreatProtectionEnabled**、**deviceThreatProtectionRequiredSecurityLevel**、**storageRequireEncryption** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに、**isSupervised**、**exchangeLastSuccessfulSyncDateTime**、**exchangeAccessState**、**exchangeAccessStateReason** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) エンティティに **deviceExchangeAccessStateSummary** プロパティを追加しました |
| 変更      | ベータ版    | [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) エンティティから **installSummary** プロパティを削除しました |
| 変更      | ベータ版    | [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) エンティティに **uploadState** プロパティを追加しました |
| 変更      | ベータ版    | [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) エンティティで次のプロパティを変更しました:<br/>**azureStorageUriExpirationDateTime** を必須から省略可能に変更しました<br/> |
| 変更      | ベータ版    | [remoteActionAudit](/graph/api/resources/intune-deviceconfig-remoteactionaudit?view=graph-rest-beta) エンティティに、**initiatedByUserPrincipalName**、**deviceOwnerUserPrincipalName**、**deviceIMEI**、**actionState** の各プロパティを追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに、**oneDriveDisableFileSync**、**safeSearchFilter**、**edgeSearchEngine**、**settingsBlockSettingsApp**、**settingsBlockSystemPage**、**settingsBlockDevicesPage**、**settingsBlockNetworkInternetPage**、**settingsBlockPersonalizationPage**、**settingsBlockAccountsPage**、**settingsBlockTimeLanguagePage**、**settingsBlockEaseOfAccessPage**、**settingsBlockPrivacyPage**、**settingsBlockUpdateSecurityPage**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips**、**experienceBlockConsumerSpecificFeatures**、**startMenuLayoutXml**、**startMenuMode**、**logonBlockFastUserSwitching**、**startBlockUnpinningAppsFromTaskbar** の各プロパティを追加しました |
| 変更      | ベータ版    | [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) エンティティに、**allowPrinting**、**allowScreenCapture**、**allowTextSuggestion** の各プロパティを追加しました |
| 変更      | ベータ版    | [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) エンティティから、**blockPrinting**、**blockScreenCapture**、**blockTextSuggestion** の各プロパティを削除しました |
| 変更      | ベータ版    | [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) エンティティに **identityName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**applicableArchitectures** を [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) エンティティに **identityName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**applicableArchitectures** を [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) エンティティに、**identityName**、**identityPublisherHash**、**identityResourceIdentifier** の各プロパティを追加しました |
| 変更      | ベータ版    | [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**applicableArchitectures** を [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) から String に変更しました<br/>**applicableDeviceTypes** を [windowsDeviceType](/graph/api/resources/windowsdevicetype?view=graph-rest-beta) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) エンティティに **restartMode** プロパティを追加しました |
| 変更      | ベータ版    | [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに、**enterpriseCodeSigningCertificates**、**symantecCodeSigningCertificate**、**sideLoadingKeys**、**managedAppPolicies**、**iosManagedAppProtections**、**androidManagedAppProtections**、**defaultManagedAppProtections**、**targetedManagedAppConfigurations**、**mdmWindowsInformationProtectionPolicies**、**windowsInformationProtectionPolicies**、**managedAppRegistrations**、**managedAppStatuses** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティから、**appReportingOverview**、**enterpriseCerts**、**symantecCert** の各ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティに **deviceSettingStateSummaries** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティに **deviceSettingStateSummaries** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) エンティティに、**termsAndConditions**、**androidForWorkSettings**、**androidForWorkAppConfigurationSchemas**、**applePushNotificationCertificate**、**softwareUpdateStatusSummary**、**deviceCompliancePolicyDeviceStateSummary**、**complianceSettingStateSummaries**、**deviceConfigurationDeviceStateSummaries**、**mobileThreatDefenseConnectors** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta) エンティティから、**teacherRootCertificates**、**teacherIdentityCertificate**、**studentRootCertificates**、**studentIdentityCertificate** の各ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**deviceStatuses** を [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta) コレクションから [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) コレクションに変更しました<br/>**groupAssignments** を [appProvisioningConfigGroupAssignment](/graph/api/resources/appprovisioningconfiggroupassignment?view=graph-rest-beta) コレクションから [mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta) コレクションに変更しました<br/> |
| 変更      | ベータ版    | [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティに **deviceConfigurationStates** ナビゲーション プロパティと **deviceCompliancePolicyStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) エンティティに **deviceStatusSummary** ナビゲーション プロパティと **userStatusSummary** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) エンティティに **installSummary** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) エンティティから **sideLoadingKeys** ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) 複合型から、**applicationId**、**appName**、**platformId**、**userFailures**、**deviceFailures** の各プロパティを削除しました |
| 変更      | ベータ版    | [iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta) 複合型に **displayName** プロパティを追加しました |
| 変更      | ベータ版    | [iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta) 複合型に **displayName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) 複合型に、**subjectName**、**description**、**expirationDateTime**、**certificate** の各プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) 複合型から **dataRecoveryCertificate** プロパティと **certificateFileName** プロパティを削除しました |
| 変更      | ベータ版    | [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) 複合型に **displayName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) 複合型で次のプロパティの型を変更しました:<br/>**applicableArchitecture** を [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) 複合型で次のプロパティを変更しました:<br/>**applicableArchitecture** を省略可能から必須に変更しました<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Microsoft Graph へのコントラクトの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいリソース:</br>[コントラクト](/graph/api/resources/contract?view=graph-rest-beta) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Microsoft Graph へのドメイン操作の追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [ドメイン](/graph/api/resources/domain?view=graph-rest-beta)に関数を追加しました。<br/>新しいエンティティ:</br>[domain](/graph/api/resources/domain?view=graph-rest-beta)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-beta)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-beta)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-beta)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-beta)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-beta)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-beta)<br/>新しいアクション:</br>[forceDelete](/graph/api/domain-forcedelete?view=graph-rest-beta)</br>[verify](/graph/api/domain-verify?view=graph-rest-beta) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>スキーマ拡張機能を使用して Microsoft Graph にカスタム データを追加する

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Microsoft Graph を、[スキーマ拡張機能](extensibility-overview.md#schema-extensions)を使用してアプリケーション データによって拡張します。これは、次のリソースでサポートされています。<br/>管理単位<br/>予定表イベント<br/>デバイス<br/>グループ<br/>message<br/>組織<br/>個人用連絡先<br/>投稿<br/>ユーザー<br/>次の例を参照してください。<br/>[スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](extensibility-schema-groups.md) |
| 追加        | ベータ版        | 検証済みの .com バニティ ドメインを必要とせずに、スキーマ拡張機能の定義を作成する別の方法が提供されました。詳しくは、[スキーマ拡張機能](extensibility-overview.md#schema-extensions)を参照してください。 |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>オープン拡張機能を使用して Microsoft Graph にカスタム データを追加する

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | 「Office 365 のデータ拡張機能」というこれまでの名称が「オープン拡張機能」に変更されました。 |
| 追加        | ベータ版          | [オープン拡張機能](extensibility-overview.md#open-extensions)をサポートする追加リソース: <br/>管理単位<br/>デバイス<br/>group<br/>組織<br/>ユーザー<br/>次の例を参照してください。<br/>[オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](extensibility-open-users.md) |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [グループの復元と完全削除](/graph/api/resources/directory?view=graph-rest-beta)に関するサポートが追加されました。<br/>新しいエンティティ: deleteditems ナビゲーション プロパティを持つディレクトリ。 |
| 追加        | ベータ版        | 新しいエンティティ:</br>[Endpoint](/graph/api/resources/endpoint?view=graph-rest-beta) |
| 変更          | ベータ版        | [groups](/graph/api/resources/group?view=graph-rest-beta) における新たな [endpoints](/graph/api/group-list-endpoints?view=graph-rest-beta) ナビゲーション プロパティ |
| 追加        | ベータ版        | 新しいエンティティ:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-beta) |
| 変更          | ベータ版        | [users](/graph/api/resources/user?view=graph-rest-beta) における新たな [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-beta) ナビゲーション プロパティ |

### <a name="reports-apis"></a>レポート API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Office 365 レポートの新しいプレビュー API が導入されました。この API を使用すると、対象ビジネスにおけるユーザーの Office 365 サービスの使用法に関する使用状況レポートを取得できます。たとえば、サービスをよく利用してクォータに到達しそうなユーザーや、Office 365 ライセンスを必要としない可能性があるユーザーなどを識別できます。詳しくは、[レポート](/graph/api/resources/report?view=graph-rest-beta)を参照してください。 |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティ:</br>[コントラクト](/graph/api/resources/contract?view=graph-rest-beta) |

## <a name="february-2017"></a>2017 年 2 月

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/>[androidForWorkEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkeasemailprofilebase?view=graph-rest-beta)<br/>[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidForWorkGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgmaileasconfiguration?view=graph-rest-beta)<br/>[androidForWorkNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworknineworkeasconfiguration?view=graph-rest-beta)<br/>[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/>[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/>[androidForWorkTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidforworktrustedrootcertificate?view=graph-rest-beta)<br/>[androidForWorkWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkwificonfiguration?view=graph-rest-beta)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-beta)<br/>[appProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-appprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)<br/>[enterpriseCertificate](/graph/api/resources/intune-apps-enterprisecertificate?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)<br/>[symantecCertificate](/graph/api/resources/intune-apps-symanteccertificate?view=graph-rest-beta)<br/>[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)<br/>[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)<br/>[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)<br/>[windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)<br/>[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)<br/>[windowsArchitecture](/graph/api/resources/intune-apps-windowsarchitecture?view=graph-rest-beta)<br/>[windowsDeviceType](/graph/api/resources/intune-apps-windowsdevicetype?view=graph-rest-beta)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta)<br/> |
| 追加    | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティに [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティに [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに [updateTargetedSecurityGroups](/graph/api/intune-mam-targetedmanagedappconfiguration-updatetargetedsecuritygroups?view=graph-rest-beta) アクションを追加しました |
| 追加    | ベータ版    | [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) エンティティに [getScopesForUser](/graph/api/intune-rbac-resourceoperation-getscopesforintune-devices-user?view=graph-rest-beta) 関数を追加しました |
| 変更      | ベータ版    | [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) エンティティに **assetTagTemplate**、**lockScreenFootnote**、**homeScreenDockIcons**、**homeScreenPages** の各プロパティを追加しました |
| 変更      | ベータ版    | [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) エンティティから **deviceSharingAssetTagInformation**、**deviceSharingLockScreenFootnote**、**homeScreenLayoutDockIcons**、**homeScreenLayoutPages** の各プロパティを削除しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) エンティティに **appsSingleAppModeBundleIds** プロパティを追加しました |
| 変更      | ベータ版    | [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティに **createdDateTime**、**description**、**lastModifiedDateTime**、**displayName**、**version** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) エンティティに **createdDateTime** プロパティと **lastModifiedDateTime** プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) エンティティから **deviceRegistrationState** プロパティを削除しました |
| 変更      | ベータ版    | [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) エンティティに **manifest** プロパティを追加しました |
| 変更      | ベータ版    | [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティに **osDescription** プロパティと **userName** プロパティを追加しました |
| 変更      | ベータ版    | [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティから **deviceType** プロパティを削除しました |
| 変更      | ベータ版    | [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**mobileAppInstallStatusValue** を Int32 から文字列に変更しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティに **targetedSecurityGroupIds** プロパティと **targetedSecurityGroupsCount** プロパティを追加しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) エンティティから **numberOfTargetedSecurityGroups** プロパティを削除しました |
| 変更      | ベータ版    | [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) エンティティに **id** プロパティを追加しました |
| 変更      | ベータ版    | [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) エンティティから **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue**、**certificateValidityPeriodScale** の各プロパティを削除しました |
| 変更      | ベータ版    | [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta) エンティティから **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue**、**certificateValidityPeriodScale** の各プロパティを削除しました |
| 変更      | ベータ版    | [windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-beta) エンティティから **applyToWindows10Mobile** プロパティを削除しました |
| 変更      | ベータ版    | [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) エンティティに **enterpriseCerts**、**iosLobAppProvisioningConfigurations**、**symantecCert** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティに **userStatusOverview** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティに **userStatusOverview** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) エンティティに **groupAssignments**、**deviceStatuses**、**userStatuses** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta) エンティティで次のプロパティの型を変更しました:<br/>**identityCertificate** を [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) から [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta) に変更しました |
| 変更      | ベータ版    | [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型に **deviceComplianceCheckinThresholdDays** プロパティと **isScheduledActionEnabled** プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) 複合型から **windowsCommercialId** プロパティと **windowsCommercialIdLastModifiedTime** プロパティを削除しました |
| 変更      | ベータ版    | [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) 複合型に **bundleID**、**appName**、**publisher**、**enabled**、**showOnLockScreen** の各プロパティを追加しました |
| 変更      | ベータ版    | [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) 複合型から **bundleIdentifier**、**notificationsEnabled**、**showInLockScreen** の各プロパティを削除しました |



## <a name="january-2017"></a>2017 年 1 月

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [user](/graph/api/resources/user?view=graph-rest-1.0) リソースの新しいアクション [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)。 |
| 追加        | v1.0        | 新しい複合型 [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-1.0)。attendee 型の型プロパティで構成されます。 |
| 追加        | v1.0        | 新しい複合型:<br/>[attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-1.0)<br/>[locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-1.0) <br/>[locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-1.0)<br/>[meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-1.0)<br/>[meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-1.0)<br/>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-1.0)<br/>[timeSlot](/graph/api/resources/timeslot?view=graph-rest-1.0) |
| 変更          | v1.0        | [attendee](/graph/api/resources/attendee?view=graph-rest-1.0) 複合型は、[recipient](/graph/api/resources/recipient?view=graph-rest-1.0) から派生する attendeeBase から派生するようになりました。継承されたプロパティを含めて、以前と同じ **status**、**type**、**emailAddress** プロパティで構成されます。 |
| 追加        | ベータ版        | hexColor が、[calendar](/graph/api/resources/calendar?view=graph-rest-beta) リソースに追加されました。 |

### <a name="intune-apis"></a>Intune API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティを追加しました。 <br/>[appReportingOverviewStatus](/graph/api/resources/intune-apps-appreportingoverviewstatus?view=graph-rest-beta)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)<br/>[deviceManagementExchangeOnpremisesPolicy](/graph/api/resources/intune-onboarding-devicemanagementexchangeonpremisespolicy?view=graph-rest-beta)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)<br/>[onpremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-beta)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)<br/>[windows10WindowsInformationProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10windowsinformationprotectionconfiguration?view=graph-rest-beta) |
|追加|ベータ版|新しい複合型を追加しました。 <br/> [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta)<br/>[enterpriseCloudResource](/graph/api/resources/intune-deviceconfig-enterprisecloudresource?view=graph-rest-beta)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-beta)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-beta)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-beta)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)<br/>[iPv6Range](/graph/api/resources/intune-deviceconfig-ipv6range?view=graph-rest-beta)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRule](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprule?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruleapplockerpolicyfiletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruledesktoptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprulestoreapptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionCorporateNetworkLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectioncorporatenetworklocation?view=graph-rest-beta)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocation?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisecloudresources?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv4ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv6ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationneutralresources?view=graph-rest-beta)
|削除|ベータ版|次の複合型を削除し、microsoft.graph.Json に置き換えました。<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|変更|ベータ版|次のエンティティで、プロパティの種類 appConfigComplianceStatus を complianceStatus に置き換えました。 <br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta)|
|変更|ベータ版|リソース [managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-beta) について、プロパティ コンテンツの種類を managedAppSummary から Json に変更しました。|
|変更|ベータ版|GetUsersWithFlaggedAppRegistration 関数を [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) コレクションから削除しました。|
|変更|ベータ版|[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) エンティティの **vppToken** ナビゲーション プロパティは、包含されるコレクションではなくなりました。|
|変更|ベータ版|**deviceStatusOverview** プロパティが、[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) エンティティと [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) エンティティに追加されました。|
|変更|ベータ版|**appReportingOverview** プロパティが [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) シングルトンに追加されました。|
|変更|ベータ版|**deviceDisplayName** および **userPrincipalName** プロパティが、[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta)、[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta)、[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) の各エンティティに追加されました。|
|変更|ベータ版|**ruleName** プロパティが [deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-beta) エンティティに追加されました。|
|変更|ベータ版|**devicesCount**、**userDisplayName**、**userPrincipalName** の各プロパティが、[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-beta)、[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-beta)、[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta) の各エンティティに追加されました。|
|変更|ベータ版|[notificationMessageTemplates](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) コレクションが [deviceManagement](/graph/api/resources/intune-deviceconfig-devicemanagement?view=graph-rest-beta) シングルトンに追加されました。|
|変更|ベータ版|**isDefault**、**lastModifiedDateTime**、**locale**、**messageTemplate**、**subject** の各プロパティが [localizedNotificationMessage](/graph/api/resources/intune-deviceconfig-localizednotificationmessage?view=graph-rest-beta) エンティティに追加されました。|
|変更|ベータ版|**azureActiveDirectoryDeviceId**、**deviceCategory**、**deviceRegistrationState**、**managementAgent** の各プロパティが [managedDevice](/graph/api/resources/intune-onboarding-manageddevice?view=graph-rest-beta) エンティティに追加されました。|
|変更|ベータ版|**lastModifiedDateTime** プロパティが [mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-beta) エンティティに追加されました。|
|変更|ベータ版|**brandingOptions**、**defaultLocale**、**displayName**、**fromEmailAddress**、**lastModifiedDateTime**、**localizedNotificationMessages** の各プロパティが [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) エンティティに追加されました。|
|変更|ベータ版|**appsAllowTrustedAppsSideloading**、**appsBlockWindowsStoreOriginatedApps**、**developerUnlockSetting**、**edgeBlockAccessToAboutFlags**、**edgeBlockDeveloperTools**、**edgeBlockExtensions**、**edgeBlockInPrivateBrowsing**、**edgeFirstRunUrl**、**edgeHomepageUrls**、**gameDvrBlocked**、**settingsBlockAddProvisioningPackage**、**settingsBlockChangeLanguage**、**settingsBlockChangePowerSleep**、**settingsBlockChangeRegion**、**settingsBlockChangeSystemTime**、**settingsBlockEditDeviceName**、**settingsBlockRemoveProvisioningPackage**、**sharedUserAppDataAllowed**、**smartScreenBlockPromptOverride**、**smartScreenBlockPromptOverrideForFiles**、**storageRestrictAppDataToSystemVolume**、**storageRestrictAppInstallToSystemVolume**、**webRtcBlockLocalhostIpAddress**、**windowsStoreBlockAutoUpdate**、**windowsStoreEnablePrivateStoreOnly** の各プロパティが、[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) エンティティに追加されました。|

## <a name="december-2016"></a>2016 年 12 月

### <a name="delta-query"></a>デルタ クエリ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [デルタ クエリ](delta-query-overview.md)を実行するため、以下のエンティティに新しいデルタ関数が追加されました。<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>例については、以下をご覧ください。<br/>[グループへの増分の変更を取得する (プレビュー)](delta-query-groups.md)<br/>[フォルダー内のメッセージへの増分の変更を取得する (プレビュー)](delta-query-messages.md)<br/>[ユーザーへの増分の変更を取得する (プレビュー)](delta-query-users.md) |

### <a name="excel-apis"></a>Excel API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | workbookPivotTable リソース、pivotTables の refresh および refreshAll アクション、workbookRangeView リソース、フィルターされた範囲に対して実行して workbookRangeView をユーザーに返す visibleView アクション、visibleView からの行コレクションと範囲リソースの取得、範囲リソースからの columnsAfter、columnsBefore、resizedRange、rowsAbove、rowsBelow 関数、および新しいテーブル プロパティが追加されました。 |

### <a name="intune-apis"></a>Intune API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Microsoft Intune に、リソースとメソッド API が追加されました。これには、Azure ポータルでの Intune のパブリック プレビューをサポートする多数のリソースとメソッドのセットが含まれます。Intune サービスの詳細については、[Intune のドキュメント](https://go.microsoft.com/fwlink/?linkid=836405) をご覧ください。Intune のリソースと API の詳細については、「[Microsoft Graph での Intune の使用](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)」をご覧ください。 |

## <a name="october-2016"></a>2016 年 10 月

### <a name="authorization-provider"></a>認証プロバイダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | v2.0 認証エンドポイントでは、[ビジネス シナリオでのデーモン プロセスおよび長時間実行プロセス](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)で使える client_credentials OAuth 許可がサポートされるようになりました。 |
| 追加        | v1.0 およびベータ版 | v2.0 認証エンドポイントでは、[管理者の同意エンドポイント](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions)経由で、[管理者の同意を必要とするアクセス許可のスコープ](permissions-reference.md)がサポートされるようになりました。 |
| 追加        | v1.0 およびベータ版 | v2.0 認証エンドポイントでは、[管理者の同意エンドポイント](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions)経由で、テナント内のすべてのユーザーに対する管理者の同意がサポートされるようになりました。 |

### <a name="invitation-apis"></a>招待 API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 招待エンティティの型に、招待するユーザー (**ゲスト**または**メンバー**) の種類を定義する invitedUserType プロパティが追加されました。 |
| 削除        | ベータ版        | 2016 年 11 月 11 日付けで、招待のエンティティ型から invitedToGroups プロパティが削除されます。このため、この API を使用して、招待したユーザーをグループに追加することができなくなります。代わりに、[メンバー追加 API](/graph/api/group-post-members?view=graph-rest-1.0) を使ってユーザーをグループに追加することになります。 |

## <a name="september-2016"></a>2016 年 9 月

### <a name="azure-ad-application-proxy"></a>Azure AD アプリケーション プロキシ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Azure AD アプリケーション プロキシ API が、Microsoft Graph ベータ エンドポイントで利用可能になりました。これらの API では、アクセスのための共通のコントロール プレーンとして Azure AD を使用し、企業ネットワーク外のユーザーにオンプレミス アプリケーションをセキュアに発行できます。発行された API を使用すると、アプリケーションの _connectors_、_connectorGroups_、_onPremisesPublishing_ の設定など、アプリケーション プロキシのさまざまな側面を取得、更新するアプリケーションを作成できます。 |

### <a name="drive"></a>ドライブ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | shareId または共有 URL により共有されている driveItems にアクセスできる _shared_ コレクションが追加されました。 |
| 追加        | ベータ版        | ドライブに _search_ 関数が追加され、ドライブのルート フォルダー内の項目だけを検索するよりも多くの項目を検索できるようになりました。 |


### <a name="driveitem"></a>DriveItem

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _createUploadSession_ のサポートが追加され、OneDrive、OneDrive for Business、SharePoint のドキュメント ライブラリに 4 MB を超えるファイルをアップロードできるようになりました。 |
| 追加        | ベータ版        | SharePoint に保存されている driveItems の従来の SharePoint API 識別子を返す、driveItem に _sharepointIds_ プロパティが追加されました。 |
| 追加        | ベータ版        | _remoteItem_ に他のプロパティが追加されました。 |
| 追加        | ベータ版        | OneDrive for Business のファイルに対して _quickXorHash_ 値が追加されました。 |
| 追加        | ベータ版        | _createSharingLink_ にスコープが追加され、会社の共有可能なリンクまたは匿名の共有リンクが作成できるようになりました。 |

### <a name="extended-properties"></a>拡張プロパティ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [拡張プロパティ](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0)が、次のリソースでサポートされるようになりました: message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post。 |

### <a name="groups"></a>グループ

パブリック プレビューの API により、動的グループ メンバーシップのサポートが追加されました。追加された内容の一部を、次の表に記載します。

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | グループが動的グループの場合に、このグループのメンバーシップを制御する規則を含む、**membershipRule** プロパティが追加されました。 |
| 追加        | ベータ版        | このグループに対する動的メンバーシップの処理が実行中または一時停止中であるかどうかを制御するための **membershipRuleProcessingState** プロパティが追加されました。 |
| 追加        | ベータ版        | **"DynamicMembership"** を含むように **groupTypes** プロパティを設定して、このグループの動的グループ機能を強化できます。 |
| 追加        | ベータ版        | Office 365 グループの優先言語を示すための **preferredLanguage** プロパティが追加されました。 |
| 追加        | ベータ版        | Office 365 グループの色のテーマを指定するための **theme** プロパティが追加されました。 |

### <a name="hybrid-deployment-support"></a>ハイブリッド展開のサポート

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | アプリで v1.0 Outlook メール、カレンダー、連絡先の API を使用して、Exchange 2016 累積的な更新プログラム 3 (CU3) を使用したハイブリッド展開のオンプレミスのメールボックスにアクセスできます。REST API サポートの詳細については、特定の[ハイブリッド展開](hybrid-rest-support.md)をご覧ください。**注:** v1.0 のこれらの API セットを使用している場合、特定のハイブリッド展開の要件を満たすオンプレミスのメールボックスで機能する、運用アプリを含むアプリを検出できるようになりました。この機能はプレビューでのみ使用できます。 |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | 2 つの場所のプロパティの型が identityRiskEvents エンドポイントの新しい複合型で置き換えられるスキーマ変更の一環として、次のプロパティが identityRiskEvents エンドポイントで変更/追加されました。</br>**location** は Edm.String から ComplexType signInLocation に変更されました。<br/>**previousLocation** は Edm.String から ComplexType signInLocation に変更されました。<br/>**signInLocation** は、city、state、countryOrRegion、geoCoordinates プロパティを含む新しい ComplexType です。<br/>**geoCoordinates** は latitude と longitude プロパティを含む新しい ComplexType です。 |

### <a name="invitation-manager"></a>招待マネージャー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 招待マネージャー API が、Microsoft Graph ベータ エンドポイントで利用可能になりました。招待マネージャー API を使用して、組織に外部ユーザーを追加するための招待状を作成します。招待の一環として、招待されたユーザーを Office 365 グループに追加することも選択できます。詳細については、[招待マネージャー](/graph/api/resources/invitation?view=graph-rest-beta)をご覧ください。 |

### <a name="onedrive"></a>OneDrive

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | **driveItem** の **CreateUploadSession** メソッドが追加され、サイズの大きなファイルの再開可能なアップロードができるようになります。 |
| 追加        | v1.0        | SharePoint から項目の SharePoint ID を追跡する複数のプロパティ (**sharepointIds**) と、ルート フォルダーを識別する 1 つのプロパティ (**root**) が追加されました。 |
| 追加        | v1.0        | **Shares** ルート コレクションが追加されました。shareIds または共有リンクとともに使用して、OneDrive と SharePoint の共有項目にアクセスできます。新しい型 sharedDriveItem を返します。 |
| 追加        | v1.0        | driveItem の **Invite** メソッドが追加されました。項目へのアクセス許可を追加できます。 |
| 追加        | v1.0        | ドライブの **Search** メソッドが追加されました。ドライブ内の項目と共有された項目を対象とした検索が可能です。 |
| 追加        | v1.0        | ファイル複合型の **processingMetadata** プロパティ、ハッシュ複合型の quickXorHash プロパティが追加されました。 |
| 追加        | v1.0        | ハッシュ複合型の **quickXorHash** プロパティが追加されました。 |

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | **onlineMeetingUrl** プロパティが、[event](/graph/api/resources/event?view=graph-rest-1.0) リソースに追加されました。 |
| 追加        | ベータ版        | event リソースに [forward](/graph/api/event-forward?view=graph-rest-beta) アクションが追加されました。 |
| 追加        | ベータ版        | カレンダーの共有をサポートする次のプロパティが、[calendar](/graph/api/resources/calendar?view=graph-rest-beta) リソースに追加されました: **canEdit**、**canShare**、**canViewPrivateItems**、**isShared**、**isShareWithMe**、**owner**。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) 複合型が追加されました。これには **automaticRepliesSetting**、**timeZone**、**language** プロパティが含まれています。 |
| 追加        | v1.0        | **mailboxSettings** プロパティが [user](/graph/api/resources/user?view=graph-rest-1.0) リソースに追加されました。 |
| 追加        | ベータ版        | メッセージに含まれる[参照投稿](/graph/api/resources/mention?view=graph-rest-beta)の 1 つ以上のインスタンスを作成、一覧表示、取得、削除する機能のサポートが追加されました。参照投稿は、他のユーザーの注意を引きつけるためのメッセージ内のコールアウトをサポートしています。 |
| 追加        | ベータ版        | [getMailTips](/graph/api/user-getmailtips?view=graph-rest-beta) アクションのサポートが追加され、特定の受信者のすべてのメール ヒントを取得できるようになりました。 次のリソースが追加されました: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-beta)、[mailTips](/graph/api/resources/mailtips?view=graph-rest-beta)、[mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-beta)。 |

### <a name="query-parameters"></a>クエリ パラメーター

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | 2016 年 9 月 26 日現在、$ プレフィックスなしのクエリ パラメーターがサポートされています。クエリ パラメーターの $ プレフィックスは、省略可能です。詳細については、ブログ投稿「[Microsoft Graph における $ プレフィックスのないクエリ パラメーターのサポート](https://dev.office.com/queryparametersinMicrosoftGraph)」をご覧ください。 |

### <a name="sharepoint"></a>SharePoint

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | SharePoint サイトへのアクセスと、[ID ごとの一覧表示](/graph/api/list-get?view=graph-rest-beta) または [パス/URL](/graph/api/baseitem-getbyurl?view=graph-rest-beta) ごとの一覧表示が可能になりました。 |
| 追加        | ベータ版        | [listItem のインスタンスを一覧表示、作成、取得、削除](/graph/api/resources/listitem?view=graph-rest-beta)できるようになりました。 |

### <a name="users"></a>ユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 更新トークンまたはセッション トークンの有効期間の開始時期を示す、読み取り専用の **refreshTokensValidFromDateTime** プロパティが追加されました。この日時より前に発行されたすべてのトークンは無効になります。また、これらのトークンを使用しようとすると、ユーザーは新たにサインインを強制されます。 |
| 追加        | ベータ版        | Outlook のグローバル アドレス一覧にこのユーザーを含める必要があるかどうかを制御するための **showInAddressList** プロパティが追加されました。 |
| 追加        | ベータ版        | **invalidateAllRefreshTokens** サービス アクションが追加されました。これを使って **refreshTokensValidFromDateTime** ユーザー プロパティを現在の日時にリセットすることで、アプリケーションに発行されたすべての更新トークンとセッション トークンが無効になります。 |


### <a name="webhooks"></a>Webhooks

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 購読可能なリソースとしてドライブのルート項目が Webhooks に追加されました。 |

## <a name="august-2016"></a>2016 年 8 月

### <a name="contacts"></a>連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | いくつかのプロパティが削除され、対応するコレクションが連絡先エンドポイントに追加されたスキーマ変更の一環として、次のプロパティが連絡先エンドポイントに追加されました。_Websites Collection(ComplexType:Website)_、_Phones Collection (ComplexType:Phone)_、_PostalAddress Collection(ComplexType:PhysicalAddress)_。詳細については、ブログ投稿「[連絡先および People API で今後予定されている変更](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/)」をご覧ください。 |
| 削除        | ベータ版        | いくつかのプロパティが削除され、対応するコレクションが連絡先エンドポイントに追加されたスキーマ変更の一環として、次のプロパティが連絡先エンドポイントから削除されました。_BusinessHomePage_、_HomePhones_、_MobilePhone1_、_BusinessPhones_、_HomeAddress_、_BusinessAddress_、_OtherAddress_。詳細については、ブログ投稿「[連絡先および People API で今後予定されている変更](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/)」をご覧ください。 |

### <a name="excel-apis"></a>Excel API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | Microsoft Graph の Excel REST API は一般公開されています。Office 365 の Excel ブックとの充実した高度な統合を構築できるようになりました。詳細については、ブログ投稿「[Microsoft Graph の新しい Excel REST API を使ってアプリをパワーアップする](https://developer.microsoft.com/office/blogs/power-your-apps-with-the-new-excel-rest-api/)」をご覧ください。 |

### <a name="people"></a>複数のユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | _WebSite_ プロパティの名前が _Websites_ に変更されました。詳細については、「[連絡先および People API で今後予定されている変更](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/)」をご覧ください。 |

### <a name="privileged-identity-management"></a>Privileged Identity Management

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Privileged Identity Management (PIM) REST API が Microsoft Graph ベータ エンドポイントで利用可能になりました。[Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) では、グローバル管理者、課金管理者など、Azure AD の組織内でのロールのジャスト イン タイム アクティベーションが提供されます。発行された API を使用すると、特権ロールの割り当てを取得、更新して、ユーザーをロールにアクティブ化するアプリケーションを作成できます。詳細については、「[Microsoft Graph:ベータ版で利用可能な Azure AD Privileged Identity Management Preview API](https://developer.microsoft.com/office/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta/)」と「[Azure AD Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta)」を参照してください。 |

## <a name="july-2016"></a>2016 年 7 月

### <a name="administrative-units"></a>管理単位

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しい管理単位のプレビュー API が導入されました。管理単位を使用すると、組織は Azure Active Directory を分割して、サブ部門に管理職務を委任できます。サブ部門は、地域、部署、コスト センターなどを表すことができます。これを Microsoft Graph API から管理できるようになりました。 |

## <a name="june-2016"></a>2016 年 6 月

### <a name="identityriskevents"></a>IdentityRiskEvents

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:-----------|:--------------|
|追加|ベータ版|新しい IdentityRiskEvents プレビュー API が導入されました。この API は、Azure Active Directory Identity Protection と連携して動作します。この API を使うと、Identity Protection によって生成されたリスク イベントに対してクエリを実行できます。詳細については、ブログ投稿「[Microsoft Graph の新しいプレビュー API の紹介:IdentityRiskEvents](https://developer.microsoft.com/office/blogs/identityriskevents-api-preview/)」をご覧ください。

### <a name="subscriptions"></a>サブスクリプション

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _メール_と_連絡先_のサブスクリプションに対して、アプリ専用スコープがサポートされるようになりました。 |

## <a name="may-2016"></a>2016 年 5 月

### <a name="calendar"></a>カレンダー

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:-----------|:--------------|
|重大な変更|ベータ版|findMeetingTimes API に対する変更です。 詳細については、ブログ投稿「[Microsoft Graph findMeetingTimes API update](https://dev.office.com/microsoft-graph-findmeetingtimes-api-update)」 (Microsoft Graph findMeetingTimes API の更新) をご覧ください。 この変更は、2016 年 5 月 19 日に有効になりました。

### <a name="contact"></a>連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | _extensions_ が追加されました。これは OData v4 のオープン型 openTypeExtension をサポートする抽象型です。 |

### <a name="directory"></a>ディレクトリ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 重大な変更 | ベータ版        | _settingTemplateId_ は _templateId_ に名前が変更されます。この変更は、2016 年 5 月 19 日に有効になります。 |

### <a name="event"></a>イベント

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | _extensions_ が追加されました。これは OData v4 のオープン型 openTypeExtension をサポートする抽象型です。 |

### <a name="eventmessages"></a>EventMessages

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | _inferenceClassification_ と _extensions_ が _eventMessages_ に追加されました。 |
| 追加        | ベータ版        | _responseRequested_ が _eventMessageRequest_ に追加されました。 |

### <a name="messages"></a>メッセージ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | _inferenceClassification_ と _extensions_ が _messages_ に追加されました。 |
| 追加        | ベータ版        | _wellknownname_ が _contactFolder_ に追加されました。 |

### <a name="post"></a>投稿

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | _extensions_ が追加されました。これは OData v4 のオープン型 openTypeExtension をサポートする抽象型です。 |

### <a name="user"></a>ユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | _inferenceClassification_ リソースの種類が追加されました。 |
| 追加        | ベータ版        | _timeZone_ が _mailboxsettings_ に追加されました。   |
| 追加        | ベータ版        | API _findMeetingTimes_ が _user_ に追加されました。   |

## <a name="april-2016"></a>2016 年 4 月

### <a name="general"></a>全般

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | _Accept-Encoding:gzip_ の使用のサポートが追加されました。 |
| 追加        | v1.0          | 拡張パスのキャスト セグメントのサポートが追加されました。 たとえば、'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event' です。 |
| 追加        | ベータ版          | 構造プロパティに対する PATCH 要求のサポートが追加されました。例:'PATCH /me/mailboxSettings'。 |
| 追加        | ベータ版          | たとえば、ユーザーがメールボックスのライセンスを持っていない場合、またはテナントに Exchange Online のサブスクリプションがない場合など、Outlook が要求を処理できないときに、Azure Active Directory が /beta/users/id/photo 要求のフォールバックとして使用されるようになりました。注: このフォールバックは GET と PATCH の両方に使用できます。 |
| 追加        | ベータ版          | 拡張パスのキャスト セグメントのサポートが追加されました。 たとえば、'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event' です。 |

### <a name="onedrive"></a>OneDrive

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 修正プログラム             | v1.0        | 500 エラーと「拡張プロパティの型がサポートされていません」というエラーで OneDrive の createLink 要求が失敗する問題が修正されました。 |

## <a name="march-2016"></a>2016 年 3 月

### <a name="calendar"></a>カレンダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _singleValueExtendedProperties_ プロパティと _multiValueExtendedProperties_ プロパティが追加されました。 |
| 追加        | ベータ版        | _suggestionHint_ プロパティが _meetingTimeCandidate_ に追加されました。 |
| 追加        | ベータ版        | _locationUri_ プロパティが _location_ に追加されました。 |
| 追加        | ベータ版        | _type_ と _postOfficeBox_ が _physicalAddress_ に追加されました。 |
| 変更          | ベータ版        | _findMeetingTimes_ で新しいパラメーター _ReturnSuggestionHints_ を使用するようになりました。 |
| 変更          | ベータ版        | _findMeetingTimes_ が _meetingTimeCandidate_ のコレクションを返すようになりました。 |

### <a name="drive"></a>ドライブ

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | サインインしたユーザーによって最近使用された項目のセットを一覧表示する _recent_ 関数が追加されました。この一覧には、ユーザーのドライブにある項目と、他のドライブとの間でアクセス可能な項目が含まれています。例: GET /me/drive/recent。 |
| 追加        | v1.0 およびベータ版 | 現在のユーザーと共有されている項目のセットを一覧表示する _sharedWithMe_ 関数が追加されました。例: GET /me/drive/sharedWithMe。 |

### <a name="driveitem"></a>DriveItem

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | 別のドライブ内の項目へのリンクを提供する _remoteItem_ 型が追加されました。 |
| 追加        | v1.0 およびベータ版 | このアクセス許可に関連付けられた共有の招待に関する詳細情報を提供する _sharingInvitation_ 型が追加されました。 |
| 追加        | v1.0 およびベータ版 | ドライブ内の項目に対する変更を追跡する _delta_ 関数が追加されました。例: GET /me/drive/items/{item-id}/delta |
| 追加        | v1.0 およびベータ版 | 新しい親の下に、または新しい名前を指定して、_driveItem_ (すべての子を含む) のコピーを作成する _copy_ が追加されました。例: POST /me/drive/items/{item-id}/copy。 |
| 追加        | v1.0 およびベータ版 | _conflictBehavior_ インスタンス属性が _driveItem_ に適用されるようになりました。 |
|追加|ベータ版|既存の項目に共有の招待を送信する _invite_ 関数が追加されました。共有の招待では、一意の共有リンクが作成され、共有リンクを記載した電子メールが招待状の受信者に送信されます。例: POST /drive/items/{item-id}/invite。

### <a name="event"></a>イベント

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいプロパティ _onlineMeetingUrl_ と、新しいメソッド _cancel_ が追加されました。 |

### <a name="event-messages"></a>イベント メッセージ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _startDateTime_、_endDateTime_、_location_、_type_、_recurrence_、_isOutOfDate_、_conversationIndex_、_unsubscribe_、_unsubscribeData_、_unsubscribeEnabled_、_flag_ プロパティが、_eventmessage_ オブジェクトに追加されました。 |
| 追加        | ベータ版        | _singleValueExtendedProperties_ プロパティと _multiValueExtendedProperties_ プロパティが追加されました。 |
| 追加        | ベータ版        | 新しいメソッド _unsubscribe_ が追加されました。          |

### <a name="excel"></a>Excel

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 現在、Excel ブックのデータの読み取りと変更が可能な新しい Excel REST API を追加しているところです。データへのインサイトを提供することで、ユーザーが Excel ブックに保存されているコンテンツから価値を取得できるスマート アプリを構築できるようになりました。Excel の分析機能の活用、表とグラフの作成、および視覚に訴えるグラフ イメージの抽出などを、アプリ内からすべて実行できます。詳細については、「[Microsoft Graph での Excel の操作](/graph/api/resources/excel?view=graph-rest-beta)」をご覧ください。 |

### <a name="general"></a>全般

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | テナント エイリアスと拒否された JWT (AAD) トークンを解決するときのエラー メッセージを改善しました。 |
| 追加        | v1.0 およびベータ版 | 空のベアラー トークンで要求を受信した場合に、承認サービス エンドポイントの場所が _www-authenticate_ ヘッダー内に返されるようになりました。 |
| 追加        | v1.0 およびベータ版 | エンティティの ID プロパティでのフィルター機能が修正されました。 例: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>以前は、サービスのアクションと関数に対する POST 要求で、アクション名または関数名に microsoft.graph のプレフィックスを付ける必要がありました。 例: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups<br/>プレフィックスは不要になりました (ただし、引き続き指定できます)。 そのため、次のような指定でも機能するようになりました。POST https://graph.microsoft.com/v1.0/me/getMemberGroups |
| 変更          | ベータ版          | サブスクリプションのプロパティ名がクリーンアップされました。  |
| 追加        | ベータ版          | エンティティとその関連機能の既定の動作を (_directorySettingTemplates_ 経由で) 検出し、(テンプレートから _setting_ を作成することにより) 上書きする機能が追加されました。最初に提供されたこの唯一のテンプレートは、Office グループ上での動作を制御するためのものです。 |

### <a name="mail-folder"></a>メール フォルダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _wellKnownName_ プロパティと _userConfigurations_ プロパティが追加されました。 |
| 追加        | ベータ版        | _singleValueExtendedProperties_ プロパティと _multiValueExtendedProperties_ プロパティが追加されました |

### <a name="messages"></a>メッセージ

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0          | _mobilePhone_ プロパティが追加されました。            |
| 追加        | v1.0 およびベータ版 | _internetMessageId_ プロパティが追加されました。メッセージ ID は、[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式です。 |
| 変更          | ベータ版          | _mobilePhone1_ プロパティは _mobilePhone_ に名前が変更されました。 |
| 変更          | ベータ版          | _createReply_ と _createReplyAll_ は、新しいパラメーター _Message_ および _comment_ を使用します。 |
| 変更          | ベータ版          | _createForward_ は、新しいパラメーター _Message_、_ToRecipients_、_comment_ を使用します。 |
| 変更          | ベータ版          | _reply_、_replyAll_、_forward_ は、新しいパラメーター _Message_ を使用します。 |

### <a name="permission"></a>アクセス許可

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | このアクセス許可に関連付けられた共有の招待の詳細情報を提供する _sharingInvitation_ プロパティが追加されました。 |

### <a name="person"></a>人物

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいプロパティ _birthday_、_personNotes_、_isFavorite_、_phones_、_permission_、_postalAddresses_、_websites_、_yomiCompany_、_department_、_profession_、_mailboxType_、_personType_ が追加されました。 |
| 追加        | ベータ版        | 新しい列挙型 _physicalAddressType_、_webSite_、_phone_、_webSiteType_ が追加されました。 |

### <a name="reference-attachment"></a>参照添付ファイル

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいプロパティ _sourceUrl_、_providerType_、_thumbnailUrl_、_previewUrl_、_permission_、_isFolder_ が追加されました。 |
| 追加        | ベータ版        | _singleValueExtendedProperties_ プロパティと _multiValueExtendedProperties_ プロパティが追加されました。 |
| 追加        | ベータ版        | 新しい列挙型 _referenceAttachmentProvider_ と _referenceAttachmentPermission_ が追加されました。 |

### <a name="subscriptions"></a>サブスクリプション

| **変更の種類** | **エンドポイント** | **説明**                          |
| :-------------- | :----------- | :--------------------------------------- |
| 追加        | v1.0         | Webhook が、_/Subscriptions_ リソースから v1.0 エンドポイントで一般公開されるようになりました。 Outlook と Office 365 のグループ会話からデータに関する通知を受信するためのサブスクリプションを作成、読み取り、更新、削除します。 |

### <a name="user"></a>ユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _mailboxSettings_ プロパティおよび対応する型が追加されました。 |

## <a name="february-2016"></a>2016 年 2 月

### <a name="driveitem"></a>DriveItem

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | Microsoft アカウントに対する driveItem の新しい _remoteItem_ プロパティ。 |

### <a name="general"></a>全般

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | -_/me/drive_ が、Microsoft アカウントおよび職場と学校のアカウントの両方で機能するようになりました。 |
| 変更          | v1.0 およびベータ版 | OneDrive ストレージがオンデマンドでプロビジョニングされたアカウントの Drive 要求は、動作の信頼性がより高くなり、テナントの既定の SharePoint サイトで非標準の名前が使用されるような、より多くのシナリオで動作します。 |
| 削除        | ベータ版          | 1.0 スキーマにより厳密に一致するように、実装されていないさまざまな型がベータ スキーマから削除されました。 |

### <a name="subscriptions"></a>サブスクリプション

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | サブスクリプション作成時の notificationUrl 検証。詳細については、「[Microsoft Graph の WebHooks の更新 - 2016 年 1 月](https://developer.microsoft.com/office/blogs/Microsoft-Graph-WebHooks-Update-January-2016/)」をご覧ください。 |
| 追加        | ベータ版        | サブスクリプション エンティティを削除できるようになりました。DELETE https://graph.microsoft.com/beta/subscriptions/ |

### <a name="users"></a>ユーザー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | Microsoft アカウントに対して _displayName_ が返されるようになりました。 |

## <a name="january-2016"></a>2016 年 1 月

### <a name="contacts"></a>連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | mobilePhone プロパティが個人用連絡先エンティティ セットに追加されました。 |

### <a name="directoryobjects"></a>directoryObjects

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正プログラム             | v1.0 およびベータ版 | directoryObjects にバインドされている呼び出しアクションが修正されました。このアクションは次のエラーで失敗していました。操作からの戻り値の型は、指定したエンティティ セットで使用できません。これは、次のアクションに適用されます: _microsoft.graph.checkMemberObjects_、_microsoft.graph.getMemberObjects_、_microsoft.graph.checkMemberGroups_、_microsoft.graph.assignLicense_、_microsoft.graph.changePassword_。 |

## <a name="december-2015"></a>2015 年 12 月

### <a name="contacts"></a>連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | mobilePhone プロパティが個人用連絡先エンティティ セットに追加されました。 |

### <a name="general"></a>全般

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正プログラム             | v1.0 およびベータ版 | 同じプロパティを複数回指定した $filter 式を使用する要求が修正されました。この要求は次の 500 エラーで失敗していました。同じキーを持つ項目が既に追加されています。 |
| 修正プログラム             | v1.0 およびベータ版 | アクション パラメーターの名前と値で大文字と小文字が区別されない問題を修正しました。 |
| 修正             | v1.0 およびベータ版 | 一部の埋め込み複合プロパティに null 値を含むペイロードの要求処理を修正しました。この要求は null 参照の例外で失敗していました。 |
| 追加        | v1.0 およびベータ版 | 複合型プロパティの並べ替えとフィルター処理のサポートが追加されました。 |
| 追加        | v1.0 およびベータ版 | 401 応答の www-authenticate ヘッダーに authorization_uri プロパティが追加されました。この URI は、トークンの取得フローを開始するために使用できます。 |
| 追加        | v1.0 およびベータ版 | ユーザーとグループ全体でエラー メッセージが改善されました。 |

### <a name="groups"></a>グループ

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正プログラム             | v1.0 およびベータ版 | 次のグループ アクションの呼び出しを修正しました: _microsoft.graph.addFavorite_、_microsoft.graph.removeFavorite_、_microsoft.graph.resetUnseenCount_。 |

### <a name="messages"></a>メッセージ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | eventMessage の eventMessageRequest サブタイプと、startDateTime、endDateTime、location、type、recurrence、isOutOfDate プロパティが、eventMessage 型に追加されました。 |

### <a name="users"></a>ユーザー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正プログラム             | v1.0 およびベータ版 | ユーザー プリンシパル名 (UPN) でユーザーを参照する場合に、他のユーザーで特定のユーザー プロパティを選択できてしまう問題を修正しました。 例: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| 修正             | v1.0 およびベータ版 | ユーザーにバインドされた _microsoft.graph.reminderView_ 関数の呼び出しを修正しました。この呼び出しは次のエラーで失敗していました。Microsoft.OutlookServices.Reminder 型で businessPhones という名前のプロパティは見つかりませんでした。 |
| 修正プログラム             | v1.0 およびベータ版 | 400 エラーで失敗していた、ユーザーの作成と更新 (POST/PATCH /v1.0/users) を修正しました。 |
