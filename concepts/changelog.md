# <a name="changelog-for-microsoft-graph"></a>Microsoft Graph の変更ログ

この変更ログでは、Microsoft Graph と、v1.0 およびベータ版のエンドポイント Microsoft Graph API の変更内容について説明します。

Microsoft Graph API に関する既知の問題の詳細については、「[既知の問題](known_issues.md)」を参照してください。

## <a name="may-2018"></a>2018 年 5 月

### <a name="groups"></a>グループ

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | [post](../api-reference/v1.0/resources/post.md) エンティティに **importance** プロパティを追加しました。 |

### <a name="microsoft-bookings-api"></a>Microsoft Bookings API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [bookingBusiness](../api-reference/beta/resources/bookingbusiness.md) エンティティと次の CRUD メソッドおよび操作を追加しました。 <br> [List](../api-reference/beta/api/bookingbusiness_list.md) <br> [Create](../api-reference/beta/api/bookingbusiness_post_bookingbusinesses.md) <br> [Get](../api-reference/beta/api/bookingbusiness_get.md) <br> [Update](../api-reference/beta/api/bookingbusiness_update.md) <br> [Delete](../api-reference/beta/api/bookingbusiness_delete.md) <br> [Publish](../api-reference/beta/api/bookingbusiness_publish.md) <br> [Unpublish](../api-reference/beta/api/bookingbusiness_unpublish.md) <br> API の統合の詳細については、[Microsoft Bookings API](booking-concept-overview.md) を参照してください。 |
| 追加        | ベータ版          | [bookingAppointment](../api-reference/beta/resources/bookingappointment.md) エンティティと次の CRUD メソッドおよび操作を追加しました。 <br> [List](../api-reference/beta/api/bookingbusiness_list_appointments.md) <br> [Create](../api-reference/beta/api/bookingbusiness_post_appointments.md) <br> [Get](../api-reference/beta/api/bookingappointment_get.md) <br> [Update](../api-reference/beta/api/bookingappointment_update.md) <br> [Delete](../api-reference/beta/api/bookingappointment_delete.md) <br> [Cancel](../api-reference/beta/api/bookingappointment_cancel.md) |
| 追加        | ベータ版          | [bookingCurrency](../api-reference/beta/resources/bookingcurrency.md) エンティティと次のメソッドを追加しました。 <br> [List](../api-reference/beta/api/bookingcurrency_list.md) <br> [Get](../api-reference/beta/api/bookingcurrency_get.md) |
| 追加        | ベータ版          | [bookingCustomer](../api-reference/beta/resources/bookingcustomer.md) エンティティと次の CRUD メソッドを追加しました。 <br> [List](../api-reference/beta/api/bookingbusiness_list_customers.md) <br> [Create](../api-reference/beta/api/bookingbusiness_post_customers.md) <br> [Get](../api-reference/beta/api/bookingcustomer_get.md) <br> [Update](../api-reference/beta/api/bookingcustomer_update.md) <br> [Delete](../api-reference/beta/api/bookingcustomer_delete.md)|
| 追加        | ベータ版          | [bookingService](../api-reference/beta/resources/bookingservice.md) エンティティと次の CRUD メソッドを追加しました。 <br> [List](../api-reference/beta/api/bookingbusiness_list_services.md) <br> [Create](../api-reference/beta/api/bookingbusiness_post_services.md) <br> [Get](../api-reference/beta/api/bookingservice_get.md) <br> [Update](../api-reference/beta/api/bookingservice_update.md) <br> [Delete](../api-reference/beta/api/bookingservice_delete.md)|
| 追加        | ベータ版          | [bookingStaffMember](../api-reference/beta/resources/bookingstaffmember.md) エンティティと次の CRUD メソッドを追加しました。 <br> [List](../api-reference/beta/api/bookingbusiness_list_staffmembers.md) <br> [Create](../api-reference/beta/api/bookingbusiness_post_staffmembers.md) <br> [Get](../api-reference/beta/api/bookingstaffmember_get.md) <br> [Update](../api-reference/beta/api/bookingstaffmember_update.md) <br> [Delete](../api-reference/beta/api/bookingstaffmember_delete.md)|
| 追加        | ベータ版          | 次の複合型を追加しました。 <br> [bookingNamedEntity](../api-reference/beta/resources/bookingnamedentity.md) <br> [bookingPerson](../api-reference/beta/resources/bookingperson.md) <br> [bookingReminder](../api-reference/beta/resources/bookingreminder.md) <br> [bookingWorkHours](../api-reference/beta/resources/bookingworkhours.md) <br> [bookingWorkTimeSlot](../api-reference/beta/resources/bookingworktimeslot.md)|

### <a name="insights-api"></a>Insights API

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [settings](../api-reference/beta/resources/user_settings.md) エンティティと次の CRUD メソッドを追加しました。 <br> [Get](../api-reference/beta/api/user_get_settings.md) <br> [Update](../api-reference/beta/api/user_update_settings.md) |

## <a name="april-2018"></a>2018 年 4 月

### <a name="audit-log-api"></a>監査ログ API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい監査ログを API サポートするため、[directoryAudit](../api-reference/beta/resources/directoryaudit.md) および [signIn](../api-reference/beta/resources/signin.md) エンティティを追加しました。 |
|追加|ベータ版|監査ログ API をサポートするため、次のリソースを追加しました。[appIndentity](../api-reference/beta/resources/appidentity.md)、[auditActivityInitiator](../api-reference/beta/resources/auditactivityinitiator.md)、[conditionalAccessPolicy](../api-reference/beta/resources/conditionalaccesspolicy.md)、[deviceDetail](../api-reference/beta/resources/devicedetail.md)、[mfaDetail](../api-reference/beta/resources/mfadetail.md)、[modifiedProperty](../api-reference/beta/resources/modifiedproperty.md)、[signinLocation](../api-reference/beta/resources/signinlocation.md)、[signinStatus](../api-reference/beta/resources/signinstatus.md)、[targetResource](../api-reference/beta/resources/targetresource.md)、[targetResourceApp](../api-reference/beta/resources/targetresourceapp.md)、[targetResourceDevice](../api-reference/beta/resources/targetresourcedevice.md)、[targetResourceDirectory](../api-reference/beta/resources/targetresourcedirectory.md)、[targetResourceGroup](../api-reference/beta/resources/targetresourcegroup.md)、[targetResourceOther](../api-reference/beta/resources/targetresourceother.md)、[targetResourcePolicy](../api-reference/beta/resources/targetresourcepolicy.md)、[targetResourceRole](../api-reference/beta/resources/targetresourcerole.md)、[targetResourceServicePrincipal](../api-reference/beta/resources/targetresourceserviceprincipal.md)、[targetResourceUser](../api-reference/beta/resources/targetresourceuser.md)、[userIdentity](../api-reference/beta/resources/useridentity.md) |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [organization](../api-reference/v1.0/resources/organization.md) エンティティに **privacyProfile** 複合型を追加しました。 |
| 追加        | v1.0        | [user](../api-reference/v1.0/resources/user.md) エンティティに **legalAgeGroup、ageGroup、および consentProvidedForMinor** 複合型を追加しました。 |
| 追加        | v1.0        | [webhook](../api-reference/v1.0/resources/webhooks.md) 通知サブスクリプションにユーザーとグループのサポートを追加しました。 |
| 追加        | ベータ版        | [ディレクトリ (削除済みアイテム)](../api-reference/beta/resources/directory.md) リソースに[ユーザーが所有する削除済みアイテムの一覧表示](../api-reference/beta/api/directory_deleteditems_user_owned.md)アクションを追加しました | 

### <a name="education-apis"></a>教育機関 API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|変更|ベータ版|[educationsynchronizationerror](../api-reference/beta/resources/educationsynchronizationerror.md) に reportableIdentifier プロパティを追加しました。|
|変更|ベータ版|[uploadUrl](../api-reference/beta/api/educationsynchronizationprofile_uploadurl.md) API の応答オプションを更新しました。|
|変更|ベータ版|[educationSynchronizationError](../api-reference/beta/resources/educationsynchronizationerror.md) リソースの種類の説明テキストを更新しました。|
|変更|ベータ版|[同期エラー取得](../api-reference/beta/api/educationsynchronizationerrors_get.md) API の説明テキストを更新しました。|


### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[managedDeviceMobileAppConfigurationDeviceStatus](../api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)<br/>|
|追加|v1.0|新しい列挙型を追加しました。<br/>[managedDeviceOwnerType](../api-reference/v1.0/resources/intune_devices_manageddeviceownertype.md)<br/>|
|追加|v1.0|[managedDevice](../api-reference/v1.0/resources/intune_devices_manageddevice.md) エンティティに **managedDeviceOwnerType** プロパティを追加しました|
|追加|v1.0|[managedDeviceMobileAppConfiguration](../api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfiguration.md) エンティティに **deviceStatuses** ナビゲーション プロパティを追加しました|
|追加|v1.0|[policyPlatformType](../api-reference/v1.0/resources/intune_deviceconfig_policyplatformtype.md) 列挙型に **androidWorkProfile** メンバーを追加しました|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidWorkProfileCertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilecertificateprofilebase)<br/>[androidWorkProfileCustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilecustomconfiguration)<br/>[androidWorkProfileEasEmailProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofileeasemailprofilebase)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofileenterprisewificonfiguration)<br/>[androidWorkProfileGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration)<br/>[androidWorkProfileGmailEasConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilegmaileasconfiguration)<br/>[androidWorkProfileNineWorkEasConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilenineworkeasconfiguration)<br/>[androidWorkProfilePkcsCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilepkcscertificateprofile)<br/>[androidWorkProfileScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilescepcertificateprofile)<br/>[androidWorkProfileTrustedRootCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofiletrustedrootcertificate)<br/>[androidWorkProfileVpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilevpnconfiguration)<br/>[androidWorkProfileWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilewificonfiguration)<br/>[restrictedAppsViolation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_restrictedappsviolation)<br/>[windowsAutopilotDeploymentProfileAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofileassignment)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[managedDeviceModelsAndManufacturers](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevicemodelsandmanufacturers)<br/>[managedDeviceReportedApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevicereportedapp)<br/>[windowsEnrollmentStatusScreenSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_enrollment_windowsenrollmentstatusscreensettings)<br/>|
|追加|ベータ版|新しい列挙型を追加しました。<br/>[androidWorkProfileCrossProfileDataSharingType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype)<br/>[androidWorkProfileRequiredPasswordType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype)<br/>[androidWorkProfileVpnConnectionType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidworkprofilevpnconnectiontype)<br/>[bitLockerRecoveryInformationType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryinformationtype)<br/>[localSecurityOptionsInformationShownOnLockScreenType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_localsecurityoptionsinformationshownonlockscreentype)<br/>[managedAppRemediationAction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappremediationaction)<br/>[managedDeviceOwnerType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddeviceownertype)<br/>[restrictedAppsState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_restrictedappsstate)<br/>[windows10VpnProfileTarget](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnprofiletarget)<br/>|
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [playLostModeSound](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_playlostmodesound.md) アクションを追加しました |
|削除|ベータ版|次の列挙型を削除しました。<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|追加|ベータ版|[androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) エンティティに **workProfileBlockScreenCapture** および **workProfileBlockCrossProfileCallerId** プロパティを追加しました|
|追加|ベータ版|[androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティに **minimumWipePatchVersion**、**allowedAndroidDeviceManufacturers**、および **appActionIfAndroidDeviceManufacturerNotAllowed** プロパティを追加しました|
|追加|ベータ版|[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに **minimumWipeSdkVersion**、**minimumWipePatchVersion**、**allowedIosDeviceModels**、**appActionIfIosDeviceModelNotAllowed**、**allowedAndroidDeviceManufacturers**、および **appActionIfAndroidDeviceManufacturerNotAllowed** プロパティを追加しました|
|追加|ベータ版|[deviceComplianceDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) エンティティに **notApplicablePlatformCount** および **conflictCount** プロパティを追加しました|
|追加|ベータ版|[deviceConfigurationDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) エンティティに **notApplicablePlatformCount** および **conflictCount** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに **accountMoveCompletionDateTime** プロパティを追加しました|
|追加|ベータ版|[iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに **minimumWipeSdkVersion**、**allowedIosDeviceModels**、および **appActionIfIosDeviceModelNotAllowed** プロパティを追加しました|
|追加|ベータ版|[managedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) エンティティに **minimumWipeOsVersion**、**minimumWipeAppVersion**、**appActionIfDeviceComplianceRequired**、および **appActionIfMaximumPinRetriesExceeded** プロパティを追加しました|
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **managedDeviceOwnerType**、**preferMdmOverGroupPolicyAppliedDateTime**、**isAutopilotEnrolled**、および **requestUserEnrollmentApproval** プロパティを追加しました|
|追加|ベータ版|[managedDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddeviceoverview) エンティティに **managedDeviceModelsAndManufacturers** プロパティを追加しました|
|追加|ベータ版|[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティに **localSecurityOptionsMachineInactivityLimitInMinutes**、**localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**、**localSecurityOptionsInformationShownOnLockScreen**、**defenderSecurityCenterDisableAccountUI**、**defenderSecurityCenterDisableHardwareUI**、**defenderSecurityCenterDisableRansomwareUI**、**defenderSecurityCenterDisableSecureBootUI**、および **defenderSecurityCenterDisableTroubleshootingUI** プロパティを追加しました|
|追加|ベータ版|[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに **printerNames**、**printerDefaultName**、**printerBlockAddition**、および **searchBlockWebResults** プロパティを追加しました|
|追加|ベータ版|[windows10VpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration) エンティティに **profileTarget**、**enableAlwaysOn**、および **enableDeviceTunnel** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile) エンティティに **enrollmentStatusScreenSettings** プロパティを追加しました|
|追加|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに **deviceConfigurationRestrictedAppsViolations** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeploymentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsDomainJoinConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdomainjoinconfiguration) エンティティに **networkAccessConfigurations** ナビゲーション プロパティを追加しました|
|削除|ベータ版|[auditActor](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditactor) 複合型から **permissions** プロパティを削除しました|
|変更|ベータ版|[bitLockerRecoveryOptions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions) 複合型で次のプロパティの型を変更しました。<br/>**recoveryInformationToStore** の型を [bitLockerRecoveryinformationType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryinformationtype) から [bitLockerRecoveryInformationType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryinformationtype) に変更<br/>|
|追加|ベータ版|[deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型に **deviceInactivityBeforeRetirementInDay** プロパティを追加しました|
|追加|ベータ版|[intuneBrand](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_intunebrand) 複合型に **landingPageCustomizedImage** プロパティを追加しました|
|削除|ベータ版|[vpnServer](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver) 複合型から **ipAddressOrFqdn** プロパティを削除しました|
|削除|ベータ版|[windowsUpdateScheduledInstall](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdatescheduledinstall) 複合型から **restartMode** プロパティを削除しました|
|追加|ベータ版|[androidForWorkVpnConnectionType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconnectiontype) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[androidVpnConnectionType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidvpnconnectiontype) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[appleVpnConnectionType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_applevpnconnectiontype) 列挙型に **paloAltoGlobalProtect** メンバーを追加しました|
|追加|ベータ版|[policyPlatformType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_policyplatformtype) 列挙型に **androidWorkProfile** メンバーを追加しました|

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0          | **locations** プロパティを [event](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/event) エンティティに追加しました。これにより、出席者が複数の場所から出席できるイベントを開催できるようになりました。 |
| 追加        | v1.0          | **locationType** プロパティを [location](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/location) 複合型に追加しました。 |
| 追加        | v1.0          | **uniqueId** および **uniqueIdType** プロパティを [location](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/location) 複合型に追加しました。 これらのプロパティは、現時点では内部使用に限られます。 |


### <a name="outlook-contacts"></a>Outlook の連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0          | **flag** プロパティを [contact](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact) エンティティに追加しました。 共有 [followupFlag](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/followupflag) 複合型を追加しました。|


### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0          | **flag** プロパティを [message](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message) エンティティに追加しました。 共有 [followupFlag](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/followupflag) 複合型を追加しました。|
| 追加        | v1.0        | **internetMessageHeaders** プロパティを [message](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message) エンティティに追加しました。 |
| 追加        | v1.0        | [internetMessageHeader](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/internetmessageheader) 複合型を追加しました。 |
| 追加        | v1.0        | **messageRules** ナビゲーション プロパティを [mailFolder](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/mailfolder) エンティティに追加しました。 **messageRules** は [messageRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/messagerule) インスタンスのコレクションです。 |
| 追加        | v1.0        | [messageRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/messagerule) エンティティと、[messageRuleActions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/messageruleactions)、[messageRulePredicates](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/messagerulepredicates)、[sizeRange](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/sizerange) 複合型を追加しました。 |
| 追加        | v1.0        | メッセージ ルールに CRUD 操作 [create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/mailfolder_post_messagerules)、[list](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/mailfolder_list_messagerules)、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/messagerule_get)、[update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/messagerule_update)、[delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/messagerule_delete) を追加しました。 |
| 追加 | ベータ版 | [mailSearchFolder](../api-reference/beta/resources/mailsearchfolder.md) を追加しました。 |
| 追加 | ベータ版 | メール検索フォルダーのために次の API を追加しました: [作成](../api-reference/beta/api/mailsearchfolder_post.md)、[更新](../api-reference/beta/api/mailsearchfolder_update.md)。 |
| 変更 | ベータ版 | メール検索フォルダーのサポートを追加しました: [mailFolder の削除](../api-reference/beta/api/mailfolder_delete.md)、[mailFolder の取得](../api-reference/beta/api/mailfolder_get.md)、[子フォルダーの一覧表示](../api-reference/beta/api/mailfolder_list_childfolders.md)。 |


### <a name="outlook-user-choices"></a>Outlook ユーザーの選択

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しい **masterCategories** ナビゲーション プロパティを [outlookUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/outlookuser) エンティティに追加しました。 **masterCategories** は [outlookCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/outlookCategory) オブジェクトのコレクションです。 |
| 追加        | v1.0        | [outlookCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/outlookCategory) エンティティを追加しました。 |
| 追加        | v1.0        | [outlookCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/outlookCategory) に CRUD 操作 [create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/outlookuser_post_mastercategories)、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/outlookcategory_get)、[update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/outlookcategory_update)、[delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/outlookcategory_delete) を追加しました。 |
| 追加        | v1.0        | 新しい [supportedLanguages](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/outlookuser_supportedlanguages) 関数を [outlookUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/outlookuser) エンティティに追加しました。 |
| 追加        | v1.0        | 新しい [supportedTimeZones](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/outlookuser_supportedtimezones) 関数を [outlookUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/outlookuser) エンティティに追加しました。 |
|追加 | v1.0 | 新しい **workingHours** プロパティを [mailboxSettings](../api-reference/v1.0/resources/mailboxsettings.md) に追加しました。 サポートされるユース ケースについては、「[workingHours リソース タイプ](../api-reference/v1.0/resources/workinghours.md)」を参照してください。|
|追加 | v1.0 | 次の新しい複合型を追加しました。 <br> [workingHours](../api-reference/v1.0/resources/workinghours.md) <br> [timeZoneBase](../api-reference/v1.0/resources/timezonebase.md) <br> [customTimeZone](../api-reference/v1.0/resources/customtimezone.md) <br> [standardTimeZoneOffset](../api-reference/v1.0/resources/standardtimezoneoffset.md) <br> [daylightTimeZoneOffset](../api-reference/v1.0/resources/daylighttimezoneoffset.md)|


### <a name="microsoft-teams"></a>Microsoft Teams 

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい [teamMemberSettings](../api-reference/beta/resources/teamMemberSettings.md) エンティティを追加しました。|
|追加|ベータ版|新しい [teamGuestSettings](../api-reference/beta/resources/teamGuestSettings.md) エンティティを追加しました。|
|追加|ベータ版|新しい [teamMessagingSettings](../api-reference/beta/resources/teamMessagingSettings.md) エンティティを追加しました。|
|追加|ベータ版|新しい [teamFunSettings](../api-reference/beta/resources/teamFunSettings.md) エンティティを追加しました。|
|追加|ベータ版|新しい[チャネルの削除](../api-reference/beta/api/channel_delete.md)操作を追加しました。|
|追加|ベータ版|新しい[チャネルのパッチ適用](../api-reference/beta/api/channel_patch.md)操作を追加しました。|
|変更|ベータ版|[channel](../api-reference/beta/resources/channel.md) エンティティへのパスを更新しました。|


### <a name="project-rome-apis"></a>Project Rome API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加 | v1.0 | [Get recent activities API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/projectrome_get_recent_activities) を追加しました |
| 追加 | v1.0 | [Get activities API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/projectrome_get_activities) を追加しました |
| 追加 | v1.0 | [Upsert Activity](https://developer.microsoft.com/ja-JP/graph/docs/v1.0/api/projectrome_put_activity) を追加しました |
| 追加 | v1.0 | [Upsert HistoryItem](https://developer.microsoft.com/ja-JP/graph/docs/v1.0/projectrome_put_historyitem) を追加しました |
| 追加 | v1.0 | [Delete Activity](https://developer.microsoft.com/ja-JP/graph/docs/v1.0/projectrome_delete_activity) を追加しました |
| 追加 | v1.0 | [Upsert HistoryItem](https://developer.microsoft.com/ja-JP/graph/docs/v1.0/projectrome_delete_historyItem) を追加しました |
| 追加 | v1.0 | [activity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/projectrome_activity) を追加しました |
| 追加 | v.10 | [historyItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/projectrome_historyitem) を追加しました |
| 追加 | v1.0 | [visualInfo](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/projectrome_visualinfo) を追加しました |
| 追加 | v1.0 | [imageInfo](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/projectrome_imageinfo) を追加しました |
| 追加 | v.10 | [Project Rome の概要](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/project_rome_overview)を追加しました |
| 変更 | ベータ版 | [Upsert Activity](https://developer.microsoft.com/ja-JP/graph/docs/beta/api/projectrome_put_activity) にディープ挿入のドキュメントを追加しました |

### <a name="reports-apis"></a>レポート API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版| 委任アクセスのサポートを追加しました。 |
|追加|v1.0| 委任アクセスのサポートを追加しました。 |

### <a name="security-apis"></a>セキュリティ API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | [セキュリティ API](../api-reference/beta/resources/security-api-overview.md) を追加しました。これには次のリソースと操作が含まれています。<br/>[警告](../api-reference/beta/resources/alert.md) (および関連するエンティティ)<br/>[警告の取得](../api-reference/beta/api/alert_get.md)<br/>[警告の一覧表示](../api-reference/beta/api/alert_list.md)<br/>[警告の更新](../api-reference/beta/api/alert_update.md)<br/><br/>次の関連ドキュメントを追加しました。<br/>[エラー](../api-reference/beta/resources/security-error-codes.md)<br/>[SIEM との統合](../concepts/security_siemintegration.md)


## <a name="march-2018"></a>2018 年 3 月

### <a name="data-policy-operations"></a>データ ポリシー操作 
 
| **変更の種類** | **バージョン** | **説明**                          | 
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティ [dataPolicyOperation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/dataPolicyOperation) を追加しました。 これは、追跡のために送信されたデータ ポリシー操作を表します。
| 追加        | ベータ版        | [users](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/users) に [exportPersonalData](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_exportPersonalData) アクションを追加しました。 このアクションは、Microsoft がユーザー用に保存している個人データをエクスポートするためのデータ ポリシー操作要求を送信します。 | 

### <a name="activityfeedservice-apis"></a>ActivityFeedService API

| **変更の種類** | **バージョン** | **説明**              |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版       | [Get recent activities API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_get_recent_activities) を追加しました |
| 追加        | ベータ版       | [Get activities API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_get_activities) を追加しました |
| 変更 | ベータ版 | [Upsert Activity](https://developer.microsoft.com/ja-JP/graph/docs/beta/api/projectrome_put_activity) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [Upsert HistoryItem](https://developer.microsoft.com/ja-JP/graph/docs/beta/projectrome_put_historyitem) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [Delete Activity](https://developer.microsoft.com/ja-JP/graph/docs/beta/projectrome_delete_activity) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [Upsert HistoryItem](https://developer.microsoft.com/ja-JP/graph/docs/beta/projectrome_delete_historyItem) に UserActivity.ReadWrite.CreatedByApp アクセス許可を追加しました |
| 変更 | ベータ版 | [activity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/projectrome_activity) に **status** プロパティを追加しました |
| 変更 | ベータ版 | [historyItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/projectrome_historyitem) に **activity** ナビゲーション プロパティを追加しました |
| 変更 | ベータ版 | [Project Rome の概要](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/project_rome_overview)に新しい API を追加しました |

### <a name="azure-ad-apis"></a>Azure AD API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|変更|ベータ版|[サブスクリプション](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/subscription) リソースに **applicationID** および **creatorUserID** プロパティを追加しました。 |
|変更|ベータ版|[サブスクリプション](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/subscription) エンティティに[一覧表示](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/subscription_list)操作を追加しました。 |


### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | **onPremisesExtensionAttributes** 複合型を [user](../api-reference/beta/resources/user.md) エンティティに追加しました。 これにはオンプレミス AD の拡張属性 1 - 15 が含まれています。 |
| 追加        | ベータ版        | **privacyProfile** 複合型を [organization](../api-reference/beta/resources/organization.md) エンティティに追加しました。 |
| 追加        | v1.0        | [ユーザーとグループの復元と完全削除](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/directory)に関するサポートを追加しました。 |

### <a name="excel-apis"></a>Excel API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|変更|v1.0|[Excel Table](../api-reference/v1.0/resources/table.md) エンティティに **legacyId** プロパティを追加しました。 これには任意の Excel テーブルに対して定数となる数値識別子（文字列データ型）が含まれています。 これは、アプリケーションが古いバージョンの Excel クライアント アプリケーションで使用している従来の識別子に依存していた場合は、追加のメタデータとして提供されます。 注: `id` と `legacyId` プロパティはアプリケーションで符号化文字列値として処理し、その他の型に解析すべきではありません。 |

### <a name="reports-apis"></a>レポート API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
|追加|ベータ版|[sharePointSiteUsageDetail](../api-reference/beta/resources/sharepointsiteusagedetail.md) エンティティに **siteId** プロパティが追加されました。|

### <a name="group-lifecycle-policy"></a>グループのライフサイクル ポリシー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [groupLifecyclePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/grouplifecyclepolicy) を追加しました |
| 追加        | v1.0        | グループのライフサイクル ポリシーに、次の API を追加しました: [Create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_post_grouplifecyclepolicies)、[List](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_list)、[Get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_get)、[Update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_update)、[Delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_delete)、[Add group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_addgroup)、[Remove group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/grouplifecyclepolicy_removegroup) |
| 追加        | v1.0        | [group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/group) に [List groupLifecylePolicies](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/group_list_grouplifecyclepolicies.md) 関数を追加しました。 |
| 変更 | v1.0 | [group](../api-reference/v1.0/resources/group.md) に renewedDateTime プロパティと [renew](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/group_renew) を追加しました | 

### <a name="terms-of-use"></a>利用規約

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [agreement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/agreement) と [agreementAcceptance](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/agreementAcceptance) リソースを追加しました。 |
| 追加        | ベータ版        | 次の [agreement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/agreement) のAPI を追加しました: [Create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/greement_post_agreements), [List](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/agreement_list), [Get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/agreement_get), [Update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/agreement_update), [Delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/agreement_delete)。 |
| 追加        | ベータ版        | [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/user) リソースに [agreementAcceptance](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/agreementAcceptance) リレーションシップを追加しました。 |

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[iosMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosmobileappconfiguration)<br/>[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_vpptoken)<br/>|
|追加|v1.0|新しい複合型を追加しました。<br/>[appConfigurationSettingItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_appconfigurationsettingitem)<br/>|
|追加|v1.0|[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_vpptoken) に [syncLicenses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_vpptoken_synclicenses.md) アクションを追加しました |
|追加|v1.0|[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_deviceappmanagement) エンティティに **vppTokens** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **managementCertificateExpirationDate** プロパティを追加しました|
|追加|ベータ版|[deviceManagementSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型に **enhancedJailBreak** プロパティを追加しました|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidDeviceOwnerEnrollmentProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androiddeviceownerenrollmentprofile)<br/>[androidDeviceOwnerGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androiddeviceownergeneraldeviceconfiguration)<br/>[androidManagedStoreAccountEnterpriseSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreaccountenterprisesettings)<br/>[androidManagedStoreAppConfigurationSchema](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreappconfigurationschema)<br/>[dataSharingConsent](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_datasharingconsent)<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary)<br/>[macOSEndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_macosendpointprotectionconfiguration)<br/>[macOSImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_macosimportedpfxcertificateprofile)<br/>[macOSLobApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_macoslobapp)<br/>[managedEBookCategory](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_books_managedebookcategory)<br/>[microsoftStoreForBusinessContainedApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_microsoftstoreforbusinesscontainedapp)<br/>[mobileContainedApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_mobilecontainedapp)<br/>[windowsUniversalAppXContainedApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_windowsuniversalappxcontainedapp)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[androidManagedStoreAppConfigurationSchemaItem](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreappconfigurationschemaitem)<br/>[deviceAndAppManagementData](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_onboarding_deviceandappmanagementdata)<br/>[loggedOnUser](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_loggedonuser)<br/>[macOSFirewallApplication](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_macosfirewallapplication)<br/>[macOSLobChildApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_macoslobchildapp)<br/>[macOSMinimumOperatingSystem](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_macosminimumoperatingsystem)<br/>[windowsAppXAppAssignmentSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_windowsappxappassignmentsettings)<br/>[windowsUniversalAppXAppAssignmentSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_windowsuniversalappxappassignmentsettings)<br/>|
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreaccountenterprisesettings) に [requestSignupUrl](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_androidforwork_androidmanagedstoreaccountenterprisesettings_requestsignupurl.md) アクションを追加しました |
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreaccountenterprisesettings) に [completeSignup](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_androidforwork_androidmanagedstoreaccountenterprisesettings_completesignup.md) アクションを追加しました |
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreaccountenterprisesettings) に [syncApps](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_androidforwork_androidmanagedstoreaccountenterprisesettings_syncapps.md) アクションを追加しました |
|追加|ベータ版|[androidManagedStoreAccountEnterpriseSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidmanagedstoreaccountenterprisesettings) に [unbind](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_androidforwork_androidmanagedstoreaccountenterprisesettings_unbind.md) アクションを追加しました |
|追加|ベータ版|[androidDeviceOwnerEnrollmentProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androiddeviceownerenrollmentprofile) に [revokeToken](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_androidforwork_androiddeviceownerenrollmentprofile_revoketoken.md) アクションを追加しました |
|追加|ベータ版|[androidDeviceOwnerEnrollmentProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androiddeviceownerenrollmentprofile) に [createToken](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_androidforwork_androiddeviceownerenrollmentprofile_createtoken.md) アクションを追加しました |
|追加|ベータ版|[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) に [assign](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_apps_manageddevicemobileappconfiguration_assign.md) アクションを追加しました |
|追加|ベータ版|[dataSharingConsent](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_datasharingconsent) に [consentToDataSharing](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_devices_datasharingconsent_consenttodatasharing.md) アクションを追加しました |
|追加|ベータ版|[user](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_shared_user) に [getLoggedOnManagedDevices](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_devices_user_getloggedonmanageddevices.md) 関数を追加しました |
|追加|ベータ版|[user](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_user) に [exportDeviceAndAppManagementData](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_onboarding_user_exportdeviceandappmanagementdata.md) 関数を追加しました |
|追加|ベータ版|[user](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_user) に [exportDeviceAndAppManagementData](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_onboarding_user_exportdeviceandappmanagementdata.md) 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**appleVolumePurchaseProgramToken**<br/>**mdmAppConfigGroupAssignment**<br/>**windows10KioskConfiguration**<br/>|
|削除|ベータ版|[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) の [assign](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_apps_manageddevicemobileappconfiguration_assign.md) アクションを削除しました |
|削除|ベータ版|[appleVolumePurchaseProgramToken](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_onboarding_applevolumepurchaseprogramtoken) の [syncLicenses](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_syncapps.md) アクションを削除しました |
|追加|ベータ版|[androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) エンティティに、**workProfileBluetoothEnableContactSharing** プロパティを追加しました|
|追加|ベータ版|[androidForWorkImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkimportedpfxcertificateprofile) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[androidImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidimportedpfxcertificateprofile) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[iosImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_iosimportedpfxcertificateprofile) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[iosMobileAppConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) エンティティに **encodedSettingXml** プロパティを追加しました|
|追加|ベータ版|[managedAppRegistration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_mam_managedappregistration) エンティティに **managedDeviceId** プロパティと** azureADDeviceId** プロパティを追加しました|
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **usersLoggedOn** プロパティを追加しました|
|削除|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_manageddevice) エンティティから**lastLoggedOnUserId** プロパティを削除しました|
|追加|ベータ版|[managedDeviceOverview](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_manageddeviceoverview) エンティティに **lastModifiedDateTime** プロパティを追加しました|
|追加|ベータ版|[mobileAppContentFile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_mobileappcontentfile) エンティティに **isDependency** プロパティを追加しました|
|追加|ベータ版|[mobileThreatDefenseConnector](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector) エンティティに**windowsEnabled** プロパティ、**macEnabled** プロパティ、**windowsDeviceBlockedOnMissingPartnerData** プロパティ、**macDeviceBlockedOnMissingPartnerData** プロパティを追加しました|
|追加|ベータ版|[officeSuiteApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_officesuiteapp) エンティティに　**shouldUninstallOlderVersionsOfOffice** プロパティを追加しました|
|追加|ベータ版|[vppToken](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_onboarding_vpptoken) エンティティに **dataSharingConsentGranted** プロパティを追加しました|
|追加|ベータ版|**localSecurityOptionsBlockRemoteLogonWithBlankPassword**, **localSecurityOptionsAdministratorAccountName**, **localSecurityOptionsEnableGuestAccount**, **localSecurityOptionsGuestAccountName**, **localSecurityOptionsAllowUndockWithoutHavingToLogon**, **localSecurityOptionsBlockUsersInstallingPrinterDrivers**, **localSecurityOptionsBlockRemoteOpticalDriveAccess**, **localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser**, **localSecurityOptionsMachineInactivityLimit**, **localSecurityOptionsDoNotRequireCtrlAltDel**, **localSecurityOptionsInformationDisplayedOnLockScreen**, **localSecurityOptionsHideLastSignedInUser**, **localSecurityOptionsHideUsernameAtSignIn**, **localSecurityOptionsLogOnMessageTitle**, **localSecurityOptionsLogOnMessageText**, **localSecurityOptionsAllowPKU2UAuthenticationRequests**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager**, **localSecurityOptionsClearVirtualMemoryPageFile**, **localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn**, **localSecurityOptionsAllowUIAccessApplicationElevation**, **localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations**, **localSecurityOptionsOnlyElevateSignedExecutables**, **localSecurityOptionsAdministratorElevationPromptBehavior**, **localSecurityOptionsStandardUserElevationPromptBehavior**, **localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation**, **localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation**, **localSecurityOptionsAllowUIAccessApplicationsForSecureLocations**, **localSecurityOptionsUseAdminApprovalMode**, **localSecurityOptionsUseAdminApprovalModeForAdministrators**, **deviceGuardLocalSystemAuthorityCredentialGuardSettings**, **deviceGuardEnableVirtualizationBasedSecurity** and **deviceGuardEnableSecureBootWithDMA** プロパティを [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティに追加しました|
|削除|ベータ版|[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティから **defenderPasswordProtectedEmailContentExecutionType** プロパティを削除しました|
|追加|ベータ版|[windows10ImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10importedpfxcertificateprofile) エンティティに **intendedPurpose** プロパティを追加しました|
|削除|ベータ版|[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) エンティティから **printerNames** プロパティ、**defaultPrinterName** プロパティ、**blockAddingNewPrinter** プロパティを削除しました|
|追加|ベータ版|[windows81SCEPCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) エンティティに **certificateStore** プロパティを追加しました|
|追加|ベータ版|[windowsAutopilotDeviceIdentity](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_enrollment_windowsautopilotdeviceidentity) エンティティに **purchaseOrderIdentifier** プロパティを追加しました|
|変更|ベータ版|[windowsCertificateProfileBase](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase) エンティティで次のプロパティを変更しました:<br/>**subjectAlternativeNameType**を必須からオプションに変更しました<br/>|
|追加|ベータ版|[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration) エンティティに **advancedThreatProtectionOnboardingFilename** プロパティと **advancedThreatProtectionOffboardingFilename** プロパティを追加しました|
|追加|ベータ版|[windowsPhone81ImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windowsphone81importedpfxcertificateprofile) エンティティに **intendedPurpose** プロパティを追加しました|
|追加|ベータ版|[windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) エンティティに **skipChecksBeforeRestart** プロパティと **updateWeeks** プロパティを追加しました|
|追加|ベータ版|[deviceAppManagement](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **managedEBookCategorie** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに **androidManagedStoreAccountEnterpriseSettings** ナビゲーション プロパティ、**androidManagedStoreAppConfigurationSchemas** ナビゲーション プロパティ、**androidDeviceOwnerEnrollmentProfiles** ナビゲーション プロパティ、**dataSharingConsents** ナビゲーション プロパティ、**deviceConfigurationUserStateSummaries** ナビゲーション プロパティを追加しました|
|削除|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティから**deviceSetupConfigurations** ナビゲーション プロパティを削除しました|
|削除|ベータ版|[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|追加|ベータ版|[managedEBook](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_books_managedebook) エンティティに **categories** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[microsoftStoreForBusinessApp](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_microsoftstoreforbusinessapp) エンティティに **containedApps** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[mobileAppContent](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_mobileappcontent) エンティティに **containedApps** ナビゲーション プロパティを追加しました|
|追加|ベータ版|[windowsUniversalAppX](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_windowsuniversalappx) エンティティに **committedContainedApps** ナビゲーション プロパティを追加しました|

### <a name="onedrive"></a>OneDrive
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[baseItemVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/baseItemVersion)<br/>[driveItemVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/driveItemVersion)<br/>[listItemVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/listItemVersion)<br/> |
|追加|v1.0|新しい複合型を追加しました。<br/>[publicationFacet](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/publicationFacet)<br/> |
|追加|v1.0|[driveItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/driveItem) エンティティに <b>publication</b> プロパティを追加しました |
|追加|v1.0|[driveItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/driveItem) エンティティに <b>versions</b> ナビゲーション プロパティを追加しました |
|追加|v1.0|[listItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/listItem) エンティティに <b>versions</b> ナビゲーション プロパティを追加しました |
|追加|v1.0|[siteCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/siteCollection) エンティティに <b>root</b> プロパティを追加しました |
|追加|v1.0|[driveItemVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/driveItemVersion) エンティティに [restoreVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/driveitemversion_restore) アクションを追加しました |
|追加|v1.0|[listItemVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/listItemVersion) エンティティに [restoreVersion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/listitemversion_restore) アクションを追加しました |


### <a name="onedrive"></a>OneDrive
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい複合型を追加しました。<br/>[itemPreviewInfo](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/itemPreviewInfo)<br/> |
|追加|ベータ版|[contentTypeInfo](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/contentTypeInfo) 複合型に <b>name</b> プロパティを追加しました |
|追加|ベータ版|[deleteAction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/deleteAction) 複合型に <b>objectType</b> プロパティを追加しました |
|追加|ベータ版|[renameAction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/renameAction) 複合型に <b>newName</b> プロパティを追加しました |
|追加|ベータ版|[SharepointIds](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/renameAction) 複合型に <b>tenantId</b> プロパティを追加しました |
|追加|ベータ版|[itemActivityTimeSet](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/itemActivityTimeSet) 複合型に <b>lastRecordedDateTime</b> プロパティを追加しました |
|追加|ベータ版|[driveItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/driveItem) エンティティに [preview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/driveitem_preview) アクションを追加しました |


## <a name="february-2018"></a>2018 年 2 月

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidForWorkImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkimportedpfxcertificateprofile)<br/>[androidImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidimportedpfxcertificateprofile)<br/>[importedWindowsAutopilotDeviceIdentity](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_enrollment_importedwindowsautopilotdeviceidentity)<br/>[iosImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_iosimportedpfxcertificateprofile)<br/>[windows10ImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10importedpfxcertificateprofile)<br/>[windows10KioskConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10kioskconfiguration)<br/>[windowsPhone81ImportedPFXCertificateProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windowsphone81importedpfxcertificateprofile)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[importedWindowsAutopilotDeviceIdentityState](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate)<br/>|
|追加|ベータ版|[reportRoot](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_reportroot) に [managedDeviceEnrollmentFailureDetails](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_troubleshooting_reportroot_manageddeviceenrollmentfailuredetails.md) 機能を追加しました |
|追加|ベータ版|[reportRoot](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_reportroot) に [managedDeviceEnrollmentFailureDetails](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_troubleshooting_reportroot_manageddeviceenrollmentfailuredetails.md) 機能を追加しました |
|追加|ベータ版|[reportRoot](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_reportroot) に [managedDeviceEnrollmentFailureTrends](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_troubleshooting_reportroot_manageddeviceenrollmentfailuretrends.md) 機能を追加しました |
|追加|ベータ版|[reportRoot](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_reportroot) に [managedDeviceEnrollmentTopFailures](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_troubleshooting_reportroot_manageddeviceenrollmenttopfailures.md) 機能を追加しました |
|追加|ベータ版|[reportRoot](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_reportroot) に [managedDeviceEnrollmentTopFailures](https://developer.microsoft.com/ja-JP/api-reference/beta/api/intune_troubleshooting_reportroot_manageddeviceenrollmenttopfailures.md) 機能を追加しました |
|変更|ベータ版|[androidCompliancePolicy](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy) エンティティから、プロパティ **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** を削除しました|
|変更|ベータ版|[androidForWorkCompliancePolicy](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy) エンティティから、プロパティ **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** を削除しました|
|変更|ベータ版|[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile) エンティティから、プロパティ **name**、**modifiedDateTime**、**totalEnrollmentCount**、**qrCode** を削除しました。|
|変更|ベータ版|[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap**、**enableOuterIdentityPrivacy** を削除しました|
|変更|ベータ版|[androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) エンティティに、**workProfileBlockAddingAccounts** プロパティを追加しました|
|変更|ベータ版|[androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) エンティティから、プロパティ **blockCrossProfileCopyPaste** と **requireAppVerify** を削除しました|
|変更|ベータ版|[androidForWorkSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_androidforworksettings) エンティティに、**deviceOwnerManagementEnabled** プロパティを追加しました|
|変更|ベータ版|[androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティから **requireAppVerify** プロパティを削除しました。|
|変更|ベータ版|[androidManagedAppProtection](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティに、**exemptedAppPackages** プロパティを追加しました|
|変更|ベータ版|[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに、プロパティ **exemptedAppProtocols** と **exemptedAppPackages** を追加しました。|
|変更|ベータ版|[iosManagedAppProtection](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに、プロパティ **exemptedAppProtocols**を追加しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_manageddevice) エンティティに、**lastLoggedOnUserId** プロパティを追加しました|
|変更|ベータ版|[mobileAppContentFile](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_apps_mobileappcontentfile) エンティティに **isFrameworkFile** プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppProtection](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_mam_targetedmanagedappprotection) エンティティに、**targetedAppManagementLevels** プロパティを追加しました|
|変更|ベータ版|[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティに、プロパティ **localSecurityOptionsBlockMicrosoftAccounts**、**localSecurityOptionsEnableAdministratorAccount**、**defenderPreventCredentialStealingType**、**defenderProcessCreationType**、**defenderUntrustedUSBProcessType**、**defenderUntrustedExecutableType**、**defenderPasswordProtectedEmailContentExecutionType**、**defenderAdvancedRansomewareProtectionType**、**applicationGuardAllowFileSaveOnHost** を追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに、プロパティ **edgeFavoritesListLocation** と **edgeBlockEditFavorites** を追加しました|
|変更|ベータ版|[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) エンティティに、プロパティ **printerNames**、**defaultPrinterName**、**blockAddingNewPrinter** を追加しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティに、ナビゲーション プロパティ **importedWindowsAutopilotDeviceIdentities** を追加しました|
|変更|ベータ版|[adminConsent](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_adminconsent) 複合型に、**shareAPNSData** プロパティを追加しました|
|変更|ベータ版|[adminConsent](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_devices_adminconsent) 複合型から、**collectFullIOSAppInventory** プロパティを削除しました|
|変更|ベータ版|[outOfBoxExperienceSettings](https://developer.microsoft.com/ja-JP/api-reference/beta/resources/intune_enrollment_outofboxexperiencesettings) 複合型から、**deviceUsageType** プロパティを追加しました|


### <a name="planner-apis"></a>Planner API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しい複合型を追加しました。<br/>[plannerPlanContext](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlanContext)<br/>[plannerPlanContextDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlanContextDetails)<br/>[plannerPlanContextCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlanContextCollection)<br/>[plannerPlanContextDetailsCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlanContextDetailsCollection)<br/>[plannerFavoritePlanReference](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerFavoritePlanReference)<br/>[plannerRecentPlanReference](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerRecentPlanReference)<br/>[plannerFavoritePlanReferenceCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerFavoritePlanReferenceCollection)<br/>[plannerRecentPlanReferenceCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerRecentPlanReferenceCollection)|
|追加|ベータ版|`favoritePlanReferences` と `recentPlanReferences` プロパティを [plannerUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerUser) エンティティに追加しました。 |
|追加|ベータ版|`favoritePlans` と `recentPlans` ナビゲーション プロパティを [plannerUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerUser) エンティティに追加しました。 |
|追加|ベータ版|`contexts` プロパティを [plannerPlan](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlan) エンティティに追加しました。 |
|追加|ベータ版|[plannerPlanDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlanDetails) エンティティに `contextDetails` プロパティを追加しました。 |
|追加|ベータ版|Planner の[デルタ クエリ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/planneruser_list_delta.md)を追加しました |

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | ベータ版    | **activatedOnSharedComputer** プロパティを [userActivationCounts](../api-reference/beta/resources/useractivationcounts.md) エンティティに追加しました。|
| 追加    | ベータ版    | **sharedComputerActivation** プロパティを [office365ActivationsUserCounts](../api-reference/beta/resources/office365activationsusercounts.md) エンティティに追加しました。|

## <a name="january-2018"></a>2018 年 1 月

### <a name="json-batching"></a>JSON バッチ処理

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|[JSON バッチ処理](https://developer.microsoft.com/ja-JP/graph/docs/concepts/json_batching)のサポートを追加しました。 内部要求の制限を 20 に設定しました。|
|変更|ベータ版|[JSON バッチ処理](https://developer.microsoft.com/ja-JP/graph/docs/concepts/json_batching)の内部要求の制限を 5 から 20 に増加しました。|

### <a name="education-apis"></a>教育機関 API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|[名簿 API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/education-overview) の他のナビゲーション プロパティを追加し、フィルター処理のサポートを改善しました。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|v1.0|新しいエンティティを追加しました。<br/>[androidCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_androidcompliancepolicy)<br/>[androidCustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_androidcustomconfiguration)<br/>[androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)<br/>[androidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_androidlobapp)<br/>[androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_androidmanagedappprotection)<br/>[androidManagedAppRegistration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_androidmanagedappregistration)<br/>[androidStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_androidstoreapp)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[applePushNotificationCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_applepushnotificationcertificate)<br/>[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_defaultmanagedappprotection)<br/>[detectedApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_detectedapp)<br/>[deviceAndAppManagementRoleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_deviceandappmanagementroleassignment)<br/>[deviceAndAppManagementRoleDefinition](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_deviceandappmanagementroledefinition)<br/>[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_deviceappmanagement)<br/>[deviceCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_devicecategory)<br/>[deviceComplianceActionItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceComplianceDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancedevicestatus)<br/>[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicy)<br/>[deviceCompliancePolicyAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicyassignment)<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicystate)<br/>[deviceComplianceScheduledActionForRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancescheduledactionforrule)<br/>[deviceComplianceSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancesettingstate)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceComplianceUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceuserstatus)<br/>[deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration)<br/>[deviceConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationassignment)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary)<br/>[deviceConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationdevicestatus)<br/>[deviceConfigurationState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationstate)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[deviceConfigurationUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationuserstatus)<br/>[deviceEnrollmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentconfiguration)<br/>[deviceEnrollmentLimitConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentlimitconfiguration)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration)<br/>[deviceInstallState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_deviceinstallstate)<br/>[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_androidforwork_devicemanagement)<br/>[deviceManagementExchangeConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_devicemanagementexchangeconnector)<br/>[deviceManagementPartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_devicemanagementpartner)<br/>[deviceManagementTroubleshootingEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_troubleshooting_devicemanagementtroubleshootingevent)<br/>[eBookInstallSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_ebookinstallsummary)<br/>[editionUpgradeConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_editionupgradeconfiguration)<br/>[enrollmentConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_enrollmentconfigurationassignment)<br/>[enrollmentTroubleshootingEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_troubleshooting_enrollmenttroubleshootingevent)<br/>[iosCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioscertificateprofile)<br/>[iosCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioscompliancepolicy)<br/>[iosCustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioscustomconfiguration)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)<br/>[iosLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_ioslobapp)<br/>[iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_iosmanagedappprotection)<br/>[iosManagedAppRegistration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_iosmanagedappregistration)<br/>[iosStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosstoreapp)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_iosupdatedevicestatus)<br/>[iosVppApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosvppapp)<br/>[iosVppEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_iosvppebook)<br/>[iosVppEBookAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_iosvppebookassignment)<br/>[localizedNotificationMessage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_notification_localizednotificationmessage)<br/>[macOSCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_macoscompliancepolicy)<br/>[macOSCustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_macoscustomconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[macOSGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_macosgeneraldeviceconfiguration)<br/>[macOSOfficeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_macosofficesuiteapp)<br/>[managedAndroidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_managedandroidlobapp)<br/>[managedAndroidStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_managedandroidstoreapp)<br/>[managedApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_managedapp)<br/>[managedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappconfiguration)<br/>[managedAppOperation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappoperation)<br/>[managedAppPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedapppolicy)<br/>[managedAppPolicyDeploymentSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedapppolicydeploymentsummary)<br/>[managedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappprotection)<br/>[managedAppRegistration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappregistration)<br/>[managedAppStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappstatus)<br/>[managedAppStatusRaw](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappstatusraw)<br/>[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice)<br/>[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfiguration)<br/>[managedDeviceMobileAppConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfigurationassignment)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_manageddevicemobileappconfigurationusersummary)<br/>[managedDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddeviceoverview)<br/>[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_managedebook)<br/>[managedEBookAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_managedebookassignment)<br/>[managedIOSLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_managedioslobapp)<br/>[managedIOSStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_managediosstoreapp)<br/>[managedMobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedmobileapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_managedmobilelobapp)<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_mdmwindowsinformationprotectionpolicy)<br/>[microsoftStoreForBusinessApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_microsoftstoreforbusinessapp)<br/>[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileapp)<br/>[mobileAppAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappassignment)<br/>[mobileAppCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappcategory)<br/>[mobileAppContent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappcontent)<br/>[mobileAppContentFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappcontentfile)<br/>[mobileLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobilelobapp)<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_mobilethreatdefenseconnector)<br/>[notificationMessageTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_notification_notificationmessagetemplate)<br/>[onPremisesConditionalAccessSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[remoteAssistancePartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_remoteassistance_remoteassistancepartner)<br/>[resourceOperation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_resourceoperation)<br/>[roleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_roleassignment)<br/>[roleDefinition](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_roledefinition)<br/>[settingStateDeviceSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_settingstatedevicesummary)<br/>[sharedPCConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_softwareupdatestatussummary)<br/>[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_targetedmanagedappconfiguration)<br/>targetedManagedAppPolicyAssignment<br/>[targetedManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_targetedmanagedappprotection)<br/>[telecomExpenseManagementPartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_tem_telecomexpensemanagementpartner)<br/>[termsAndConditions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_companyterms_termsandconditions)<br/>[termsAndConditionsAcceptanceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_companyterms_termsandconditionsacceptancestatus)<br/>[termsAndConditionsAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_companyterms_termsandconditionsassignment)<br/>[userInstallStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_userinstallstatesummary)<br/>[webApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_webapp)<br/>[windows10CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10compliancepolicy)<br/>[windows10CustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10customconfiguration)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10generalconfiguration)<br/>[windows10MobileCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10mobilecompliancepolicy)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10TeamGeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10teamgeneralconfiguration)<br/>[windows81CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows81compliancepolicy)<br/>[windows81GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows81generalconfiguration)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration)<br/>[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotection)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectionapplockerfile)<br/>[windowsInformationProtectionNetworkLearningSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_wip_windowsinformationprotectionnetworklearningsummary)<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy)<br/>[windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_windowsmobilemsi)<br/>[windowsPhone81CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsphone81compliancepolicy)<br/>[windowsPhone81CustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsphone81customconfiguration)<br/>[windowsPhone81GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsphone81generalconfiguration)<br/>[windowsUniversalAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_windowsuniversalappx)<br/>[windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration)<br/>|
|追加|v1.0|新しい複合型を追加しました。<br/>[allDevicesAssignmentTarget](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_alldevicesassignmenttarget)<br/>[allLicensedUsersAssignmentTarget](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_alllicensedusersassignmenttarget)<br/>[androidMinimumOperatingSystem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_androidminimumoperatingsystem)<br/>[androidMobileAppIdentifier](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_androidmobileappidentifier)<br/>[appListItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_applistitem)<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_bitlockerremovabledrivepolicy)<br/>[configurationManagerClientEnabledFeatures](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_configurationmanagerclientenabledfeatures)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_deleteuserfromsharedappledeviceactionresult)<br/>[deviceActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_deviceactionresult)<br/>[deviceAndAppManagementAssignmentTarget](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_deviceandappmanagementassignmenttarget)<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicysettingstate)<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfigurationsettingstate)<br/>[deviceEnrollmentPlatformRestriction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentplatformrestriction)<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_deviceexchangeaccessstatesummary)<br/>[deviceGeoLocation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_devicegeolocation)<br/>[deviceHealthAttestationState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_devicehealthattestationstate)<br/>[deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicemanagementsettings)<br/>[deviceOperatingSystemSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_deviceoperatingsystemsummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_edgesearchengine)<br/>[edgeSearchEngineBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_edgesearchenginebase)<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_edgesearchenginecustom)<br/>[exclusionGroupAssignmentTarget](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_exclusiongroupassignmenttarget)<br/>[fileEncryptionInfo](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_fileencryptioninfo)<br/>[groupAssignmentTarget](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_groupassignmenttarget)<br/>[intuneBrand](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_intunebrand)<br/>[iosDeviceType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosdevicetype)<br/>[iosHomeScreenApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosLobAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_ioslobappassignmentsettings)<br/>[iosMinimumOperatingSystem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosminimumoperatingsystem)<br/>[iosMobileAppIdentifier](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_iosmobileappidentifier)<br/>[iosNetworkUsageRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_iosnetworkusagerule)<br/>[iosNotificationSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iosStoreAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosstoreappassignmentsettings)<br/>[iosVppAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_iosvppappassignmentsettings)<br/>[ipRange](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_iprange)<br/>[iPv4Range](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_ipv4range)<br/>[iPv6Range](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_ipv6range)<br/>[keyValuePair](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_androidforwork_keyvaluepair)<br/>[locateDeviceActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_locatedeviceactionresult)<br/>[managedAppDiagnosticStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappdiagnosticstatus)<br/>[managedAppPolicyDeploymentSummaryPerApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedapppolicydeploymentsummaryperapp)<br/>[mediaContentRatingAustralia](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingaustralia)<br/>[mediaContentRatingCanada](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingcanada)<br/>[mediaContentRatingFrance](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingfrance)<br/>[mediaContentRatingGermany](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratinggermany)<br/>[mediaContentRatingIreland](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingireland)<br/>[mediaContentRatingJapan](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingjapan)<br/>[mediaContentRatingNewZealand](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingnewzealand)<br/>[mediaContentRatingUnitedKingdom](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingunitedkingdom)<br/>[mediaContentRatingUnitedStates](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_mediacontentratingunitedstates)<br/>[microsoftStoreForBusinessAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_microsoftstoreforbusinessappassignmentsettings)<br/>[mimeContent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_mimecontent)<br/>[mobileAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappassignmentsettings)<br/>[mobileAppIdentifier](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_mobileappidentifier)<br/>[omaSetting](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasetting)<br/>[omaSettingBase64](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettingbase64)<br/>[omaSettingBoolean](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettingboolean)<br/>[omaSettingDateTime](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettingdatetime)<br/>[omaSettingFloatingPoint](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettingfloatingpoint)<br/>[omaSettingInteger](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettinginteger)<br/>[omaSettingString](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettingstring)<br/>[omaSettingStringXml](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_omasettingstringxml)<br/>[proxiedDomain](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_proxieddomain)<br/>[remoteLockActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_remotelockactionresult)<br/>[resetPasscodeActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_resetpasscodeactionresult)<br/>[resourceAction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_resourceaction)<br/>[rgbColor](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_rgbcolor)<br/>[rolePermission](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_rbac_rolepermission)<br/>[settingSource](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_settingsource)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[updateWindowsDeviceAccountActionParameter](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_updatewindowsdeviceaccountactionparameter)<br/>[vppLicensingType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_vpplicensingtype)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windows10networkproxyserver)<br/>[windowsDefenderScanActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_windowsdefenderscanactionresult)<br/>[windowsDeviceAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_windowsdeviceaccount)<br/>[windowsDeviceADAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_windowsdeviceadaccount)<br/>[windowsDeviceAzureADAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_windowsdeviceazureadaccount)<br/>[windowsFirewallNetworkProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsfirewallnetworkprofile)<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectionapp)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectiondesktopapp)<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectioniprangecollection)<br/>[windowsInformationProtectionProxiedDomainCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectionproxieddomaincollection)<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectionresourcecollection)<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotectionstoreapp)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsUpdateActiveHoursInstall](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsupdateactivehoursinstall)<br/>[windowsUpdateInstallScheduleType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsupdateinstallscheduletype)<br/>[windowsUpdateScheduledInstall](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_windowsupdatescheduledinstall)<br/>|
|追加|v1.0|[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileapp) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_apps_mobileapp_assign.md) アクションを追加しました |
|追加|v1.0|[mobileAppContentFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappcontentfile) に [commit](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_apps_mobileappcontentfile_commit.md) アクションを追加しました |
|追加|v1.0|[mobileAppContentFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_apps_mobileappcontentfile) に [renewUpload](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_apps_mobileappcontentfile_renewupload.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [retire](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_retire.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [wipe](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_wipe.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [resetPasscode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_resetpasscode.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [remoteLock](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_remotelock.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [requestRemoteAssistance](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_requestremoteassistance.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [disableLostMode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_disablelostmode.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [locateDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_locatedevice.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [bypassActivationLock](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_bypassactivationlock.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [rebootNow](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_rebootnow.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [shutDown](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_shutdown.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [recoverPasscode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_recoverpasscode.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [cleanWindowsDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_cleanwindowsdevice.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_deleteuserfromsharedappledevice.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [syncDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_syncdevice.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [windowsDefenderScan](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_windowsdefenderscan.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [windowsDefenderUpdateSignatures](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md) アクションを追加しました |
|追加|v1.0|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_manageddevice) に [updateWindowsDeviceAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_manageddevice_updatewindowsdeviceaccount.md) を追加しました |
|追加|v1.0|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_user) に [removeAllDevicesFromManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_user_removealldevicesfrommanagement.md) アクションを追加しました |
|追加|v1.0|[deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_deviceconfig_deviceconfiguration_assign.md) アクションを追加しました |
|追加|v1.0|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicy) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_deviceconfig_devicecompliancepolicy_assign.md) アクションを追加しました |
|追加|v1.0|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_devicecompliancepolicy) に [scheduleActionsForRules](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules.md) アクションを追加しました |
|追加|v1.0|[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_organization) に [setMobileDeviceManagementAuthority](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_organization_setmobiledevicemanagementauthority.md) アクションを追加しました |
|追加|v1.0|[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_deviceappmanagement) に [syncMicrosoftStoreForBusinessApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md) アクションを追加しました |
|追加|v1.0|[deviceManagementExchangeConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_devicemanagementexchangeconnector) に [sync](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_devicemanagementexchangeconnector_sync.md) アクションを追加しました |
|追加|v1.0|[deviceEnrollmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentconfiguration) に [setPriority](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_deviceenrollmentconfiguration_setpriority.md) アクションを追加しました |
|追加|v1.0|[deviceEnrollmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_deviceenrollmentconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_deviceenrollmentconfiguration_assign.md) アクションを追加しました |
|追加|v1.0|[targetedManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_targetedmanagedappprotection) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_targetedmanagedappprotection_assign.md) アクションを追加しました |
|追加|v1.0|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_targetedmanagedappconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_targetedmanagedappconfiguration_assign.md) アクションを追加しました |
|追加|v1.0|[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_windowsinformationprotection) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_windowsinformationprotection_assign.md) アクションを追加しました |
|追加|v1.0|[managedAppPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedapppolicy) に [targetApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_managedapppolicy_targetapps.md) アクションを追加しました |
|追加|v1.0|[managedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappprotection) に [targetApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_managedappprotection_targetapps.md) アクションを追加しました |
|追加|v1.0|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_targetedmanagedappconfiguration) に [targetApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_targetedmanagedappconfiguration_targetapps.md) アクションを追加しました |
|追加|v1.0|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_user) に [wipeManagedAppRegistrationsByDeviceTag](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md) アクションを追加しました |
|追加|v1.0|[notificationMessageTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_notification_notificationmessagetemplate) に [sendTestMessage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_notification_notificationmessagetemplate_sendtestmessage.md) アクションを追加しました |
|追加|v1.0|[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_books_managedebook) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_books_managedebook_assign.md) アクションを追加しました |
|追加|v1.0|[remoteAssistancePartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_remoteassistance_remoteassistancepartner) に [beginOnboarding](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md) アクションを追加しました |
|追加|v1.0|[remoteAssistancePartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_remoteassistance_remoteassistancepartner) に [disconnect](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_remoteassistance_remoteassistancepartner_disconnect.md) アクションを追加しました |
|追加|v1.0|[applePushNotificationCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_devices_applepushnotificationcertificate) に [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md) 関数を追加しました |
|追加|v1.0|[reportRoot](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_reportroot) に [deviceConfigurationUserActivity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md) 関数を追加しました |
|追加|v1.0|[reportRoot](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_deviceconfig_reportroot) に [deviceConfigurationDeviceActivity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md) 関数を追加しました |
|追加|v1.0|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_androidforwork_devicemanagement) に [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_onboarding_devicemanagement_verifywindowsenrollmentautodiscovery.md) 関数を追加しました |
|追加|v1.0|[managedAppRegistration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_mam_managedappregistration) コレクションに **getUserIdsWithFlaggedAppRegistration** 関数を追加しました |
|追加|v1.0|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_user) に [getManagedAppDiagnosticStatuses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_user_getmanagedappdiagnosticstatuses.md) 関数を追加しました |
|追加|v1.0|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_user) に [getManagedAppPolicies](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_mam_user_getmanagedapppolicies.md) 関数を追加しました |
|追加|v1.0|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_androidforwork_devicemanagement) に [getEffectivePermissions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/intune_rbac_devicemanagement_geteffectivepermissions.md) 関数を追加しました |
|変更|v1.0|[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_onboarding_organization) エンティティに **mobileDeviceManagementAuthority** プロパティを追加しました|
|変更|v1.0|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_user) エンティティに **deviceEnrollmentLimit** プロパティを追加しました|
|変更|v1.0|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_shared_user) エンティティに **managedDevices**、**managedAppRegistrations**、**deviceManagementTroubleshootingEvents** ナビゲーション プロパティを追加しました|
|||
|追加|ベータ版|新しいエンティティを追加しました。<br/>[deviceManagementScriptAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_devicemanagementscriptassignment)<br/>[iosCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/resources/intune_deviceconfig_ioscertificateprofile)<br/>[windowsInformationProtectionNetworkLearningSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionnetworklearningsummary)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[revokeAppleVppLicensesActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_revokeapplevpplicensesactionresult)<br/>[vppTokenRevokeLicensesActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptokenrevokelicensesactionresult)<br/>|
|追加|ベータ版|[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile) に [revokeToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworkenrollmentprofile_revoketoken.md) アクションを追加しました |
|追加|ベータ版|[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_mobileapp_assign.md) アクションを追加しました |
|追加|ベータ版|[deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_devicemanagementscript) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_devicemanagementscript_assign.md) アクションを追加しました |
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [revokeAppleVppLicenses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_revokeapplevpplicenses.md) アクションを追加しました |
|追加|ベータ版|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_assign.md) アクションを追加しました |
|追加|ベータ版|[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken) に [revokeLicenses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_vpptoken_revokelicenses.md) アクションを追加しました |
|追加|ベータ版|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_user) に [wipeManagedAppRegistrationsByDeviceTag](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md) アクションを追加しました |
|追加|ベータ版|[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_books_managedebook_assign.md) アクションを追加しました |
|追加|ベータ版|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_user) に [getEffectiveDeviceEnrollmentConfigurations](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_user_geteffectivedeviceenrollmentconfigurations.md) 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**appReportingOverviewStatus**<br/>**complianceSettingStateSummary**<br/>**deviceConfigurationUserStateSummary**<br/>**eBookGroupAssignment**<br/>**eBookVppGroupAssignment**<br/>**mobileAppGroupAssignment**<br/>**mobileAppVppGroupAssignment**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**androidForWorkAppConfigurationExample**<br/>**androidForWorkAppConfigurationExampleJson**<br/>**appInstallationFailure**<br/>**appsComplianceListItem**<br/>**defaultDeviceEnrollmentRestrictions**<br/>**defaultDeviceEnrollmentWindowsHelloForBusinessSettings**<br/>**deviceEnrollmentPlatformRestrictions**<br/>|
|変更|ベータ版|[androidCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy) エンティティに **securityRequireVerifyApps**、**securityRequireSafetyNetAttestationBasicIntegrity**、**securityRequireSafetyNetAttestationCertifiedDevice**、**securityRequireGooglePlayServices**、**securityRequireUpToDateSecurityProviders**、**securityRequireCompanyPortalAppIntegrity** プロパティを追加しました|
|変更|ベータ版|[androidForWorkApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp) エンティティに **packageId** プロパティを追加しました|
|変更|ベータ版|[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema) エンティティで次のプロパティの型を変更しました:<br/>**exampleJson** を [androidForWorkAppConfigurationExample](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample.md) からバイナリに変更しました<br/>|
|変更|ベータ版|[androidForWorkCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy) エンティティに **securityRequireVerifyApps**、**securityRequireSafetyNetAttestationBasicIntegrity**、**securityRequireSafetyNetAttestationCertifiedDevice**、**securityRequireGooglePlayServices**、**securityRequireUpToDateSecurityProviders**、**securityRequireCompanyPortalAppIntegrity** プロパティを追加しました|
|変更|ベータ版|[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile) エンティティに **displayName**、**lastModifiedDateTime**、**enrolledDeviceCount**、**qrCodeContent**、**qrCodeImage** プロパティを追加しました|
|変更|ベータ版|[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile) エンティティから **isTokenActive** プロパティを削除しました|
|変更|ベータ版|[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration) エンティティに、**innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap**、**outerIdentityPrivacyTemporaryValue** プロパティを追加しました|
|変更|ベータ版|[androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) エンティティに、**workProfileBlockCrossProfileCopyPaste** と **securityRequireVerifyApps** プロパティを追加しました|
|変更|ベータ版|[androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティに **securityRequireVerifyApps** プロパティを追加しました|
|変更|ベータ版|[androidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp) エンティティに **packageId** と **identityVersion** プロパティを追加しました|
|変更|ベータ版|[androidStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp) エンティティに **packageId** プロパティを追加しました|
|変更|ベータ版|[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに **faceIdBlocked** プロパティを追加しました|
|変更|ベータ版|[deviceAndAppManagementRoleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_deviceandappmanagementroleassignment) エンティティに **members** プロパティを追加しました|
|変更|ベータ版|[deviceEnrollmentPlatformRestrictionsConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration) エンティティに **macOSRestriction** プロパティを追加しました|
|変更|ベータ版|[deviceManagementPartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementpartner) エンティティに **whenPartnerDevicesWillBeRemovedDateTime** と **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** プロパティを追加しました|
|変更|ベータ版|[deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_devicemanagementscript) エンティティで次のプロパティの型を変更しました:<br/>**scriptContent** を文字列からバイナリに変更しました<br/>|
|変更|ベータ版|[iosEasEmailProfileConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseasemailprofileconfiguration) エンティティに **smimeEnablePerMessageSwitch** プロパティを追加しました|
|変更|ベータ版|[iosLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに **faceIdBlocked** プロパティを追加しました|
|変更|ベータ版|[managedAndroidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp) エンティティに **packageId** と **identityVersion** プロパティを追加しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **azureADDeviceId** と **remoteAssistanceSessionErrorDetails** プロパティを追加しました|
|変更|ベータ版|[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) エンティティから、**legacyAppConfiguration** プロパティを削除しました|
|変更|ベータ版|[managedIOSLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[managedMobileLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp) エンティティから **identityVersion** プロパティを削除しました|
|変更|ベータ版|[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) エンティティに **publishingState** プロパティを追加しました|
|変更|ベータ版|[mobileAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) エンティティに **installState** プロパティを追加しました|
|変更|ベータ版|[mobileLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobilelobapp) エンティティから **identityVersion** プロパティを削除しました|
|変更|ベータ版|[mobileThreatDefenseConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector) エンティティに **allowPartnerToCollectIOSApplicationMetadata** プロパティを追加しました|
|変更|ベータ版|[roleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_roleassignment) エンティティから **members** プロパティを削除しました|
|変更|ベータ版|[termsAndConditions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditions) エンティティに **lastModifiedDateTime** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy) エンティティに **deviceThreatProtectionEnabled** と **deviceThreatProtectionRequiredSecurityLevel** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy) エンティティから **minimumUpdateAutoInstallClassification** プロパティを削除しました|
|変更|ベータ版|[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに **privacyBlockPublishUserActivities** と **privacyBlockActivityFeed** プロパティを追加しました|
|変更|ベータ版|[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) エンティティに **configurationAccountType** プロパティを追加しました|
|変更|ベータ版|[windows10VpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration) エンティティから **trustedNetworkDomains** プロパティを削除しました|
|変更|ベータ版|[windows81CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81compliancepolicy) エンティティから **minimumUpdateAutoInstallClassification** プロパティを削除しました|
|変更|ベータ版|[windowsAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsappx) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy) エンティティに **daysWithoutContactBeforeUnenroll** プロパティを追加しました|
|変更|ベータ版|[windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsPhone81AppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsPhoneXAP](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[windowsUniversalAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx) エンティティに **identityVersion** プロパティを追加しました|
|変更|ベータ版|[activeDirectoryWindowsAutopilotDeploymentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_enrollment_activedirectorywindowsautopilotdeploymentprofile) エンティティに **domainJoinConfiguration** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceComplianceActionItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) エンティティから **notificationMessageTemplate** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティに **windowsInformationProtectionNetworkLearningSummaries** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティから、**deviceConfigurationUserStateSummaries** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティで次のプロパティの型を変更しました:<br/>**roleAssignments** を [roleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_roleassignment) コレクションから [deviceAndAppManagementRoleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_deviceandappmanagementroleassignment) コレクションに変更しました<br/>|
|変更|ベータ版|[deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_devicemanagementscript) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosEasEmailProfileConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseasemailprofileconfiguration) エンティティに **smimeEncryptionCertificate** プロパティを追加しました|
|変更|ベータ版|[iosEasEmailProfileConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseasemailprofileconfiguration) エンティティで次のプロパティの型を変更しました:<br/>**smimeSigningCertificate** を [iosCertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscertificateprofilebase) から [iosCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscertificateprofile) に変更しました<br/>|
|変更|ベータ版|[iosVppApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) エンティティから **vppToken** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) エンティティから **groupAssignments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_organization) エンティティから **depOnboardingSettings** と **appleVolumePurchaseProgramTokens** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_user) エンティティに **deviceEnrollmentConfigurations** ナビゲーション プロパティを追加しました|
|変更|ベータ版|
  [deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型から **windowsCommercialId** プロパティと **windowsCommercialIdLastModifiedTime** プロパティを削除しました|
|変更|ベータ版|[intuneBrand](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_intunebrand) 複合型に **showDisplayNameNextToLogo** プロパティを追加しました|
|変更|ベータ版|[outOfBoxExperienceSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_enrollment_outofboxexperiencesettings) 複合型に **deviceUsageType** プロパティを追加しました|
|変更|ベータ版|[vppLicensingType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_vpplicensingtype) 複合型に **supportsUserLicensing** と **supportsDeviceLicensing** プロパティを追加しました|
|変更|ベータ版|[vppTokenActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptokenactionresult) 複合型から **actionMessage** プロパティを削除しました|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | v1.0    | 以下の API を追加しました。<br>[getTeamsUserActivityUserDetail](../api-reference/v1.0/api/reportroot_getteamsuseractivityuserdetail.md)<br>[getTeamsUserActivityCounts](../api-reference/v1.0/api/reportroot_getteamsuseractivitycounts.md)<br>[getTeamsUserActivityUserCounts](../api-reference/v1.0/api/reportroot_getteamsuseractivityusercounts.md)<br>[getTeamsDeviceUsageUserDetail](../api-reference/v1.0/api/reportroot_getteamsdeviceusageuserdetail.md)<br>[getTeamsDeviceUsageUserCounts](../api-reference/v1.0/api/reportroot_getteamsdeviceusageusercounts.md)<br>[getTeamsDeviceUsageDistributionUserCounts](../api-reference/v1.0/api/reportroot_getteamsdeviceusagedistributionusercounts.md) |

## <a name="december-2017"></a>2017 年 12 月

### <a name="delta-query"></a>デルタ クエリ

| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 変更      | v1.0    | [users](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_delta) と [groups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/group_delta) に、オプションのクエリ フィルタリング機能を追加します。 |

### <a name="microsoft-intune-apis"></a>Microsoft Intune API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile)<br/>[deviceAndAppManagementRoleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_deviceandappmanagementroleassignment)<br/>[deviceAndAppManagementRoleDefinition](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_deviceandappmanagementroledefinition)<br/>[macOSLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_macoslobapp)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[resourceAction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_resourceaction)<br/>[updateWindowsDeviceAccountActionParameter](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_updatewindowsdeviceaccountactionparameter)<br/>[vppTokenActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptokenactionresult)<br/>[windowsDeviceAADAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_windowsdeviceaadaccount)<br/>[windowsDeviceAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_windowsdeviceaccount)<br/>[windowsDeviceADAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_windowsdeviceadaccount)<br/>|
|追加|ベータ版|[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile) に [revokeTokens](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworkenrollmentprofile_revoketokens) アクションを追加しました |
|追加|ベータ版|[androidForWorkEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkenrollmentprofile) に [createToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworkenrollmentprofile_createtoken) アクションを追加しました |
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [wipe](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_wipe) アクションを追加しました |
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [updateWindowsDeviceAccount](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_updatewindowsdeviceaccount) を追加しました |
|追加|ベータ版|[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken) に [revokeLicenses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_vpptoken_revokelicenses) アクションを追加しました |
|追加|ベータ版|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) コレクションに [getDevicePasscode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_getdevicepasscode) 関数を追加しました |
|追加|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) に [getEffectivePermissions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_rbac_devicemanagement_geteffectivepermissions) 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**windowsStoreForBusinessApp**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**windowsStoreForBusinessAppAssignmentSettings**<br/>|
|変更|ベータ版|[androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティに **dateAndTimeBlockChanges** プロパティを追加しました|
|変更|ベータ版|[depEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) エンティティから **enableAuthenticationViaCompanyPortal** プロパティを削除しました|
|変更|ベータ版|[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティから **windowsStoreForBusinessLastSuccessfulSyncDateTime** プロパティ、**isEnabledForWindowsStoreForBusiness** プロパティ、**windowsStoreForBusinessLanguage** プロパティ、**windowsStoreForBusinessLastCompletedApplicationSyncTime** プロパティを削除しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティに **maximumDepTokens** プロパティと **intuneAccountId** プロパティを追加しました|
|変更|ベータ版|[enrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_corpenrollment_enrollmentprofile) エンティティに **enableAuthenticationViaCompanyPortal** プロパティを追加しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **managedDeviceName** プロパティと **partnerReportedThreatState** プロパティを追加しました|
|変更|ベータ版|[officeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) エンティティに **installProgressDisplayLevel** プロパティを追加しました|
|変更|ベータ版|[roleAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_roleassignment) エンティティに **resourceScopes** プロパティを追加しました|
|変更|ベータ版|[roleDefinition](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_roledefinition) エンティティに **rolePermissions** プロパティと **isBuiltIn** プロパティを追加しました|
|変更|ベータ版|[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken) エンティティに **tokenActionResults** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy)エンティティに **minimumUpdateAutoInstallClassification** プロパティを追加しました|
|変更|ベータ版|[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティに **defenderSecurityCenterDisableAppBrowserUI** プロパティ、**defenderSecurityCenterDisableFamilyUI** プロパティ、**defenderSecurityCenterDisableHealthUI**, **defenderSecurityCenterDisableNetworkUI** プロパティ、**defenderSecurityCenterDisableVirusUI** プロパティ、**defenderSecurityCenterOrganizationDisplayName**, **defenderSecurityCenterHelpEmail** プロパティ、**defenderSecurityCenterHelpPhone** プロパティ、**defenderSecurityCenterHelpURL** プロパティ、**defenderSecurityCenterNotificationsFromApp** プロパティ、**defenderSecurityCenterITContactDisplay** プロパティ、**applicationGuardAllowVirtualGPU** プロパティを追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに **enableAutomaticRedeployment** プロパティと **authenticationAllowFIDODevice** プロパティを追加しました|
|変更|ベータ版|[windows10VpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration) エンティティに **trustedNetworkDomains** プロパティを追加しました|
|変更|ベータ版|[windows81CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81compliancepolicy) エンティティに **minimumUpdateAutoInstallClassification** プロパティを追加しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティに **androidForWorkEnrollmentProfiles** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceHealthAttestationState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_devicehealthattestationstate) 複合型に **healthAttestationSupportedStatus** プロパティを追加しました|
|変更|ベータ版|[hardwareInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_hardwareinformation) 複合型に **tpmSpecificationVersion** プロパティ、**operatingSystemEdition** プロパティ、**deviceFullQualifiedDomainName** プロパティ、**deviceGuardVirtualizationBasedSecurityHardwareRequirementState** プロパティ、**deviceGuardVirtualizationBasedSecurityState** プロパティ、**deviceGuardLocalSystemAuthorityCredentialGuardState** プロパティを追加しました|
|変更|ベータ版|[iosVppAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosvppappassignmentsettings) 複合型に **vpnConfigurationId** プロパティを追加しました|
|変更|ベータ版|[rolePermission](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_rolepermission) 複合型に **resourceActions** プロパティを追加しました|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 追加    | v1.0    | 以下の API を追加しました。<br>[getEmailActivityUserDetail](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/reportroot_getemailactivityuserdetail.md)<br>[getEmailActivityCounts](../api-reference/v1.0/api/reportroot_getemailactivitycounts.md)<br>[getEmailActivityUserCounts](../api-reference/v1.0/api/reportroot_getemailactivityusercounts.md)<br>[getEmailAppUsageUserDetail](../api-reference/v1.0/api/reportroot_getemailappusageuserdetail.md)<br>[getEmailAppUsageAppsUserCounts](../api-reference/v1.0/api/reportroot_getemailappusageappsusercounts.md)<br>[getEmailAppUsageUserCounts](../api-reference/v1.0/api/reportroot_getemailappusageusercounts.md)<br>[getEmailAppUsageVersionsUserCounts](../api-reference/v1.0/api/reportroot_getemailappusageversionsusercounts.md)<br>[getMailboxUsageDetail](../api-reference/v1.0/api/reportroot_getmailboxusagedetail.md)<br>[getMailboxUsageMailboxCounts](../api-reference/v1.0/api/reportroot_getmailboxusagemailboxcounts.md)<br>[getMailboxUsageQuotaStatusMailboxCounts](../api-reference/v1.0/api/reportroot_getmailboxusagequotastatusmailboxcounts.md)<br>[getMailboxUsageStorage](../api-reference/v1.0/api/reportroot_getmailboxusagestorage.md)<br>[getOffice365ActivationsUserDetail](../api-reference/v1.0/api/reportroot_getoffice365activationsuserdetail.md)<br>[getOffice365ActivationCounts](../api-reference/v1.0/api/reportroot_getoffice365activationcounts.md)<br>[getOffice365ActivationsUserCounts](../api-reference/v1.0/api/reportroot_getoffice365activationsusercounts.md)<br>[getOffice365ActiveUserDetail](../api-reference/v1.0/api/reportroot_getoffice365activeuserdetail.md)<br>[getOffice365ActiveUserCounts](../api-reference/v1.0/api/reportroot_getoffice365activeusercounts.md)<br>[getOffice365ServicesUserCounts](../api-reference/v1.0/api/reportroot_getoffice365servicesusercounts.md)<br>[getOffice365GroupsActivityDetail](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitydetail.md)<br> [getOffice365GroupsActivityCounts](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitycounts.md)<br>[getOffice365GroupsActivityGroupCounts](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitygroupcounts.md)<br>[getOffice365GroupsActivityStorage](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitystorage.md)<br>[getOffice365GroupsActivityFileCounts](../api-reference/v1.0/api/reportroot_getoffice365groupsactivityfilecounts.md)<br>[getOneDriveActivityUserDetail](../api-reference/v1.0/api/reportroot_getonedriveactivityuserdetail.md)<br>[getOneDriveActivityUserCounts](../api-reference/v1.0/api/reportroot_getonedriveactivityusercounts.md)<br>[getOneDriveActivityFileCounts](../api-reference/v1.0/api/reportroot_getonedriveactivityfilecounts.md)<br>[getOneDriveUsageAccountDetail](../api-reference/v1.0/api/reportroot_getonedriveusageaccountdetail.md)<br>[getOneDriveUsageAccountCounts](../api-reference/v1.0/api/reportroot_getonedriveusageaccountcounts.md)<br>[getOneDriveUsageFileCounts](../api-reference/v1.0/api/reportroot_getonedriveusagefilecounts.md)<br>[getOneDriveUsageStorage](../api-reference/v1.0/api/reportroot_getonedriveusagestorage.md)<br>[getSharePointActivityUserDetail](../api-reference/v1.0/api/reportroot_getsharepointactivityuserdetail.md)<br>[getSharePointActivityFileCounts](../api-reference/v1.0/api/reportroot_getsharepointactivityfilecounts.md)<br>[getSharePointActivityUserCounts](../api-reference/v1.0/api/reportroot_getsharepointactivityusercounts.md)<br>[getSharePointActivityPages](../api-reference/v1.0/api/reportroot_getsharepointactivitypages.md)<br>[getSharePointSiteUsageDetail](../api-reference/v1.0/api/reportroot_getsharepointsiteusagedetail.md)<br>[getSharePointSiteUsageFileCounts](../api-reference/v1.0/api/reportroot_getsharepointsiteusagefilecounts.md)<br>[getSharePointSiteUsageSiteCounts](../api-reference/v1.0/api/reportroot_getsharepointsiteusagesitecounts.md)<br>[getSharePointSiteUsageStorage](../api-reference/v1.0/api/reportroot_getsharepointsiteusagestorage.md)<br>[getSharePointSiteUsagePages](../api-reference/v1.0/api/reportroot_getsharepointsiteusagepages.md)<br>[getSkypeForBusinessActivityUserDetail](../api-reference/v1.0/api/reportroot_getskypeforbusinessactivityuserdetail.md)<br>[getSkypeForBusinessActivityCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessactivitycounts.md)<br>[getSkypeForBusinessActivityUserCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessactivityusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserDetail](../api-reference/v1.0/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessdeviceusageusercounts.md)<br>[getSkypeForBusinessOrganizerActivityCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessorganizeractivitycounts.md)<br>[getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md)<br>[getSkypeForBusinessParticipantActivityCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessparticipantactivitycounts.md)<br>[getSkypeForBusinessParticipantActivityUserCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md)<br>[getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/v1.0/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md)<br>[getYammerActivityUserDetail](../api-reference/v1.0/api/reportroot_getyammeractivityuserdetail.md)<br>[getYammerActivityCounts](../api-reference/v1.0/api/reportroot_getyammeractivitycounts.md)<br>[getYammerActivityUserCounts](../api-reference/v1.0/api/reportroot_getyammeractivityusercounts.md)<br>[getYammerDeviceUsageUserDetail](../api-reference/v1.0/api/reportroot_getyammerdeviceusageuserdetail.md)<br>[getYammerDeviceUsageDistributionUserCounts](../api-reference/v1.0/api/reportroot_getyammerdeviceusagedistributionusercounts.md)<br>[getYammerDeviceUsageUserCounts](../api-reference/v1.0/api/reportroot_getyammerdeviceusageusercounts.md)<br>[getYammerGroupsActivityDetail](../api-reference/v1.0/api/reportroot_getyammergroupsactivitydetail.md)<br>[getYammerGroupsActivityGroupCounts](../api-reference/v1.0/api/reportroot_getyammergroupsactivitygroupcounts.md)<br>[getYammerGroupsActivityCounts](../api-reference/v1.0/api/reportroot_getyammergroupsactivitycounts.md)|
| 追加    | ベータ版    | 以下の API を追加しました。<br>[getTeamsUserActivityUserDetail](../api-reference/beta/api/reportroot_getteamsuseractivityuserdetail.md)<br>[getTeamsUserActivityCounts](../api-reference/beta/api/reportroot_getteamsuseractivitycounts.md)<br>[getTeamsUserActivityUserCounts](../api-reference/beta/api/reportroot_getteamsuseractivityusercounts.md)<br>[getTeamsDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getteamsdeviceusageuserdetail.md)<br>[getTeamsDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getteamsdeviceusageusercounts.md)<br>[getTeamsDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getteamsdeviceusagedistributionusercounts.md) |

## <a name="november-2017"></a>2017 年 11 月

### <a name="azure-ad-synchronization-apis"></a>Azure AD 同期 API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 次のリソースを含む、Azure AD ID 同期のサポートが追加されました。<br/>[Job](../api-reference/beta/resources/synchronization_synchronizationjob.md)<br/>[Schema](../api-reference/beta/resources/synchronization_synchronizationschema.md)<br/>[Template](../api-reference/beta/resources/synchronization_synchronizationtemplate.md)<br/>使用可能なメソッドの詳細については、リソースのトピックを参照してください。|

### <a name="education-apis"></a>教育機関 API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|次のリソースを含む、教育機関向けのシナリオのサポートが追加されました。<br/>[Schools](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/educationschool)<br/>[Classes](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/educationclass)<br/>[Users](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/educationuser)<br/>[Assignments](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/educationassignment)<br/>[Submissions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/educationsubmission)<br/>使用可能なメソッドの詳細については、リソースのトピックを参照してください。|

### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[auditEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditevent)<br/>[deviceManagementTroubleshootingEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_troubleshooting_devicemanagementtroubleshootingevent)<br/>[deviceSetupConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicesetupconfiguration)<br/>[enrollmentTroubleshootingEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_troubleshooting_enrollmenttroubleshootingevent)<br/>[macOSOfficeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_macosofficesuiteapp)<br/>[microsoftStoreForBusinessApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_microsoftstoreforbusinessapp)<br/>[ndesConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ndesconnector)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[auditActor](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditactor)<br/>[auditProperty](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditproperty)<br/>[auditResource](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditresource)<br/>[bulkManagedDeviceActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_bulkmanageddeviceactionresult)<br/>[deviceProtectionOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_deviceprotectionoverview)<br/>[microsoftStoreForBusinessAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_microsoftstoreforbusinessappassignmentsettings)<br/>[operatingSystemVersionRange](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_operatingsystemversionrange)<br/>[remoteLockActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_remotelockactionresult)<br/>|
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) コレクションに executeAction アクションを追加しました |
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [wipe](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_wipe.md) アクションを追加しました |
|追加|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [shutDown](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_shutdown.md) アクションを追加しました |
|追加|ベータ版|[deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_assign.md) アクションを追加しました |
|追加|ベータ版|[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) に [syncMicrosoftStoreForBusinessApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md) アクションを追加しました |
|追加|ベータ版|[enrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_corpenrollment_enrollmentprofile) に setDefaultProfile アクションを追加しました |
|追加|ベータ版|[depOnboardingSetting](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting) に ShareForSchoolDataSyncService アクションを追加しました |
|追加|ベータ版|[depOnboardingSetting](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting) に unshareForSchoolDataSyncService アクションを追加しました |
|追加|ベータ版|[auditEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditevent) コレクションに getAuditCategories 関数を追加しました |
|追加|ベータ版|[auditEvent](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_auditing_auditevent) コレクションに getAuditActivityType 関数を追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**mobileAppIdentifierDeployment**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**windowsInformationProtectionCloudResource**<br/>**windowsInformationProtectionCloudResourceCollection**<br/>|
|変更|ベータ版|[androidDeviceComplianceLocalActionLockDeviceWithPasscode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionlockdevicewithpasscode) エンティティで次のプロパティを変更しました。<br/>**passcode** を必須から省略可能に変更しました<br/>|
|変更|ベータ版|[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **microsoftStoreForBusinessLastSuccessfulSyncDateTime** プロパティ、**isEnabledForMicrosoftStoreForBusiness** プロパティ、**microsoftStoreForBusinessLanguage** プロパティ、**microsoftStoreForBusinessLastCompletedApplicationSyncTime** プロパティを追加しました|
|変更|ベータ版|[deviceConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationassignment) エンティティに **target** プロパティを追加しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティに **deviceProtectionOverview** プロパティを追加しました|
|変更|ベータ版|[deviceManagementExchangeConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeconnector) エンティティに **exchangeAlias** プロパティと **exchangeOrganization** プロパティを追加しました|
|変更|ベータ版|[managedAndroidStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedandroidstoreapp) エンティティに **appStoreUrl** プロパティと **minimumSupportedOperatingSystem** プロパティを追加しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **remoteAssistanceSessionErrorString** プロパティを追加しました|
|変更|ベータ版|[managedIOSStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managediosstoreapp) エンティティに **appStoreUrl** プロパティ、**applicableDeviceType** プロパティ、**minimumSupportedOperatingSystem** プロパティを追加しました|
|変更|ベータ版|[mobileAppInstallSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary) エンティティに **notApplicableDeviceCount** プロパティ、**pendingInstallDeviceCount** プロパティ、**notApplicableUserCount** プロパティ、**pendingInstallUserCount** プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティから **targetedSecurityGroupIds** プロパティと **targetedSecurityGroupsCount** プロパティを削除しました|
|変更|ベータ版|[targetedManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappprotection) エンティティから **targetedSecurityGroupsCount** プロパティと **targetedSecurityGroupIds** プロパティを削除しました|
|変更|ベータ版|[windows10CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy) エンティティに **validOperatingSystemBuildRanges** プロパティを追加しました|
|変更|ベータ版|[windows10MobileCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10mobilecompliancepolicy) エンティティに **activeFirewallRequired** プロパティ、**uacRequired** プロパティ、**validOperatingSystemBuildRanges** プロパティを追加しました|
|変更|ベータ版|[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration) エンティティに **enableExpeditedTelemetryReporting** プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) エンティティから **allowedApps** プロパティ、**enterpriseCloudResources** プロパティ、**targetedSecurityGroupIds** プロパティを削除しました|
|変更|ベータ版|[windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) エンティティに **ignoreVersionDetection** プロパティを追加しました|
|変更|ベータ版|[androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationassignment) エンティティから **deviceConfiguration** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceConfigurationGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment) エンティティに **deviceConfiguration** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) エンティティに **deviceSetupConfigurations** ナビゲーション プロパティ、**ndesConnectors** ナビゲーション プロパティ、**exchangeOnPremisesPolicies** ナビゲーション プロパティ、**conditionalAccessSettings** ナビゲーション プロパティ、**auditEvents** ナビゲーション プロパティ、**troubleshootingEvents** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **windowsProtectionState** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティから、**mobileAppIdentifierDeployments** ナビゲーション プロパティおよび **targetedSecurityGroups** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[targetedManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappprotection) エンティティから **targetedSecurityGroups** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_user) エンティティに **deviceManagementTroubleshootingEvents** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) エンティティから **allowedAppLockerFiles** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[windowsManagedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_windowsmanageddevice) エンティティから **windowsProtectionState** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[iosMinimumOperatingSystem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosminimumoperatingsystem) 複合型に **v11_0** プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtectionApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp) 複合型に **denied** プロパティを追加しました|

### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 次の API に JSON サポートが追加されました。<br>[getEmailActivityUserDetail](../api-reference/beta/api/reportroot_getemailactivityuserdetail.md)<br>[getEmailActivityCounts](../api-reference/beta/api/reportroot_getemailactivitycounts.md)<br>[getEmailActivityUserCounts](../api-reference/beta/api/reportroot_getemailactivityusercounts.md)<br>[getEmailAppUsageUserDetail](../api-reference/beta/api/reportroot_getemailappusageuserdetail.md)<br>[getEmailAppUsageAppsUserCounts](../api-reference/beta/api/reportroot_getemailappusageappsusercounts.md)<br>[getEmailAppUsageUserCounts](../api-reference/beta/api/reportroot_getemailappusageusercounts.md)<br>[getEmailAppUsageVersionsUserCounts](../api-reference/beta/api/reportroot_getemailappusageversionsusercounts.md)<br>[getMailboxUsageDetail](../api-reference/beta/api/reportroot_getmailboxusagedetail.md)<br>[getMailboxUsageMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagemailboxcounts.md)<br>[getMailboxUsageQuotaStatusMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagequotastatusmailboxcounts.md)<br>[getMailboxUsageStorage](../api-reference/beta/api/reportroot_getmailboxusagestorage.md)<br>[getOffice365ActivationsUserDetail](../api-reference/beta/api/reportroot_getoffice365activationsuserdetail.md)<br>[getOffice365ActivationCounts](../api-reference/beta/api/reportroot_getoffice365activationcounts.md)<br>[getOffice365ActivationsUserCounts](../api-reference/beta/api/reportroot_getoffice365activationsusercounts.md)<br>[getOffice365ActiveUserDetail](../api-reference/beta/api/reportroot_getoffice365activeuserdetail.md)<br>[getOffice365ActiveUserCounts](../api-reference/beta/api/reportroot_getoffice365activeusercounts.md)<br>[getOffice365ServicesUserCounts](../api-reference/beta/api/reportroot_getoffice365servicesusercounts.md)<br>[getOffice365GroupsActivityDetail](../api-reference/beta/api/reportroot_getoffice365groupsactivitydetail.md)<br> [getOffice365GroupsActivityCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitycounts.md)<br>[getOffice365GroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitygroupcounts.md)<br>[getOffice365GroupsActivityStorage](../api-reference/beta/api/reportroot_getoffice365groupsactivitystorage.md)<br>[getOffice365GroupsActivityFileCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivityfilecounts.md)<br>[getOneDriveActivityUserDetail](../api-reference/beta/api/reportroot_getonedriveactivityuserdetail.md)<br>[getOneDriveActivityUserCounts](../api-reference/beta/api/reportroot_getonedriveactivityusercounts.md)<br>[getOneDriveActivityFileCounts](../api-reference/beta/api/reportroot_getonedriveactivityfilecounts.md)<br>[getOneDriveUsageAccountDetail](../api-reference/beta/api/reportroot_getonedriveusageaccountdetail.md)<br>[getOneDriveUsageAccountCounts](../api-reference/beta/api/reportroot_getonedriveusageaccountcounts.md)<br>[getOneDriveUsageFileCounts](../api-reference/beta/api/reportroot_getonedriveusagefilecounts.md)<br>[getOneDriveUsageStorage](../api-reference/beta/api/reportroot_getonedriveusagestorage.md)<br>[getSharePointActivityUserDetail](../api-reference/beta/api/reportroot_getsharepointactivityuserdetail.md)<br>[getSharePointActivityFileCounts](../api-reference/beta/api/reportroot_getsharepointactivityfilecounts.md)<br>[getSharePointActivityUserCounts](../api-reference/beta/api/reportroot_getsharepointactivityusercounts.md)<br>[getSharePointActivityPages](../api-reference/beta/api/reportroot_getsharepointactivitypages.md)<br>[getSharePointSiteUsageDetail](../api-reference/beta/api/reportroot_getsharepointsiteusagedetail.md)<br>[getSharePointSiteUsageFileCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagefilecounts.md)<br>[getSharePointSiteUsageSiteCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagesitecounts.md)<br>[getSharePointSiteUsageStorage](../api-reference/beta/api/reportroot_getsharepointsiteusagestorage.md)<br>[getSharePointSiteUsagePages](../api-reference/beta/api/reportroot_getsharepointsiteusagepages.md)<br>[getSkypeForBusinessActivityUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessactivityuserdetail.md)<br>[getSkypeForBusinessActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivitycounts.md)<br>[getSkypeForBusinessActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivityusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageusercounts.md)<br>[getSkypeForBusinessOrganizerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivitycounts.md)<br>[getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md)<br>[getSkypeForBusinessParticipantActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivitycounts.md)<br>[getSkypeForBusinessParticipantActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md)<br>[getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md)<br>[getYammerActivityUserDetail](../api-reference/beta/api/reportroot_getyammeractivityuserdetail.md)<br>[getYammerActivityCounts](../api-reference/beta/api/reportroot_getyammeractivitycounts.md)<br>[getYammerActivityUserCounts](../api-reference/beta/api/reportroot_getyammeractivityusercounts.md)<br>[getYammerDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getyammerdeviceusageuserdetail.md)<br>[getYammerDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusagedistributionusercounts.md)<br>[getYammerDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusageusercounts.md)<br>[getYammerGroupsActivityDetail](../api-reference/beta/api/reportroot_getyammergroupsactivitydetail.md)<br>[getYammerGroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitygroupcounts.md)<br>[getYammerGroupsActivityCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitycounts.md) |

### <a name="webhooks"></a>Webhooks

| 変更の種類 | バージョン | 説明                              |
|:------------|:--------|:-----------------------------------------|
| 重大な変更 | ベータ版および v1.0 | ドライブ ルート項目の [webhooks](../api-reference/v1.0/resources/webhooks.md) [サブスクリプション有効期限の最大長](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type) の短縮。 新しい値はドライブ ルート項目用にサポートされている最大有効期限です。 | 

## <a name="october-2017"></a>2017 年 10 月

### <a name="azure-ad-apis"></a>Azure AD API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
|追加|ベータ版|[identityProvider](../api-reference/beta/resources/identityprovider.md) エンティティと、[作成](../api-reference/beta/api/identityprovider_post_identityproviders.md)、[一覧表示](../api-reference/beta/api/identityprovider_list.md)、[取得](../api-reference/beta/api/identityprovider_get.md)、[更新](../api-reference/beta/api/identityprovider_update.md)、および[削除](../api-reference/beta/api/identityprovider_delete.md)操作を追加しました。|


### <a name="microsoft-intune-apis"></a>Microsoft Intune API
|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新しいエンティティを追加しました。<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionlockdevicewithpasscode)<br/>[iosLobAppProvisioningConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfigurationassignment)<br/>[iosVppEBookAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_iosvppebookassignment)<br/>[managedDeviceMobileAppConfigurationAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationassignment)<br/>[managedEBookAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebookassignment)<br/>[managedMobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedmobileapp)<br/>[mobileAppAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappassignment)<br/>[termsAndConditionsAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditionsassignment)<br/>[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken)<br/>[windows10PFXImportCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pfximportcertificateprofile)<br/>[windowsAssignedAccessProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsassignedaccessprofile)<br/>[windowsDomainJoinConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdomainjoinconfiguration)<br/>|
|追加|ベータ版|新しい複合型を追加しました。<br/>[iosLobAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappassignmentsettings)<br/>[iosSingleSignOnSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iossinglesignonsettings)<br/>[iosStoreAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosstoreappassignmentsettings)<br/>[iosVppAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosvppappassignmentsettings)<br/>[mobileAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappassignmentsettings)<br/>[proxiedDomain](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_proxieddomain)<br/>[windowsInformationProtectionProxiedDomainCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionproxieddomaincollection)<br/>[windowsStoreForBusinessAppAssignmentSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessappassignmentsettings)<br/>|
|追加|ベータ版|[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_mobileapp_assign.md) アクションを追加しました |
|追加|ベータ版|[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign.md) アクションを追加しました |
|追加|ベータ版|[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_manageddevicemobileappconfiguration_assign.md) アクションを追加しました |
|追加|ベータ版|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_assign.md) アクションを追加しました |
|追加|ベータ版|[deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) に [assignedAccessMultiModeProfiles](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_assignedaccessmultimodeprofiles.md) アクションを追加しました |
|追加|ベータ版|[vppToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken) に [syncLicenses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_vpptoken_synclicenses.md) アクションを追加しました |
|追加|ベータ版|[managedAppPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) に [targetApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_managedapppolicy_targetapps.md) アクションを追加しました |
|追加|ベータ版|[managedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) に [targetApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_managedappprotection_targetapps.md) アクションを追加しました |
|追加|ベータ版|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) に [targetApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_targetapps.md) アクションを追加しました |
|追加|ベータ版|[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_books_managedebook_assign.md) アクションを追加しました |
|削除|ベータ版|次のエンティティを削除しました。<br/>**cloudPkiSubscription**<br/>|
|削除|ベータ版|次の複合型を削除しました。<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|変更|ベータ版|[androidDeviceComplianceLocalActionBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionbase) エンティティに **gracePeriodInMinutes** プロパティを追加しました|
|変更|ベータ版|[androidForWorkVpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration) エンティティから **enableSplitTunneling** プロパティを削除しました|
|変更|ベータ版|[androidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp) エンティティにプロパティ **versionName** および **versionCode** を追加しました|
|変更|ベータ版|[androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティにプロパティ **minimumRequiredPatchVersion** および **minimumWarningPatchVersion** を追加しました|
|変更|ベータ版|[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティにプロパティ **minimumRequiredPatchVersion** および **minimumWarningPatchVersion** を追加しました|
|変更|ベータ版|[deviceCompliancePolicyAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicyassignment) エンティティに **target** プロパティを追加しました|
|変更|ベータ版|[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) エンティティに **singleSignOnSettings** プロパティを追加しました|
|変更|ベータ版|[iosLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp) エンティティにプロパティ **versionNumber** および **buildNumber** を追加しました|
|変更|ベータ版|[iosVppApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) エンティティに **bundleId** プロパティを追加しました|
|変更|ベータ版|[iosWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration) エンティティに、プロパティ **preSharedKey** を追加しました|
|変更|ベータ版|[managedAndroidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp) エンティティにプロパティ **versionName** および **versionCode** を追加しました|
|変更|ベータ版|[managedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) エンティティに **periodBeforePinReset** プロパティを追加しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティにプロパティ **subscriberCarrier**、**meid**、**totalStorageSpaceInBytes** および **freeStorageSpaceInBytes** を追加しました|
|変更|ベータ版|[managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティから **enrollmentType** プロパティを削除しました|
|変更|ベータ版|[managedIOSLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp) エンティティにプロパティ **versionNumber** および **buildNumber** を追加しました|
|変更|ベータ版|[mobileAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) エンティティに **displayVersion** プロパティを追加しました|
|変更|ベータ版|[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_organization) エンティティから、プロパティ **defaultDeviceEnrollmentRestrictions**、**defaultDeviceEnrollmentWindowsHelloForBusinessSettings** および **defaultDeviceEnrollmentLimit** を削除しました|
|変更|ベータ版|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティに **isAssigned** プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappprotection) エンティティに **isAssigned** プロパティを追加しました|
|変更|ベータ版|[windows10CompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy) エンティティにプロパティ **activeFirewallRequired**、**uacRequired**、**defenderEnabled**、**defenderVersion**、**signatureOutOfDate** および **rtpEnabled** を追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティにプロパティ **assignedAccessSingleModeUserName**、**assignedAccessSingleModeAppUserModelId**、**microsoftAccountSignInAssistantSettings**、**authenticationAllowSecondaryDevice**、**cryptographyAllowFipsAlgorithmPolicy**、**securityBlockAzureADJoinedDevicesAutoEncryption**、**systemTelemetryProxyServer**、**inkWorkspaceAccess**、**inkWorkspaceBlockSuggestedApps**、**defenderCloudBlockLevel** および **defenderCloudExtendedTimeout** を追加しました|
|変更|ベータ版|[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) エンティティにプロパティ **protectedApps**、**enterpriseProxiedDomains** および **isAssigned** を追加しました|
|変更|ベータ版|[windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) エンティティに **productVersion** プロパティを追加しました|
|変更|ベータ版|[androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **vppTokens** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[deviceCompliancePolicyAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicyassignment) エンティティから **deviceCompliancePolicy** ナビゲーション プロパティを削除しました|
|変更|ベータ版|[deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment) エンティティに **deviceCompliancePolicy** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) エンティティに **identityCertificateForClientAuthentication** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティに **apps** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[termsAndConditions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditions) エンティティに **assignments** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに **assignedAccessMultiModeProfiles** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) エンティティに **protectedAppLockerFiles** ナビゲーション プロパティを追加しました|
|変更|ベータ版|[airPrintDestination](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination) 複合型にプロパティ **port** および **forceTls** を追加しました|
|変更|ベータ版|[deviceCompliancePolicySettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 複合型で次のプロパティの型を変更しました: <br/>**errorCode** を Int32 から Int64 に変更しました<br/>|
|変更|ベータ版|[deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 複合型で次のプロパティの型を変更しました: <br/>**errorCode** を Int32 から Int64 に変更しました<br/>|
|変更|ベータ版|[windowsNetworkIsolationPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationpolicy) 複合型で次のプロパティの型を変更しました: <br/>**enterpriseCloudResources** を [windowsNetworkIsolationCloudResourceCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationCloudResourceCollection.md) から [proxiedDomain](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_proxieddomain) コレクションに変更しました<br/>**enterpriseInternalProxyServers** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>**enterpriseIPRanges** を windowsNetworkIsolationIPRangeCollection から [ipRange](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange) コレクションに変更しました<br/>**enterpriseNetworkDomainNames** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>**enterpriseProxyServers** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>**neutralDomainResources** を windowsNetworkIsolationResourceCollection から String コレクションに変更しました<br/>|

### <a name="microsoft-teams-apis"></a>Microsoft Teams API

|変更の種類|バージョン|説明|
|:---|:---|:---|
|追加|ベータ版|新たに [team](../api-reference/beta/resources/team.md) エンティティを追加しました。|
|追加|ベータ版|[team](../api-reference/beta/resources/team.md) エンティティに [create](../api-reference/beta/api/team_put_teams.md)、[get](../api-reference/beta/api/team_get.md)、[update](../api-reference/beta/api/team_update.md) 操作を追加しました。|

### <a name="outlook-messages"></a>Outlook メッセージ

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | この動作の機能強化は、ユーザーがサインインしているユーザーとメール フォルダーを共有しているとき、またはサインインしているユーザーにユーザーのメールボックスを委任しているときに、共有のメール フォルダーやメッセージ コンテンツを取得することに関するものです。 このような状況で、アプリは、サインインしているユーザーが委任されたアクセス許可を提供している間、ユーザーの ID またはユーザー プリンシパル名を指定して、[その共有メール フォルダーを取得する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/mailfolder_get)ことや、[その共有予定表のメッセージを取得する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_messages)ことができます。 |


### <a name="outlook-user-choices"></a>Outlook のユーザーの選択

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
|追加 | ベータ版 | [mailboxSettings](../api-reference/beta/resources/mailboxsettings.md) に新しい **workingHours** プロパティを追加しました。 サポートされるユース ケースについては、「[workingHours リソース タイプ](../api-reference/beta/resources/workinghours.md)」を参照してください。|
|追加 | ベータ版 | 次の新しい複合型を追加しました。 <br> [workingHours](../api-reference/beta/resources/workinghours.md) <br> [timeZoneBase](../api-reference/beta/resources/timezonebase.md) <br> [customTimeZone](../api-reference/beta/resources/customtimezone.md) <br> [standardTimeZoneOffset](../api-reference/beta/resources/standardtimezoneoffset.md) <br> [daylightTimeZoneOffset](../api-reference/beta/resources/daylighttimezoneoffset.md)|


### <a name="reports-apis"></a>レポート API
| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 変更      | ベータ版    | [getEmailActivityUserDetail](../api-reference/beta/api/reportroot_getemailactivityuserdetail.md)、[getEmailActivityCounts](../api-reference/beta/api/reportroot_getemailactivitycounts.md)、および [getEmailActivityUserCounts](../api-reference/beta/api/reportroot_getemailactivityusercounts.md) API を追加しました。 EmailActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getEmailAppUsageUserDetail](../api-reference/beta/api/reportroot_getemailappusageuserdetail.md)、[getEmailAppUsageAppsUserCounts](../api-reference/beta/api/reportroot_getemailappusageappsusercounts.md)、[getEmailAppUsageUserCounts](../api-reference/beta/api/reportroot_getemailappusageusercounts.md)、および [getEmailAppUsageVersionsUserCounts](../api-reference/beta/api/reportroot_getemailappusageversionsusercounts.md) API を追加しました。 EmailAppUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getMailboxUsageDetail](../api-reference/beta/api/reportroot_getmailboxusagedetail.md)、[getMailboxUsageMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagemailboxcounts.md)、[getMailboxUsageQuotaStatusMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagequotastatusmailboxcounts.md)、および [getMailboxUsageStorage](../api-reference/beta/api/reportroot_getmailboxusagestorage.md) API を追加しました。 MailboxUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOffice365ActivationsUserDetail](../api-reference/beta/api/reportroot_getoffice365activationsuserdetail.md)、[getOffice365ActivationCounts](../api-reference/beta/api/reportroot_getoffice365activationcounts.md)、および [getOffice365ActivationsUserCounts](../api-reference/beta/api/reportroot_getoffice365activationsusercounts.md) API を追加しました。 Office365Activations API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOffice365ActiveUserDetail](../api-reference/beta/api/reportroot_getoffice365activeuserdetail.md)、[getOffice365ActiveUserCounts](../api-reference/beta/api/reportroot_getoffice365activeusercounts.md)、および [getOffice365ServicesUserCounts](../api-reference/beta/api/reportroot_getoffice365servicesusercounts.md) API を追加しました。 Office365ActiveUser API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOffice365GroupsActivityDetail](../api-reference/beta/api/reportroot_getoffice365groupsactivitydetail.md)、[getOffice365GroupsActivityCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitycounts.md)、[getOffice365GroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitygroupcounts.md)、[getOffice365GroupsActivityStorage](../api-reference/beta/api/reportroot_getoffice365groupsactivitystorage.md)、および [getOffice365GroupsActivityFileCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivityfilecounts.md) API を追加しました。 Office365GroupsActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOneDriveActivityUserDetail](../api-reference/beta/api/reportroot_getonedriveactivityuserdetail.md)、[getOneDriveActivityUserCounts](../api-reference/beta/api/reportroot_getonedriveactivityusercounts.md)、および [getOneDriveActivityFileCounts](../api-reference/beta/api/reportroot_getonedriveactivityfilecounts.md) API を追加しました。 OneDriveActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getOneDriveUsageAccountDetail](../api-reference/beta/api/reportroot_getonedriveusageaccountdetail.md)、[getOneDriveUsageAccountCounts](../api-reference/beta/api/reportroot_getonedriveusageaccountcounts.md), [getOneDriveUsageFileCounts](../api-reference/beta/api/reportroot_getonedriveusagefilecounts.md)、および [getOneDriveUsageStorage](../api-reference/beta/api/reportroot_getonedriveusagestorage.md) API を追加しました。 OneDriveUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSharePointActivityUserDetail](../api-reference/beta/api/reportroot_getsharepointactivityuserdetail.md)、[getSharePointActivityFileCounts](../api-reference/beta/api/reportroot_getsharepointactivityfilecounts.md)、[getSharePointActivityUserCounts](../api-reference/beta/api/reportroot_getsharepointactivityusercounts.md)、および [getSharePointActivityPages](../api-reference/beta/api/reportroot_getsharepointactivitypages.md) API を追加しました。 SharePointActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSharePointSiteUsageDetail](../api-reference/beta/api/reportroot_getsharepointsiteusagedetail.md)、[getSharePointSiteUsageFileCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagefilecounts.md)、[getSharePointSiteUsageSiteCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagesitecounts.md)、[getSharePointSiteUsageStorage](../api-reference/beta/api/reportroot_getsharepointsiteusagestorage.md)、および [getSharePointSiteUsagePages](../api-reference/beta/api/reportroot_getsharepointsiteusagepages.md) API を追加しました。 SharePointSiteUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessActivityUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessactivityuserdetail.md)、[getSkypeForBusinessActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivitycounts.md)、および [getSkypeForBusinessActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivityusercounts.md) API を追加しました。 SfbActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md)、[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md)、および [getSkypeForBusinessDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageusercounts.md) API を追加しました。 SfbDeviceUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessOrganizerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivitycounts.md)、[getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md)、および [getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md) API を追加しました。 SfbOrganizerActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessParticipantActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivitycounts.md)、[getSkypeForBusinessParticipantActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md)、および [getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md) API を追加しました。 SfbParticipantActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md)、[getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md)、および [getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md) API を追加しました。 SfbP2PActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getYammerActivityUserDetail](../api-reference/beta/api/reportroot_getyammeractivityuserdetail.md)、[getYammerActivityCounts](../api-reference/beta/api/reportroot_getyammeractivitycounts.md)、および [getYammerActivityUserCounts](../api-reference/beta/api/reportroot_getyammeractivityusercounts.md) API を追加しました。 YammerActivity API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getYammerDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getyammerdeviceusageuserdetail.md)、[getYammerDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusagedistributionusercounts.md)、および [getYammerDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusageusercounts.md) API を追加しました。 YammerDeviceUsage API は、これらにより置き換えられました。 |
| 変更      | ベータ版    | [getYammerGroupsActivityDetail](../api-reference/beta/api/reportroot_getyammergroupsactivitydetail.md)、[getYammerGroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitygroupcounts.md)、および [getYammerGroupsActivityCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitycounts.md) API を追加しました。 YammerGroupsActivity API は、これらにより置き換えられました。 |



## <a name="september-2017"></a>2017 年 9 月

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_activedirectorywindowsautopilotdeploymentprofile.md)<br/>[azureADWindowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_azureadwindowsautopilotdeploymentprofile.md)<br/>[deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md)<br/>[deviceEnrollmentLimitConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)<br/>[deviceManagementPartner](../api-reference/beta/resources/intune_onboarding_devicemanagementpartner.md)<br/>[enrollmentConfigurationAssignment](../api-reference/beta/resources/intune_onboarding_enrollmentconfigurationassignment.md)<br/>[windows10EnrollmentCompletionPageConfiguration](../api-reference/beta/resources/intune_onboarding_windows10enrollmentcompletionpageconfiguration.md)<br/>[windows10NetworkBoundaryConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10networkboundaryconfiguration.md)<br/>[windowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile.md)<br/>[windowsAutopilotDeviceIdentity](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeviceidentity.md)<br/>[windowsAutopilotSettings](../api-reference/beta/resources/intune_enrollment_windowsautopilotsettings.md)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[adminConsent](../api-reference/beta/resources/intune_devices_adminconsent.md)<br/>[allDevicesAssignmentTarget](../api-reference/beta/resources/intune_shared_alldevicesassignmenttarget.md)<br/>[allLicensedUsersAssignmentTarget](../api-reference/beta/resources/intune_shared_alllicensedusersassignmenttarget.md)<br/>[deviceAndAppManagementAssignmentTarget](../api-reference/beta/resources/intune_shared_deviceandappmanagementassignmenttarget.md)<br/>[deviceEnrollmentPlatformRestriction](../api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestriction.md)<br/>[deviceHealthAttestationState](../api-reference/beta/resources/intune_devices_devicehealthattestationstate.md)<br/>[exclusionGroupAssignmentTarget](../api-reference/beta/resources/intune_shared_exclusiongroupassignmenttarget.md)<br/>[groupAssignmentTarget](../api-reference/beta/resources/intune_shared_groupassignmenttarget.md)<br/>[outOfBoxExperienceSettings](../api-reference/beta/resources/intune_enrollment_outofboxexperiencesettings.md)<br/>[windowsFirewallNetworkProfile](../api-reference/beta/resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationpolicy.md)<br/>windowsNetworkIsolationResourceCollection<br/> |
| 追加    | ベータ版    | [windowsAutopilotSettings](../api-reference/beta/resources/intune_enrollment_windowsautopilotsettings.md) に [sync](../api-reference/beta/api/intune_enrollment_windowsautopilotsettings_sync.md) アクションを追加しました |
| 追加    | ベータ版    | [windowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile.md) に [assign](../api-reference/beta/api/intune_enrollment_windowsautopilotdeploymentprofile_assign.md) アクションを追加しました |
| 追加    | ベータ版    | [deviceCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy.md) に localActions アクションを追加しました |
| 追加    | ベータ版    | [deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md) に [setPriority](../api-reference/beta/api/intune_onboarding_deviceenrollmentconfiguration_setpriority.md) アクションを追加しました |
| 追加    | ベータ版    | [deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md) に [assign](../api-reference/beta/api/intune_onboarding_deviceenrollmentconfiguration_assign.md) アクションを追加しました |
| 追加    | ベータ版    | [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md) コレクションに uploadDepToken アクションを追加しました |
| 追加    | ベータ版    | [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md) コレクションに syncWithAppleDeviceEnrollmentProgram アクションを追加しました |
| 追加    | ベータ版    | [managedAppProtection](../api-reference/beta/resources/intune_mam_managedappprotection.md) に updateMobileAppIdentifierDeployments アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppProtection](../api-reference/beta/resources/intune_mam_targetedmanagedappprotection.md) に assign アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppConfiguration](../api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration.md) に assign アクションを追加しました |
| 追加    | ベータ版    | [windowsInformationProtection](../api-reference/beta/resources/intune_mam_windowsinformationprotection.md) に assign アクションを追加しました |
| 追加    | ベータ版    | [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md) コレクションに getEncryptionPublicKey 関数を追加しました |
| 変更      | ベータ版    | [androidCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy.md) エンティティに、プロパティ **requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity**、**conditionStatementId** を追加しました |
| 変更      | ベータ版    | [androidForWorkCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy.md) エンティティに、プロパティ **requireAppVerify**、**requireSafetyNetAttestationBasicIntegrity**、**requireSafetyNetAttestationCertifiedDevice**、**requireGooglePlayServices**、**requireUpToDateSecurityProviders**、**requireCompanyPortalAppIntegrity** を追加しました |
| 変更      | ベータ版    | [androidForWorkGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration.md) エンティティに、プロパティ **blockCrossProfileCopyPaste** と **requireAppVerify** を追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) エンティティに、プロパティ **kioskModeApps** と **requireAppVerify** を追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) エンティティから、プロパティ **kioskModeManagedApps** を削除しました |
| 変更      | ベータ版    | cloudPkiSubscription エンティティから、プロパティ **cloudPkiProvider**、**createdDateTime**、**description**、**lastModifiedDateTime**、**displayName**、**syncStatus**、**lastSyncError**、**lastSyncDateTime**、**credentials**、**trustedRootCertificate**、**version** を削除しました |
| 変更      | ベータ版    | [deviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_deviceconfiguration.md) エンティティから、プロパティ **assignmentStatus**、**assignmentProgress**、**assignmentErrorMessage** を削除しました |
| 変更      | ベータ版    | [deviceManagement](../api-reference/beta/resources/intune_shared_devicemanagement.md) エンティティに、**adminConsent** プロパティを追加しました |
| 変更      | ベータ版    | [iosVppApp](../api-reference/beta/resources/intune_apps_iosvppapp.md) エンティティに、プロパティ **vppTokenOrganizationName**、**vppTokenAccountType**、**vppTokenAppleId** を追加しました |
| 変更      | ベータ版    | [managedDevice](../api-reference/beta/resources/intune_devices_manageddevice.md) エンティティに、プロパティ **deviceEnrollmentType**、**wiFiMacAddress**、**deviceHealthAttestationState** を追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfiguration](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration.md) エンティティに、プロパティ **legacyAppConfiguration** を追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfigurationDeviceSummary](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) エンティティに、プロパティ **notApplicableCount** を追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfigurationUserSummary](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) エンティティに、プロパティ **notApplicableCount** を追加しました |
| 変更      | ベータ版    | [windows10EndpointProtectionConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) エンティティに、プロパティ **firewallBlockStatefulFTP**、**firewallIdleTimeoutForSecurityAssociationInSeconds**、**firewallPreSharedKeyEncodingMethod**、**firewallIPSecExemptionsAllowNeighborDiscovery**、**firewallIPSecExemptionsAllowICMP**、**firewallIPSecExemptionsAllowRouterDiscovery**、**firewallIPSecExemptionsAllowDHCP**、**firewallCertificateRevocationListCheckMethod**、**firewallMergeKeyingModuleSettings**、**firewallPacketQueueingMethod**、**firewallProfileDomain**、**firewallProfilePublic**、**firewallProfilePrivate**、**defenderAttackSurfaceReductionExcludedPaths**、**defenderOfficeAppsOtherProcessInjectionType**、**defenderOfficeAppsExecutableContentCreationOrLaunchType**、**defenderOfficeAppsLaunchChildProcessType**、**defenderOfficeMacroCodeAllowWin32ImportsType**、**defenderScriptObfuscatedMacroCodeType**、**defenderScriptDownloadedPayloadExecutionType**、**defenderEmailContentExecutionType**、**defenderGuardMyFoldersType**、**defenderGuardedFoldersAllowedAppPaths**、**defenderAdditionalGuardedFolders**、**defenderNetworkProtectionType**、**defenderExploitProtectionXml**、**defenderExploitProtectionXmlFileName**、**defenderSecurityCenterBlockExploitProtectionOverride**、**appLockerApplicationControl**、**applicationGuardBlockClipboardSharing**、**applicationGuardAllowPrintToPDF**、**applicationGuardAllowPrintToXPS**、**applicationGuardAllowPrintToLocalPrinters**、**applicationGuardAllowPrintToNetworkPrinters**、**bitLockerDisableWarningForOtherDiskEncryption** を追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration.md) エンティティに、プロパティ **displayAppListWithGdiDPIScalingTurnedOn**、**displayAppListWithGdiDPIScalingTurnedOff**、**messagingBlockSync**、**messagingBlockMMS**、**messagingBlockRichCommunicationServices** を追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration.md) エンティティから、プロパティ **bluetoothDeviceName** を削除しました |
| 変更      | ベータ版    | [windows10TeamGeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) エンティティから、プロパティ **deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation**、**deviceAccountSessionInitiationProtocolAddress** を削除しました |
| 変更      | ベータ版    | [androidCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy.md) エンティティに、ナビゲーション プロパティ **localActions** を追加しました |
| 変更      | ベータ版    | [deviceManagement](../api-reference/beta/resources/intune_shared_devicemanagement.md) エンティティに、ナビゲーション プロパティ **windowsAutopilotSettings**、**windowsAutopilotDeviceIdentities**、**windowsAutopilotDeploymentProfiles**、**deviceEnrollmentConfigurations**、**deviceManagementPartners**、**depOnboardingSettings** を追加しました |
| 変更      | ベータ版    | [deviceManagement](../api-reference/beta/resources/intune_shared_devicemanagement.md) エンティティから、ナビゲーション プロパティ **cloudPkiSubscriptions** を削除しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](../api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration.md) エンティティに、ナビゲーション プロパティ **assignments** を追加しました |
| 変更      | ベータ版    | [targetedManagedAppProtection](../api-reference/beta/resources/intune_mam_targetedmanagedappprotection.md) エンティティに、ナビゲーション プロパティ **assignments** を追加しました |
| 変更      | ベータ版    | [windowsInformationProtection](../api-reference/beta/resources/intune_mam_windowsinformationprotection.md) エンティティに、ナビゲーション プロパティ **assignments** を追加しました |

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

[Drive]: ../api-reference/v1.0/resources/drive.md
[DriveItem]: ../api-reference/v1.0/resources/driveitem.md
[SharedDriveItem]: ../api-reference/v1.0/resources/shareddriveitem.md
[FolderView]: ../api-reference/v1.0/resources/folderview.md
[Folder]: ../api-reference/v1.0/resources/folder.md
[ItemReference]: ../api-reference/v1.0/resources/itemreference.md
[Video]: ../api-reference/v1.0/resources/video.md
[Drive-beta]: ../api-reference/beta/resources/drive.md
[DriveItem-beta]: ../api-reference/beta/resources/driveitem.md
[DriveItemVersion-beta]: ../api-reference/beta/resources/driveitemversion.md
[ItemActivity-beta]: ../api-reference/beta/resources/itemactivity.md
[CommentAction-beta]: ../api-reference/beta/resources/commentaction.md
[CreateAction-beta]: ../api-reference/beta/resources/createaction.md
[DeleteAction-beta]: ../api-reference/beta/resources/deleteaction.md
[EditAction-beta]: ../api-reference/beta/resources/editaction.md
[ItemActionSet-beta]: ../api-reference/beta/resources/itemactionset.md
[ItemActivityTimeSet-beta]: ../api-reference/beta/resources/itemactivitytimeset.md
[MentionAction-beta]: ../api-reference/beta/resources/mentionaction.md
[MoveAction-beta]: ../api-reference/beta/resources/moveaction.md
[PublicationFacet-beta]: ../api-reference/beta/resources/publicationfacet.md
[RenameAction-beta]: ../api-reference/beta/resources/renameaction.md
[RestoreAction-beta]: ../api-reference/beta/resources/restoreaction.md
[ShareAction-beta]: ../api-reference/beta/resources/shareaction.md
[VersionAction-beta]: ../api-reference/beta/resources/versionaction.md
[ItemReference-beta]: ../api-reference/beta/resources/itemreference.md
[SharepointIds-beta]: ../api-reference/beta/resources/sharepointids.md
[Video-beta]: ../api-reference/beta/resources/video.md
[CheckIn-beta]: ../api-reference/beta/api/driveitem_checkin.md
[CheckOut-beta]: ../api-reference/beta/api/driveitem_checkout.md
[CreateLink-beta]: ../api-reference/beta/api/driveitem_createlink.md


### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | ベータ版          | [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/user) エンティティに、関数 [findRoomLists](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_findroomlists) と [findRooms](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_findrooms) を追加しました。 |
| 追加        | ベータ版          | **locations** プロパティが [event](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/event) エンティティに追加され、出席者が複数の場所から出席できるイベントを編成できるようになりました。 |
| 追加        | ベータ版          | **locationType** プロパティが [location](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/location) 複合型に追加されました。 |
| 追加        | ベータ版          | **uniqueId** および **uniqueIdType** プロパティが [location](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/location) 複合型に追加されました。 これらのプロパティは、現時点では内部使用に限られます。 |
| 変更          | v1.0 およびベータ版 | この動作の機能強化は、ユーザーがサインインしているユーザーと予定表を共有しているとき、またはサインインしているユーザーにユーザーのメールボックスを委任しているときに、共有の予定表やイベント コンテンツを取得することに関するものです。 このような状況で、アプリは、サインインしているユーザーが委任されたアクセス許可を提供している間、ユーザーの ID またはユーザー プリンシパル名を指定して、[その共有予定表を取得する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/calendar_get)ことや、[その共有予定表のイベントを取得する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_events)ことができます。 |

### <a name="outlook-contacts"></a>Outlook の連絡先

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | この動作の機能強化は、ユーザーがサインインしているユーザーと連絡先フォルダーを共有しているとき、またはサインインしているユーザーにユーザーのメールボックスを委任しているときに、共有の連絡先フォルダーや連絡先コンテンツを取得することに関するものです。 このような状況で、アプリは、サインインしているユーザーが委任されたアクセス許可を提供している間、ユーザーの ID またはユーザー プリンシパル名を指定して、[その共有連絡先フォルダーを取得する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/contactfolder_get)ことや、[その共有フォルダーの連絡先を取得する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_contacts)ことができます。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [message](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/message) エンティティに、プロパティ **internetMessageHeaders** を追加しました。 |
| 追加        | ベータ版        | [internetMessageHeader](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/internetmessageheader) 複合型を追加しました。 |
| 追加        | ベータ版        | [mailFolder](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/mailfolder) エンティティに、ナビゲーション プロパティ **messageRules** を追加しました。 **messageRules** は [messageRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/messagerule) インスタンスのコレクションです。 |
| 追加        | ベータ版        | [messageRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/messagerule) エンティティと、[messageRuleActions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/messageruleactions)、[messageRulePredicates](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/messagerulepredicates)、[sizeRange](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/sizerange) 複合型が追加されました。 |
| 追加        | ベータ版        | メッセージ ルールに次の CRUD 操作が追加されました: [create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/mailfolder_post_messagerules)、[list](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/mailfolder_list_messagerules)、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/messagerule_get)、[update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/messagerule_update)、[delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/messagerule_delete)。 |


### <a name="outlook-user-choices"></a>Outlook のユーザーの選択

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [outlookUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookuser) エンティティに、新しい **masterCategories** ナビゲーション プロパティを追加しました。 **masterCategories** は [outlookCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookCategory) オブジェクトのコレクションです。 |
| 追加        | ベータ版        | [outlookCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookCategory) エンティティを追加しました。 |
| 追加        | ベータ版        | [outlookCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookCategory) に次の CRUD 操作を追加しました: [create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/outlookuser_post_mastercategories)、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/outlookcategory_get)、[update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/outlookcategory_update)、[delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/outlookcategory_delete)。 |
| 追加        | ベータ版        | 新しい [supportedLanguages](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/outlookuser_supportedlanguages) 関数が [outlookUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookuser) エンティティに追加されました。 |
| 追加        | ベータ版        | [outlookUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookuser) エンティティに、新しい [supportedTimeZones](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/outlookuser_supportedtimezones) 関数を追加しました。 |


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

[BaseItemVersion-beta]: ../api-reference/beta/resources/baseitemversion.md
[BooleanColumn-beta]:  ../api-reference/beta/resources/booleanColumn.md
[BooleanColumn]: ../api-reference/v1.0/resources/booleancolumn.md
[CalculatedColumn]: ../api-reference/v1.0/resources/calculatedcolumn.md
[ChoiceColumn]: ../api-reference/v1.0/resources/choicecolumn.md
[ColumnDefinition-beta]: ../api-reference/beta/resources/columndefinition.md
[ColumnDefinition]: ../api-reference/v1.0/resources/columndefinition.md
[ColumnLink-beta]: ../api-reference/beta/resources/columnLink.md
[ColumnLink]: ../api-reference/v1.0/resources/columnLink.md
[ContentType-beta]: ../api-reference/beta/resources/contentType.md
[ContentType]: ../api-reference/v1.0/resources/contentType.md
[ContentTypeInfo-beta]: ../api-reference/beta/resources/contentTypeInfo.md
[ContentTypeInfo]: ../api-reference/v1.0/resources/contentTypeInfo.md
[ContentTypeOrder-beta]: ../api-reference/beta/resources/contentTypeOrder.md
[ContentTypeOrder]: ../api-reference/v1.0/resources/contentTypeOrder.md
[CurrencyColumn-beta]: ../api-reference/beta/resources/currencycolumn.md
[CurrencyColumn]: ../api-reference/v1.0/resources/currencycolumn.md
[DateTimeColumn]: ../api-reference/v1.0/resources/datetimecolumn.md
[DefaultColumnValue]: ../api-reference/v1.0/resources/defaultColumnValue.md
[List-beta]: ../api-reference/beta/resources/list.md
[List]: ../api-reference/v1.0/resources/list.md
[ListInfo-beta]: ../api-reference/beta/resources/listinfo.md
[ListInfo]: ../api-reference/v1.0/resources/listinfo.md
[ListItem-beta]: ../api-reference/beta/resources/listitem.md
[ListItem]: ../api-reference/v1.0/resources/listitem.md
[ListItemVersion-beta]: ../api-reference/beta/resources/listitemversion.md
[LookupColumn-beta]: ../api-reference/beta/resources/lookupColumn.md
[LookupColumn]: ../api-reference/v1.0/resources/lookupcolumn.md
[NumberColumn-beta]: ../api-reference/beta/resources/numberColumn.md
[NumberColumn]: ../api-reference/v1.0/resources/numbercolumn.md
[PersonOrGroupColumn-beta]: ../api-reference/beta/resources/personOrGroupColumn.md
[PersonOrGroupColumn]: ../api-reference/v1.0/resources/personorgroupcolumn.md
[Site-beta]: ../api-reference/beta/resources/site.md
[Site]: ../api-reference/v1.0/resources/site.md
[SystemFacet-beta]: ../api-reference/beta/resources/systemfacet.md
[SystemFacet]: ../api-reference/v1.0/resources/systemFacet.md
[TextColumn]: ../api-reference/v1.0/resources/textcolumn.md


### <a name="sharepoint-sites"></a>SharePoint サイト

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [SiteCollection][SiteCollection-beta] 複合型に、プロパティ **dataLocationCode** と **root** を追加しました。 |

[SiteCollection-beta]: ../api-reference/beta/resources/sitecollection.md


## <a name="august-2017"></a>2017 年 8 月

### <a name="group-lifecycle-policy"></a>グループのライフサイクル ポリシー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [groupLifecyclePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/grouplifecyclepolicy) エンティティを追加しました。 |
| 追加        | ベータ版        | グループのライフサイクル ポリシーに、次の API を追加しました。[create](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_post_grouplifecyclepolicies)、[list](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_list)、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_get)、[update](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_update)、[delete](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_delete)、[add group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_addgroup)、[remove group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_removegroup)、および [renew a group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/grouplifecyclepolicy_renewgroup)。 |
| 追加        | ベータ版        | [group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/group) エンティティに [List groupLifecylePolicies](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/group_list_grouplifecyclepolicies.md) 関数を追加しました。 |

### <a name="intune-apis"></a>Intune API
| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 追加された新しいエンティティ:<br/>[windowsPrivacyDataAccessControlItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsprivacydataaccesscontrolitem)<br/> |
| 追加    | ベータ版    | 追加された新しい複合型:<br/>[configurationManagerClientEnabledFeatures](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_configurationmanagerclientenabledfeatures)<br/>[windowsDefenderScanActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_windowsdefenderscanactionresult)<br/> |
| 追加    | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [windowsDefenderScan](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_windowsdefenderscan.md) アクションを追加しました |
| 追加    | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [windowsDefenderUpdateSignatures](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md) アクションを追加しました |
| 追加    | ベータ版    | [deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) に [windowsPrivacyAccessControls](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_windowsprivacyaccesscontrols.md) アクションを追加しました |
| 変更      | ベータ版    | [appleVolumePurchaseProgramToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) エンティティに **automaticallyUpdateApps** および **countryOrRegion** プロパティを追加しました |
| 変更      | ベータ版    | [depEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) エンティティに **enableAuthenticationViaCompanyPortal** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceActionItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) エンティティに **notificationMessageCCList** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) エンティティに **notApplicableCount** プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **configurationManagerClientEnabledFeatures** プロパティを追加しました |
| 変更      | ベータ版    | [organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_organization) エンティティから **intuneBrand** プロパティを削除しました |
| 変更      | ベータ版    | [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティに **smartScreenEnableInShell**、**smartScreenBlockOverrideForFiles**、**applicationGuardEnabled**、**applicationGuardBlockFileTransfer**、**applicationGuardBlockNonEnterpriseContent**、**applicationGuardAllowPersistence**、および **applicationGuardForceAuditing** プロパティを追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに **searchBlockDiacritics**、**searchDisableAutoLanguageDetection**、**searchDisableIndexingEncryptedItems**、**searchEnableRemoteQueries**、**searchDisableUseLocation**、**searchDisableIndexerBackoff**、**searchDisableIndexingRemovableDrive**、**searchEnableAutomaticIndexSizeManangement**、**smartScreenEnableAppInstallControl**、および **privacyAdvertisingId** プロパティを追加しました |
| 変更      | ベータ版    | [windows10TeamGeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) エンティティから **settingsDeviceName** プロパティを削除しました |
| 変更      | ベータ版    | [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) エンティティから **restartMode** プロパティを削除しました |
| 変更      | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに **detectedApps** および **managedDevices** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに **privacyAccessControls** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型に **secureByDefault** プロパティを追加しました |
| 変更      | ベータ版    | [windowsUpdateScheduledInstall](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdatescheduledinstall) 複合型に **restartMode** プロパティを追加しました |

### <a name="onenote"></a>OneNote

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | [onenote](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/onenote) ナビゲーション プロパティを **site** に追加しました。 |
| 追加        | ベータ版          | コピー操作用にターゲット *siteCollectionId* とターゲット *siteId* パラメーターを追加しました。次に例を示します。[CopyNotebook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/notebook_copynotebook)。 |

### <a name="people"></a>複数のユーザー 

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | v1.0 に [People API](../api-reference/v1.0/resources/person.md) を追加しました。People API の詳細については、「[People の関連情報を取得する](people_example.md)」を参照してください。 |
| 追加        | v1.0        | People.Read.All アクセス許可を追加しました。 詳細については、「[アクセス許可](permissions_reference.md)」を参照してください。 |
| 追加        | v1.0        | [personType](../api-reference/v1.0/resources/persontype.md) リソースを追加しました。 |
| 変更          | v1.0        | [scoredEmailAddress](../api-reference/v1.0/resources/scoredemailaddress.md) リソースが **rankedEmailAddress** リソースに取って代わりました。 |
| 変更          | v1.0        | [person](../api-reference/v1.0/resources/person.md) リソースは次のように更新されました。<ul><li>**scoredEmailAddresses** プロパティ ([scoredEmailAddress](../api-reference/v1.0/resources/scoredemailaddress.md) 型のコレクション) が **emailAddresses** プロパティに取って代わりました</li><li>**jobTitle** プロパティが **title** プロパティに取って代わりました</li><li>**sources** プロパティと **mailboxType** プロパティが削除されました</li><li>**personType** プロパティは現在、文字列型ではなく [personType](../api-reference/v1.0/resources/persontype.md) 型であり、以前の **sources** プロパティと **mailboxType** プロパティの機能に取って代わりました</li><li>**imAddress** プロパティを追加しました</li></ul> |
| 削除        | v1.0        | **personDataSource** リソースが削除されました。 |

### <a name="user"></a>ユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | **employeeId** プロパティを [user](../api-reference/beta/resources/user.md) に追加しました。 |

## <a name="july-2017"></a>2017 年 7 月

### <a name="group-settings"></a>グループ設定

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | グループ設定のサポートを追加しました。<br/>新しいリソースの種類: [groupSetting](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/groupsetting.md)、[groupSettingTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/groupsettingtemplate.md)、[settingValue](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/settingvalue.md)、および [settingTemplateValue](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/settingtemplatevalue.md) |
| 変更          | v1.0        | プロパティ **classification** とナビゲーション プロパティ **settings** を [group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/group.md) に追加しました |

### <a name="intune-apis"></a>Intune API

| 変更の種類&nbsp; | バージョン | 説明                              |
| :--------------- | :------ | :--------------------------------------- |
| 追加         | ベータ版    | [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_iosmobileappconfiguration_assign) アクションを [iosMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) に追加しました |
| 追加         | ベータ版    | [syncDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_syncdevice) アクションを [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に追加しました |
| 変更           | ベータ版    | **appsInstallAllowList**、**appsLaunchBlockList**、**appsHideList** プロパティを [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティに追加しました |
| 変更           | ベータ版    | **disableAppEncryptionIfDeviceEncryptionIsEnabled** プロパティを [androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティに追加しました |
| 変更           | ベータ版    | **disableAppEncryptionIfDeviceEncryptionIsEnabled** プロパティを [defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [deviceComplianceDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [deviceComplianceSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [deviceConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) エンティティに追加しました |
| 変更           | ベータ版    | **subscriptions** プロパティを [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに追加しました |
| 変更           | ベータ版    | **version** プロパティを [deviceManagementExchangeConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeconnector) エンティティに追加しました |
| 変更           | ベータ版    | **utcTimeOffsetInMinutes** プロパティを [iosUpdateConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration) エンティティに追加しました |
| 変更           | ベータ版    | **complianceGracePeriodExpirationDateTime** プロパティを [iosUpdateDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus) エンティティに追加しました |
| 変更           | ベータ版    | **preSharedKey** プロパティを [macOSWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoswificonfiguration) エンティティに追加しました |
| 変更           | ベータ版    | **phoneNumber**、**androidSecurityPatchLevel**、**userDisplayName** プロパティを [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに追加しました |
| 変更           | ベータ版    | **userName**、**deviceModel**、**platform**、**complianceGracePeriodExpirationDateTime** プロパティを [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) エンティティに追加しました |
| 変更           | ベータ版    | **userPrincipalName** プロパティを [mobileAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) エンティティに追加しました |
| 変更           | ベータ版    | **overrideDefaultRule** プロパティを [onPremisesConditionalAccessSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings) エンティティに追加しました |
| 変更           | ベータ版    | **userPrincipalName** プロパティを [userAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_userappinstallstatus) エンティティに追加しました |
| 変更           | ベータ版    | **connectAppBlockAutoLaunch**、**deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation**、**deviceAccountSessionInitiationProtocolAddress**、**settingsBlockMyMeetingsAndFiles**、**settingsBlockSessionResume**、**settingsBlockSigninSuggestions**、**settingsDefaultVolume**、**settingsScreenTimeoutInMinutes**、**settingsSessionTimeoutInMinutes**、**settingsSleepTimeoutInMinutes** プロパティを [windows10TeamGeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) エンティティに追加しました |
| 変更           | ベータ版    | **deploymentSummary** ナビゲーション プロパティを [defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに追加しました |
| 変更           | ベータ版    | **settingName**、**userId**、**userName**、**userEmail**、**currentValue** プロパティを[deviceCompliancePolicySettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 複合型に追加しました |
| 変更           | ベータ版    | [deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 複合型に、**settingName**、**userId**、**userName**、**userEmail**、**currentValue** の各プロパティを追加しました |
| 変更           | ベータ版    | **unknownCount** プロパティを[deviceOperatingSystemSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_deviceoperatingsystemsummary) 複合型に追加しました |



## <a name="june-2017"></a>2017 年 6 月

### <a name="project-rome"></a>Project Rome

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 以下のリソースと API が追加されています。<br/>[アクティビティ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/projectrome_activity)<br/>[アクティビティを作成または置換する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_put_activity)<br/>[アクティビティを削除する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_delete_activity)<br/>[履歴項目](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/projectrome_historyitem)<br/>[履歴項目を作成または置換する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_put_historyitem)<br/>[履歴項目を削除する](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_delete_historyitem) |

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [calendar](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/calendar) の 4 つのプロパティ **canEdit**、**canShare**、**canViewPrivateItems**、および **owner** を v1.0 に昇格しました。 |


### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[defaultDeviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_defaultdevicecompliancepolicy)<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary)<br/>[deviceManagementScriptDeviceState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptdevicestate)<br/>[deviceManagementScriptRunSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptrunsummary)<br/>[deviceManagementScriptUserState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptuserstate)<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus)<br/>[windowsManagedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanageddevice)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate)<br/>[windowsManagementAppHealthSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthsummary)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[bitLockerFixedDrivePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerfixeddrivepolicy)<br/>[bitLockerRecoveryOptions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions)<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerremovabledrivepolicy)<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_deleteuserfromsharedappledeviceactionresult)<br/>[iosNetworkUsageRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnetworkusagerule)<br/> |
| 削除    | ベータ版    | 次のエンティティを削除しました。<br/>**deviceManagementScriptState**<br/> |
| 削除    | ベータ版    | [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_user) の wipeByDeviceTag アクションを削除しました。 |
| 変更      | ベータ版    | [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration) エンティティに、プロパティ **innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap** および **outerIdentityPrivacyTemporaryValue** を追加しました |
| 変更      | ベータ版    | [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap** および **enableOuterIdentityPrivacy** を削除しました |
| 変更      | ベータ版    | [androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [complianceSettingStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/complianceSettingStateSummary) エンティティから、プロパティ **instanceDisplayName** および **settingPlatform** を削除しました |
| 変更      | ベータ版    | [defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment) エンティティに **excludeGroup** プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary) エンティティから、プロパティ **instanceDisplayName** および **settingPlatform** を削除しました |
| 変更      | ベータ版    | [deviceComplianceSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) エントリから、プロパティ **devicePlatform** を削除しました |
| 変更      | ベータ版    | [deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) エンティティに、プロパティ **assignmentStatus**、**assignmentProgress** および **assignmentErrorMessage** を追加しました |
| 変更      | ベータ版    | 
            [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに、プロパティ **intuneBrand** を追加しました |
| 変更      | ベータ版    | [deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) エンティティに、プロパティ **enforceSignatureCheck** および **fileName** を追加しました |
| 変更      | ベータ版    | [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) エンティティに、プロパティ **innerAuthenticationProtocolForEapTtls** および **outerIdentityPrivacyTemporaryValue** を追加しました |
| 変更      | ベータ版    | [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls** および **enableOuterIdentityPrivacy** を削除しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) エンティティに、プロパティ **classroomAppForceUnpromptedScreenObservation**、**keyboardBlockDictation**、**networkUsageRules** および **wiFiConnectOnlyToConfiguredNetworks** を追加しました |
| 変更      | ベータ版    | [iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [iosWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration) エンティティに、プロパティ **preSharedKey** を追加しました |
| 変更      | ベータ版    | [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) エンティティに、プロパティ **innerAuthenticationProtocolForEapTtls** および **outerIdentityPrivacyTemporaryValue** を追加しました |
| 変更      | ベータ版    | [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) エンティティから、プロパティ **nonEapAuthenticationMethodForEapTtls** および **enableOuterIdentityPrivacy** を削除しました |
| 変更      | ベータ版    | [managedAppPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) エンティティから、プロパティ **lastModifiedTime** および **deployedAppCount** を削除しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに、プロパティ **serialNumber** を追加しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティから、プロパティ **managementAgents** を削除しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティに、プロパティ **deployedAppCount** を追加しました |
| 変更      | ベータ版    | [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) エンティティに、プロパティ **bitLockerFixedDrivePolicy** および **bitLockerRemovableDrivePolicy** を追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに、プロパティ **enterpriseCloudPrintDiscoveryEndPoint**、**enterpriseCloudPrintOAuthAuthority**、**enterpriseCloudPrintOAuthClientIdentifier**、**enterpriseCloudPrintResourceIdentifier**、**enterpriseCloudPrintDiscoveryMaxLimit**、**enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**、**edgeBlockAddressBarDropdown**、**edgeBlockCompatibilityList**、**edgeClearBrowsingDataOnExit**、**edgeAllowStartPagesModification**、**edgeDisableFirstRunPage**、**edgeBlockLiveTileDataCollection** および **edgeSyncFavoritesWithInternetExplorer** を追加しました |
| 変更      | ベータ版    | [windowsManagementApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) エンティティに、プロパティ **availableVersion** を追加しました |
| 変更      | ベータ版    | [windowsManagementApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) エンティティから、プロパティ **onboardingStatus**、**deployedVersion** および **lastModifiedTime** を削除しました |
| 変更      | ベータ版    | [windowsStoreForBusinessApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) エンティティに、プロパティ **packageIdentityName** を追加しました |
| 変更      | ベータ版    | [androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を追加しました |
| 変更      | ベータ版    | [defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** を追加しました |
| 変更      | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに、ナビゲーション プロパティ **deviceConfigurationUserStateSummaries** および **iosUpdateStatuses** を追加しました |
| 変更      | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティから、ナビゲーション プロパティ **complianceSettingStateSummaries** を削除しました |
| 変更      | ベータ版    | [deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) エンティティに、ナビゲーション プロパティ **runSummary**、**deviceRunStates** および **userRunStates** を追加しました |
| 変更      | ベータ版    | [deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) エンティティから、ナビゲーション プロパティ **runStates** を削除しました |
| 変更      | ベータ版    | [iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を追加しました |
| 変更      | ベータ版    | [managedAppPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) エンティティから、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を削除しました |
| 変更      | ベータ版    | [targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティに、ナビゲーション プロパティ **mobileAppIdentifierDeployments** および **deploymentSummary** を追加しました |
| 変更      | ベータ版    | [windowsManagementApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) エンティティに、ナビゲーション プロパティ **healthSummary** および **healthStates** を追加しました |
| 変更      | ベータ版    | [appInstallationFailure](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) 複合型に、プロパティ **applicationId**、**appName**、**platformId**、**userFailures** および **deviceFailures** を追加しました |
| 変更      | ベータ版    | [bitLockerSystemDrivePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy) 複合型に、プロパティ **encryptionMethod**、**startupAuthenticationRequired**、**startupAuthenticationBlockWithoutTpmChip**、**startupAuthenticationTpmUsage**、**startupAuthenticationTpmPinUsage**、**startupAuthenticationTpmKeyUsage**、**startupAuthenticationTpmPinAndKeyUsage**、**recoveryOptions** および **prebootRecoveryEnableMessageAndUrl** を追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicySettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 複合型から、プロパティ **settingName**、**userId**、**userName**、**userEmail** および **currentValue** を削除しました |
| 変更      | ベータ版    | [deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 複合型から、プロパティ **settingName**、**userId**、**userName**、**userEmail** および **currentValue** を削除しました |
| 変更      | ベータ版    | [deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型に、プロパティ **windowsCommercialId** および **windowsCommercialIdLastModifiedTime** を追加しました |
| 変更      | ベータ版    | [vpnServer](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver) 複合型に、プロパティ **address** を追加しました |


## <a name="may-2017"></a>2017 年 5 月

### <a name="application-api-changes"></a>アプリケーション API の変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | アプリケーション API の更新。これはプロパティの名前変更と[アプリケーション](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/application) エンティティの再構築を含む最初の変更のセットです。<br/>**新しいエンティティ:** [api](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/api])、[informationalUrl](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/informationalUrl)、[installedClient](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/installedclient)[permissionScope](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/permissionscope)、[preauthorizedApplication](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/preauthorizedapplication)、[web](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/web)。<br/>**削除されたプロパティ:** addIns、appRoles、availableToOtherOrganizations、knownClientApplications、oauth2AllowUrlPathMatching、recordConsentConditions。<br/>**名前が変更されたプロパティ:** appId から id、identifierUris から applicationAliases、availableToOtherTenants から orgRestrictions、mainLogo から logo、oauth2Permissions から publishedPermissionsScopes、publicClient は allowPublicClient、replyUrls から redirectUrls。<br/>**新しいプロパティ:** タグ。 |

### <a name="remove-deprecated-planner-api"></a>使用されていない Planner API の削除
| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 削除        | ベータ版        | 次のエンティティを削除しました:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Project Rome

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | プロジェクト ローマのサポートを追加しました。これには、[デバイスのリストの取得](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_list_devices)、[デバイスへのコマンドの送信](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/send_device_command)、および[コマンドのステータスの確認](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/get_device_command_status)が含まれます。 |
| 追加        | ベータ版        | ユーザーの [activities](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/projectrome_activity) と [historyItems](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/projectrome_historyitem) のサポートが追加され、これには[アクティビティの upsert](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_put_activity) と[履歴項目の upsert](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/projectrome_put_historyitem) が含まれます。 |

### <a name="administrative-units-property-changes"></a>管理単位のプロパティの変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [scopedRoleMembership](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/scopedrolemembership) エンティティの roleMemberInfo プロパティ型を [ID](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/identity) に変更しました |
| 変更          | ベータ版        | [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/user) エンティティのナビゲーション プロパティ scopedAdministratorOf を scopedRoleMemberOf に変更しました |
| 変更          | ベータ版        | [administrativeUnit](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/administrativeunit) エンティティのナビゲーション プロパティ scopedAdministrators を scopedRoleMembers に変更しました |
| 変更          | ベータ版        | [directoryRole](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/directoryrole) エンティティのナビゲーション プロパティ scopedAdministrators を scopedMembers に変更しました |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>プレビューでのユーザーとグループの Webhook サポートの追加

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:-----------|:--------------|
| 変更        | ベータ版       | ユーザーとグループの [Webhook](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/webhooks) に対するサポートを追加しました。

### <a name="add-delta-query-to-v10"></a>デルタ クエリの v1.0 への追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | v1.0 にデルタ関数のサポートを追加します。 [デルタ クエリ](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_overview)を実行するために、次のエンティティに追加します。<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>例については、以下を参照してください。<br/>[グループへの増分の変更を取得する](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_groups)<br/>[フォルダー内のメッセージへの増分の変更を取得する](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_messages)<br/>[ユーザーへの増分の変更を取得する](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_users) |
| 変更          | ベータ版        | [users](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_delta) と [groups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/group_delta) に、オプションのクエリ フィルタリング機能 (ID 別) を追加します。 |

### <a name="added-user-resource-support-for-deleted-items"></a>削除されたアイテムをサポートするユーザー リソースの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [ユーザーの復元と完全削除](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/directory)に関するサポートを追加しました。 |

### <a name="added-onpremisesprovisioningerror"></a>OnPremisesProvisioningError の追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティ:[OnPremisesProvisioningError](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/onpremisesprovisioningerror) |
| 変更          | ベータ版        | [user](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/user)、[group](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/group)、および [orgcontact](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/orgcontact) への OnPremisesProvisioningError プロパティの追加 |

### <a name="added-deleteddatetime-property"></a>deletedDateTime プロパティの追加

|**変更の種類**|**バージョン**|**説明**|
|:-------------|:-----------|:--------------|
|変更|ベータ版|deletedDateTime プロパティを [user](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/user) エンティティに追加しました。
|変更|ベータ版|deletedDateTime プロパティを [group](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/group) エンティティに追加しました。
|変更|ベータ版|deletedDateTime プロパティを [application](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/application) エンティティに追加しました。

### <a name="added-domain-operations-to-v10"></a>V1.0 に追加されたドメイン操作

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [ドメイン](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domain)に操作を追加しました。<br/>新しいエンティティ:</br>[domain](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/domainDnsUnavailableRecord)<br/>新しいアクション:</br>[verify](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/api/domain_verify) |

### <a name="added-contracts-to-v10"></a>V1.0 追加されたコントラクト

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しいエンティティ:</br>[コントラクト](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/contract) |

### <a name="added-licensedetails-to-v10"></a>V1.0 に追加された licenseDetails

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 新しいエンティティ:</br>[licenseDetails](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/licensedetails) |
| 変更          | v1.0        | [users](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/resources/user) における新しい [licensedetails](https://graph.microsoft.io/ja-JP/docs/api-reference/v1.0/api/user_list_licensedetails) ナビゲーション プロパティ |


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
| 追加        | v1.0          | [device](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/device)、[group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/group)、[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/organization)、[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user) リソースで [openTypeExtension](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/opentypeextension) をサポートします。 |
| 追加        | v1.0 およびベータ版 | ユーザーが個人の Microsoft アカウントでサインインした場合は、event、post、group、message、contact、および user リソースでオープン拡張機能をサポートします。(これは、これらのリソースと、ユーザーが職場または学校のアカウントを使用してサインインした場合にオープン拡張機能をサポートする device、group、organization および user に追加します。) |
| 追加        | v1.0 およびベータ版 | `$expand` をサポートしました。[device](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/device)、[group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/group)、[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/organization)、[post](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/post)、[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user) のリソースでオープンな[拡張機能を利用できます](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/opentypeextension_get)。 |
| 追加        | ベータ版          | `$expand` をサポートしました。[administrativeUnit](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/administrativeunit) で[オープン拡張機能が利用できます](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/opentypeextension_get)。 |


### <a name="extensions-schema-extensions"></a>拡張機能 (スキーマ拡張機能) 

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0          | 新しいリソース [schemaExtension](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/schemaextension) と CRUD メソッドで、次のリソースの拡張定義を管理します: [contact](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact)、[device](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/device)、[event](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/event)、[group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/group)、[message](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message)、[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/organization)、[post](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/post)、[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user)。[administrativeUnit](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/administrativeunit) サポートは、以前と同様ベータ版に制限されていることに注意してください。 |
| 追加        | v1.0          | リソース [contact](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact)、[device](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/device)、[event](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/event)、[group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/group)、[message](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message)、[organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/organization)、[post](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/post)、[user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user) の、既存の POST、GET、および ATCH メソッドが、対応するリソース インスタンスにスキーマ拡張機能として保存されているカスタム データの追加、取得、および更新または削除をサポートするようになりました。 |
| 追加        | v1.0 およびベータ版 | `$filter` を使用して、拡張機能名など特定の拡張機能プロパティの値と一致する　プロパティを持つリソース インスタンスを検索できるようになりました。詳細については、この[例](https://devx.microsoft-tst.com/ja-JP/graph/docs/concepts/extensibility_schema_groups#5-get-a-group-and-its-extension-data)を参照してください。 |
| 変更          | v1.0 およびベータ版 | [スキーマ拡張機能の定義を削除](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/schemaextension_delete)しても、その定義に基づいて追加されたカスタム データへのアクセスに影響しなくなりました。 |
| 変更          | v1.0 およびベータ版 | スキーマ拡張機能の複合型を null に設定して、リソース・インスタンスからスキーマ拡張機能を削除できるようになりました。 |


### <a name="group"></a>グループ

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 追加 | v1.0 およびベータ版 | **drives** および **sites** ナビゲーション プロパティを **group** に追加しました。

### <a name="insights-apis"></a>Insights API

|**変更の種類**|**バージョン**|**説明**| 
|:-------------|:-----------|:--------------|
|追加|ベータ版|追加された[共有 API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/insights_shared)。<br />新しいリソース:<br />[sharingDetail](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/insights_sharingdetail) <br />[insightIdentity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/insights_insightidentity) <br />
|追加|ベータ版|追加された[使用 API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/insights_used)。<br />新しいリソース:<br />[usageDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/insights_usagedetails) <br />
|変更|ベータ版|次のリソースの新しい**タイプ** プロパティ:<br />[resourceVisualization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/insights_resourcevisualization) リソース。 <br />
|削除|ベータ版|次のエンティティを削除しました。<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[androidForWorkMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidforworkmobileappconfiguration)<br/>[cartToClassAssociation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_carttoclassassociation)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[eBookInstallSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_ebookinstallsummary)<br/>[eBookVppGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_ebookvppgroupassignment)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[remoteAssistancePartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windowsDeviceMalwareState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsdevicemalwarestate)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsMalwareInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsmalwareinformation)<br/>[windowsProtectionState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsprotectionstate)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[androidPermissionAction](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidpermissionaction)<br/>[bitLockerSystemDrivePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[settingSource](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingsource)<br/> |
| 追加    | ベータ版    | [managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_books_managedebook_assign) アクションを追加しました |
| 追加    | ベータ版    | [remoteAssistancePartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) に [beginOnboarding](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_beginonboarding) アクションを追加しました |
| 追加    | ベータ版    | [remoteAssistancePartner](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) に [disconnect](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_disconnect) アクションを追加しました |
| 削除    | ベータ版    | 次のエンティティを削除しました。<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| 削除    | ベータ版    | 次の複合型を削除しました。<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| 変更      | ベータ版    | [androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) エンティティに、次のプロパティを追加しました。**workProfilePasswordBlockFingerprintUnlock**、**workProfilePasswordBlockTrustAgents**、**workProfilePasswordExpirationDays**、**workProfilePasswordMinimumLength**、**workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**、**workProfilePasswordPreviousPasswordBlockCount**、**workProfilePasswordSignInFailureCountBeforeFactoryReset**、**workProfilePasswordRequiredType**、**workProfileRequirePassword**。 |
| 変更      | ベータ版    | [androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile) エンティティに、**subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [androidForWorkScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティに **kioskModeManagedApps** プロパティを追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティから **kioskModeManagedAppId** プロパティを削除しました |
| 変更      | ベータ版    | [androidPkcsCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidpkcscertificateprofile) エンティティに、**subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [androidScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [calendar](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/calendar) エンティティから **hexColor** プロパティを削除しました |
| 変更      | ベータ版    | [complianceSettingStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary) エンティティに、**setting** プロパティと **platformType** プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティから **windowsManagementAppEnabled** プロパティを削除しました |
| 変更      | ベータ版    | [deviceComplianceDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) エンティティに、**userName** プロパティ、**deviceModel** プロパティ、**platform** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) エンティティに、**userPrincipalName** プロパティと **deviceModel** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) エンティティに、**platformType**、**setting**、**userId**、**userEmail** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary) エンティティに、**inGracePeriodCount** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) エンティティに **userName** プロパティ、**deviceModel** プロパティ、**platform** プロパティを追加しました |
| 変更      | ベータ版    | [event](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/event) エンティティから **creationOptions** プロパティを削除しました |
| 変更      | ベータ版    | [eventMessage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/eventMessage) エンティティから **isDelegated** プロパティを削除しました |
| 変更      | ベータ版    | [group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/group) エンティティから、**unseenConversationsCount** プロパティと **unseenMessagesCount** プロパティを削除しました |
| 変更      | ベータ版    | [iosMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) エンティティに **settingXml** プロパティと **settings** プロパティを追加しました |
| 変更      | ベータ版    | [iosPkcsCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iospkcscertificateprofile) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [iosScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [macOSCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) エンティティに **systemIntegrityProtectionEnabled** プロパティを追加しました |
| 変更      | ベータ版    | [macOSScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに、**complianceGracePeriodExpirationDateTime**、**userPrincipalName**、**imei** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) エンティティから **settingXml** プロパティと **settings** プロパティを削除しました |
| 変更      | ベータ版    | [officeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) エンティティに、次のプロパティを追加しました。**useSharedComputerActivation**、**updateChannel**、**officePlatformArchitecture**、**localesToInstall**。 |
| 変更      | ベータ版    | [organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_organization) エンティティから **applePushNotificationCertificateSetting** プロパティを削除しました |
| 変更      | ベータ版    | [post](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/post) エンティティで次のプロパティを変更しました。<br/>**sender** を省略可能から必須に変更しました<br/> |
| 変更      | ベータ版    | [softwareUpdateStatusSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary) エンティティに、次のプロパティを追加しました。**compliantUserCount**、**nonCompliantUserCount**、**remediatedUserCount**、**errorUserCount**、**unknownUserCount**、**conflictUserCount**、**notApplicableUserCount**。 |
| 変更      | ベータ版    | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに、次のプロパティを追加しました。**bluetoothAllowedServices**、**bluetoothBlockPrePairing**、**cellularData**、**defenderDetectedMalwareActions**、**defenderPotentiallyUnwantedAppAction**、**lockScreenAllowTimeoutConfiguration**、**lockScreenBlockCortana**、**lockScreenBlockToastNotifications**、**lockScreenTimeoutInSeconds**、**passwordBlockSimple**、**privacyAutoAcceptPairingAndConsentPrompts**、**privacyBlockInputPersonalization**、**startMenuHideChangeAccountSettings**、**startMenuHideHibernate**、**startMenuHideLock**、**startMenuHideShutDown**、**startMenuHideSignOut**、**startMenuHideSleep**、**startMenuHideSwitchAccount**、**settingsBlockAppsPage**、**settingsBlockGamingPage**、**windowsSpotlightBlockConsumerSpecificFeatures**、**windowsSpotlightBlocked**、**windowsSpotlightBlockOnActionCenter**、**windowsSpotlightBlockTailoredExperiences**、**windowsSpotlightBlockThirdPartyNotifications**、**windowsSpotlightBlockWelcomeExperience**、**windowsSpotlightBlockWindowsTips**、**windowsSpotlightConfigureOnLockScreen**、**connectedDevicesServiceBlocked**。 |
| 変更      | ベータ版    | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティから次のプロパティを削除しました。**automaticUpdateMode**、**automaticUpdateSchedule**、**automaticUpdateTime**、**prereleaseFeatures**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips**、**experienceBlockConsumerSpecificFeatures**。 |
| 変更      | ベータ版    | [windows10PkcsCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pkcscertificateprofile) エンティティに **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [windows81SCEPCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) エンティティに、**indexingEncryptedStoresOrItemsBlocked** プロパティと **smbAutoEncryptedFileExtensions** プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) エンティティで次のプロパティを変更しました:<br/>**rightsManagementServicesTemplateId** を必須から省略可能に変更しました<br/> |
| 変更      | ベータ版    | [windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) エンティティで次のプロパティを変更しました:<br/>**productCode** を必須から省略可能に変更しました<br/> |
| 変更      | ベータ版    | [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) エンティティに、**subjectNameFormatString** プロパティと **subjectAlternativeNameFormatString** プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **mobileAppConfigurations** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに、**cartToClassAssociations**、**deviceCompliancePolicySettingStateSummaries**、**remoteAssistancePartners**、**windowsInformationProtectionAppLearningSummaries**、**windowsMalwareInformation** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [eBookGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment) エンティティに **eBook** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **windowsProtectionState** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook) エンティティに **installSummary** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) エンティティから **outlook** ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [windowsManagementApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp) エンティティから **healthStates** ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [defaultDeviceEnrollmentRestrictions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_defaultdeviceenrollmentrestrictions) 複合型に **androidForWorkRestrictions** プロパティを追加しました |
| 変更      | ベータ版    | [deviceCompliancePolicySettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 複合型に **userPrincipalName** プロパティと **sources** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 複合型に **userPrincipalName** プロパティと **sources** プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 複合型に、**settingName**、**userId**、**userName**、**userEmail**、**currentValue** の各プロパティを追加しました |
| 変更      | ベータ版    | [mailboxSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/mailboxSettings) 複合型から **archiveFolder** プロパティを削除しました |


### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | **findMeetingTimes**に対して、列挙型の値 **unrestricted** を追加しました。これは、**timeConstraint** パラメーターの一部である **activityDomain** プロパティとして指定します。これにより、**findMeetingTimes**はスケジュールを設定しているアクティビティの種類に適した時間を検索します。詳細については、[要求の本文](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_findmeetingtimes#request-body)セクションを参照してください。 |
| 追加        | ベータ版          | **イベント**の本文を、既定の HTML 形式の代わりにプレーン テキストで取得することをサポートします。詳細については、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/event_get) および [list](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_list_events) イベントを参照してください。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | **メッセージ**の本文を、既定の HTML 形式の代わりにプレーン テキストで取得することをサポートします。詳細については、[get](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/message_get) および [list](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_list_messages) イベントを参照してください。 |


### <a name="outlook-tasks"></a>Outlook のタスク

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Outlook タスクにアクセスするために、新しい **Outlook** ナビゲーション プロパティを [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/user) に追加しました。 |
| 追加        | ベータ版        | 新しいエンティティ ([outlookuser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlookuser)、[outlookTaskGroup](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlooktaskgroup)、[outlookTaskFolder](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlooktaskfolder)、および [outlookTask](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/outlooktask)) とそれらのメソッドが、Outlook タスクの整理とアクセスをサポートします。 |
| 追加        | ベータ版        | Outlook タスクで添付ファイルをサポートします ([attachment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/attachment)、[fileAttachment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/fileattachment)、[itemAttachment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/itemattachment)、および [referenceAttachment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/referenceattachment) リソース)。 |
| 追加        | ベータ版        | Outlook タスクで[拡張プロパティ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/extended-properties-overview)をサポートします ([singleValueLegacyExtendedProperty](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/singlevaluelegacyextendedproperty) および [multiValueLegacyExtendedProperty](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/multivaluelegacyextendedproperty) リソース)。 |

### <a name="planner-apis"></a>Planner API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | [Planner API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/planner_overview) を追加しました。<br />新しいリソース:<br />[plannerPlan](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerBuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/plannerprogresstaskboardtaskformat) |

### <a name="sharepoint-sites"></a>SharePoint サイト

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 追加      | v1.0      | サイト リソースが v1.0 エンドポイントで使用できるようになりました。<br/> **site** および **siteCollection** リソース型を追加しました。
| 変更        | ベータ版      | **site** リソースの ID の形式を変更しました。これはベータ版 API の大きな変更点です。
| 削除       | ベータ版      | **sharePoint** エンティティをベータ版 API から削除しました。この機能は、現在 **sites**コレクションから使用できます。

### <a name="sharepoint-lists"></a>SharePoint リスト

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:----------|:--------------|
| 変更 | ベータ版 | **Sharepoint** のナビゲーション プロパティを削除しました。サイトは、**sites** ナビゲーション プロパティから直接アクセスできるようになりました。 <br/> **fieldDefinition** リソースを削除しました。これは既に **columnDefinition** に置き換えられています。 <br/> **siteCollectionId** および **siteId** プロパティを **site** から削除しました。代わりに **sharepointIds** を使用します。 <br/> **listItemId** プロパティを **listItem** から削除しました。代わりに **sharepointIds** を使用します。 <br/> **listItem** の **columnSet** プロパティの名前を **fields** に変更しました。 <br/> **site** リソースを、ID の一部に SharePoint ホスト名を使用するように変更しました。
| 追加 | ベータ版 | **booleanColumn**、**calculatedColumn**、**choiceColumn**、**dateTimeColumn**、**lookupColumn**、**numberColumn**、**personOrGroupColumn**、および **textColumn** リソース型を追加しました。 <br/> **displayName** プロパティを **site** に追加しました。 <br/> **columns** ナビゲーション プロパティを **site** に追加しました。 <br/> **list** および **listItem** ナビゲーション プロパティを **sharedDriveItem** に追加しました。 <br/> **sharepointIds** プロパティを **list** と **listItem**、および **site** に追加しました。 <br/> **columnDefinition** リソース型を追加しました。




## <a name="april-2017"></a>2017 年 4 月

### <a name="administrative-units-property-changes"></a>管理単位のプロパティ変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | 管理単位の API がプレビュー (ベータ版) で更新されます。最初の一連の変更は、2017 年 5 月 3 日に適用されます。これには、次のプロパティ名の変更が含まれます。<br />scopedRoleMembership エンティティの - **roleMemberInfo** 複合型が **ID** 複合型に変更されます<br />user エンティティの - **scopedAdministratorOf** ナビゲーション プロパティが **scopedRoleMemberOf** に変更されます<br />administrativeUnit エンティティの - **scopedAdministrators** ナビゲーション プロパティが **scopedRoleMembers** に変更されます<br />directoryRole エンティティの - **scopedAdministrators** ナビゲーション プロパティが **scopedMembers** に変更されます |

### <a name="application-and-serviceprincipal-api-changes"></a>application API と servicePrincipal API の変更

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [application](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/application) API と [servicePrincipal](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/serviceprincipal) API は、プレビュー (ベータ版) で更新されます。最初の一連の変更は、2017 年 5 月 15 日に適用されます。変更には、プロパティの名前変更と再構築が含まれます。一部のプロパティ (appRoles、addIns など) は、変更が完了するまで利用できません。変更は、v1.0 へのリリース前にプレビュー (ベータ版) でリリースされます。 |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>クラウド ソリューション プロバイダー開発者向けプレビュー サポートの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | クラウド ソリューション プロバイダーの事前承認されたアプリケーションが Microsoft Graph を呼び出せるようにする、新しいプレビュー機能を追加し、新しい[承認トピック](https://graph.microsoft.io/ja-JP/docs/concepts/auth_cloudsolutionprovider)に記載しました。 |

### <a name="added-onpremises-properties-to-user-entity"></a>user エンティティへの onPremises プロパティの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [user](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/user) エンティティに、新しい onPremises プロパティである onPremisesDomainName、OnPremisesSamAccountName、onPremisesUserPrincipalName を追加しました。 |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>新しい Planner API とグループ可視性プロパティに対する更新

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | [Group](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/group) エンティティに、可視性プロパティの追加の値として **HiddenMembership** を追加しました |
| 追加        | ベータ版        | 新しい [Planner API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/planner_overview) を追加しました。<br />新しいリソース:<br />[plannerPlan](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerBuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat) |

### <a name="intune-apis"></a>Intune API
| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティを追加しました。<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy)<br/>[deviceComplianceSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate)<br/>[deviceInstallState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate)<br/>[deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment)<br/>[iosVppEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_iosvppebook)<br/>[managedEBook](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_managedebook)<br/>[userInstallStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary)<br/>[windowsManagementApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapphealthstate)<br/> |
| 追加        | ベータ版        | 新しい複合型を追加しました。<br/>[dailySchedule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark)<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter)<br/>[iosWebContentFilterBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase)<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess)<br/>[runSchedule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver)<br/> |
| 追加        | ベータ版        | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [requestRemoteAssistance](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_requestremoteassistance) アクションを追加しました |
| 追加        | ベータ版        | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [cleanWindowsDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_cleanwindowsdevice) アクションを追加しました |
| 追加        | ベータ版        | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser) アクションを追加しました |
| 追加        | ベータ版        | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_deleteuserfromsharedappledevice) アクションを追加しました |
| 追加        | ベータ版        | [deviceManagementScript](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagementscript_assign) アクションを追加しました |
| 追加        | ベータ版        | [appleVolumePurchaseProgramToken](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) に [syncLicenses](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses) アクションを追加しました |
| 追加        | ベータ版        | [mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) コレクションに **getTopMobileApps** 関数を追加しました |
| 追加        | ベータ版        | [applePushNotificationCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate) に [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest) 関数を追加しました |
| 追加        | ベータ版        | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) に [getDeviceComplianceSettingStates](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates) 関数を追加しました |
| 追加        | ベータ版        | [reportRoot](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) に [deviceConfigurationUserActivity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity) 関数を追加しました |
| 追加        | ベータ版        | [reportRoot](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) に [deviceConfigurationDeviceActivity](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity) 関数を追加しました |
| 削除        | ベータ版        | 次の複合型を削除しました。<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| 変更          | ベータ版        | [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティに **deviceSharingAllowed** プロパティを追加しました |
| 変更          | ベータ版        | [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティから **deviceSharingBlocked** プロパティを削除しました。 |
| 変更          | ベータ版        | [defaultManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) エンティティに **minimumRequiredSdkVersion** プロパティを追加しました |
| 変更          | ベータ版        | [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **windowsManagementAppEnabled** プロパティを追加しました |
| 変更          | ベータ版        | [deviceComplianceActionItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) エンティティに **notificationTemplateId** プロパティを追加しました |
| 変更          | ベータ版        | [deviceConfigurationGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment) エンティティに **excludeGroup** プロパティを追加しました |
| 変更          | ベータ版        | [iosCustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration) エンティティで次のプロパティを変更しました:<br/>**payloadFileName** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) エンティティに **contentFilterSettings** プロパティを追加しました |
| 変更          | ベータ版        | [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) エンティティに **cellularBlockPersonalHotspot** プロパティと **passcodeBlockFingerprintModification** プロパティを追加しました |
| 変更          | ベータ版        | [iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) エンティティに **minimumRequiredSdkVersion** プロパティを追加しました |
| 変更          | ベータ版        | [macOSCustomConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration) エンティティで次のプロパティを変更しました:<br/>**payloadFileName** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [managedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) エンティティに、**disableAppPinIfDevicePinIsSet**、**minimumRequiredOsVersion**、**minimumWarningOsVersion**、**minimumRequiredAppVersion**、**minimumWarningAppVersion** の各プロパティを追加しました |
| 変更          | ベータ版        | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに、**remoteAssistanceSessionUrl**、**isEncrypted**、**model**、**manufacturer** の各プロパティを追加しました |
| 変更          | ベータ版        | [getMobileAppCount](https://developer.microsoft.com/ja-JP/graph/docs/docs/api-reference/beta/api/intune_apps_mobileapp_getmobileappcount) エンティティで次のプロパティを変更しました。<br/>**bindingParameter** を **mobileApp** から *mobileApp* の **collection** に変更しました<br/>**status** を GUID から String に変更しました<br/> |
| 変更          | ベータ版        | [mobileAppGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment) エンティティに **vpnConfigurationId** プロパティを追加しました |
| 変更          | ベータ版        | [notificationMessageTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate) エンティティから **fromEmailAddress** プロパティを削除しました |
| 変更          | ベータ版        | [officeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) エンティティに **excludedApps** プロパティを追加しました |
| 変更          | ベータ版        | [officeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) エンティティから **excludedOfficeApps** プロパティを削除しました |
| 変更          | ベータ版        | [sharedPCConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration) エンティティに **enabled** プロパティを追加しました |
| 変更          | ベータ版        | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに、**networkProxyApplySettingsDeviceWide**、**networkProxyDisableAutoDetect**、**networkProxyAutomaticConfigurationUrl**、**networkProxyServer**、**bluetoothDeviceName**、**wiFiScanInterval**、**wirelessDisplayBlockProjectionToThisDevice**、**wirelessDisplayBlockUserInputFromReceiver**、**wirelessDisplayRequirePinForPairing**、**experienceBlockDeviceDiscovery**、**experienceBlockErrorDialogWhenNoSIM**、**experienceBlockTaskSwitcher**、**startMenuPinnedFolderDocuments**、**startMenuPinnedFolderDownloads**、**startMenuPinnedFolderFileExplorer**、**startMenuPinnedFolderHomeGroup**、**startMenuPinnedFolderMusic**、**startMenuPinnedFolderNetwork**、**startMenuPinnedFolderPersonalFolder**、**startMenuPinnedFolderPictures**、**startMenuPinnedFolderSettings**、**startMenuPinnedFolderVideos**、**startMenuAppListVisibility**、**startMenuHideFrequentlyUsedApps**、**startMenuHideRecentJumpLists**、**startMenuHideRecentlyAddedApps**、**startMenuHideRestartOptions**、**startMenuHideUserTile**、**startMenuHidePowerButton**、**startMenuLayoutEdgeAssetsXml**、**personalizationDesktopImageUrl**、**personalizationLockScreenImageUrl** の各プロパティを追加しました |
| 変更          | ベータ版        | [windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) エンティティで次のプロパティの型を変更しました:<br/>**productCode** を Guid から String に変更しました<br/> |
| 変更          | ベータ版        | [windowsPhone81AppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) エンティティで次のプロパティを変更しました:<br/>**phoneProductIdentifier** を必須から省略可能に変更しました<br/>**phonePublisherId** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [windowsPhone81AppXBundle](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle) エンティティで次のプロパティを変更しました:<br/>**appXPackageInformationList** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [windowsStoreForBusinessApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) エンティティに **productKey** プロパティと **licenseType** プロパティを追加しました |
| 変更          | ベータ版        | [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) エンティティに **previewBuildSetting** プロパティを追加しました |
| 変更          | ベータ版        | [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **windowsManagementApp** ナビゲーション プロパティと **managedEBooks** ナビゲーション プロパティを追加しました |
| 変更          | ベータ版        | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに **deviceManagementScripts**、**managedDeviceOverview**、**cloudPkiSubscriptions** の各ナビゲーション プロパティを追加しました |
| 変更          | ベータ版        | [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions) 複合型に **osMinimumVersion** プロパティと **osMaximumVersion** プロパティを追加しました |
| 変更          | ベータ版        | [hardwareInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_hardwareinformation) 複合型に **isSharedDevice** プロパティと **sharedDeviceCachedUsers** プロパティを追加しました |
| 変更          | ベータ版        | [omaSettingBase64](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64) 複合型で次のプロパティを変更しました:<br/>**fileName** を必須から省略可能に変更しました<br/> |
| 変更          | ベータ版        | [omaSettingStringXml](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml) 複合型で次のプロパティを変更しました:<br/>**fileName** を必須から省略可能に変更しました<br/> |

## <a name="march-2017"></a>2017 年 3 月

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[androidForWorkApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp)<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema)<br/>[androidForWorkSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings)<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration)<br/>[applePushNotificationCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary)<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary)<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate)<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary)<br/>[deviceConfigurationState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate)<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate)<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration)<br/>[managedDeviceCertificateState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary)<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary)<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary)<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector)<br/>[officeSuiteApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)<br/>[settingStateDeviceSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary)<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary)<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration)<br/>[windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile)<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy)<br/>[windowsMobileMSI](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample)<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson)<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem)<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate)<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate)<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine)<br/>[edgeSearchEngineBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase)<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom)<br/>[excludedApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_excludedapps)<br/>[iosEduCertificateSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings)<br/>[ipRange](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange)<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp)<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource)<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection)<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp)<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection)<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection)<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp)<br/> |
| 追加    | ベータ版    | [androidForWorkSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) に [requestSignupUrl](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl) アクションを追加しました |
| 追加    | ベータ版    | [androidForWorkSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) に [completeSignup](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup) アクションを追加しました |
| 追加    | ベータ版    | [androidForWorkSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) に [syncApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps) アクションを追加しました |
| 追加    | ベータ版    | [androidForWorkSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) に [unbind](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind) アクションを追加しました |
| 追加    | ベータ版    | [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) に [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) アクションを追加しました |
| 追加    | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) に [recoverPasscode](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_devices_manageddevice_recoverpasscode) アクションを追加しました |
| 追加    | ベータ版    | [organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_organization) に [removeApplePushNotificationCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate) アクションを追加しました |
| 追加    | ベータ版    | [iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) に [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments) アクションを追加しました |
| 追加    | ベータ版    | [androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) に [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments) アクションを追加しました |
| 追加    | ベータ版    | [targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) に [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments) アクションを追加しました |
| 追加    | ベータ版    | [iosManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) に [updateTargetedSecurityGroups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | [androidManagedAppProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) に [updateTargetedSecurityGroups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | [windowsInformationProtection](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) に [updateTargetedSecurityGroups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | [windowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy) に [updateTargetedSecurityGroups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy) に [updateTargetedSecurityGroups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) に [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag) アクションを追加しました |
| 追加    | ベータ版    | [mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) に [getTopMobileApps](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps) 関数を追加しました |
| 追加    | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) に [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery) 関数を追加しました |
| 削除    | ベータ版    | 次のエンティティを削除しました。<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/> |
| 削除    | ベータ版    | 次の複合型を削除しました。<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/> |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティに **webBrowserBlockPopups** プロパティを追加しました |
| 変更      | ベータ版    | [androidGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) エンティティから **webBrowserAllowPopups** プロパティを削除しました |
| 変更      | ベータ版    | [androidStoreApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp) エンティティに **appIdentifier** プロパティを追加しました |
| 変更      | ベータ版    | [appReportingOverviewStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/appReportingOverviewStatus) エンティティから **applicationCount**、**failedApplicationCount**、**appInstallFailures** の各プロパティを削除しました |
| 変更      | ベータ版    | [depEnrollmentProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) エンティティに **sharedIPadMaximumUserCount** プロパティと **enableSharedIPad** プロパティを追加しました |
| 変更      | ベータ版    | [depOnboardingSetting](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting) エンティティに **shareTokenWithSchoolDataSyncService** プロパティと **lastSyncErrorCode** プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) エンティティから、**numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceComplianceUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceComplianceUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) エンティティから、**numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) エンティティから、**numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceConfigurationUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) エンティティに、**pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime**、**configurationVersion** の各プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfigurationUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) エンティティから、**numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime**、**policyRevision** の各プロパティを削除しました |
| 変更      | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに **subscriptionState** プロパティを追加しました |
| 変更      | ベータ版    | [iosCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy) エンティティに **managedEmailProfileRequired** プロパティを追加しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) エンティティに **appsSingleAppModeList** プロパティを追加しました |
| 変更      | ベータ版    | [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) エンティティから **appsSingleAppModeBundleIds** プロパティを削除しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティに **expirationDateTime** プロパティを追加しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティから **expiration** プロパティを削除しました |
| 変更      | ベータ版    | [macOSCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) エンティティに、**passwordMinimumCharacterSetCount**、**osMinimumVersion**、**osMaximumVersion**、**deviceThreatProtectionEnabled**、**deviceThreatProtectionRequiredSecurityLevel**、**storageRequireEncryption** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedAndroidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに、**isSupervised**、**exchangeLastSuccessfulSyncDateTime**、**exchangeAccessState**、**exchangeAccessStateReason** の各プロパティを追加しました |
| 変更      | ベータ版    | [managedDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddeviceoverview) エンティティに **deviceExchangeAccessStateSummary** プロパティを追加しました |
| 変更      | ベータ版    | [managedIOSLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | [mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) エンティティから **installSummary** プロパティを削除しました |
| 変更      | ベータ版    | [mobileAppContentFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) エンティティに **uploadState** プロパティを追加しました |
| 変更      | ベータ版    | [mobileAppContentFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) エンティティで次のプロパティを変更しました:<br/>**azureStorageUriExpirationDateTime** を必須から省略可能に変更しました<br/> |
| 変更      | ベータ版    | [remoteActionAudit](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_remoteactionaudit) エンティティに、**initiatedByUserPrincipalName**、**deviceOwnerUserPrincipalName**、**deviceIMEI**、**actionState** の各プロパティを追加しました |
| 変更      | ベータ版    | [windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに、**oneDriveDisableFileSync**、**safeSearchFilter**、**edgeSearchEngine**、**settingsBlockSettingsApp**、**settingsBlockSystemPage**、**settingsBlockDevicesPage**、**settingsBlockNetworkInternetPage**、**settingsBlockPersonalizationPage**、**settingsBlockAccountsPage**、**settingsBlockTimeLanguagePage**、**settingsBlockEaseOfAccessPage**、**settingsBlockPrivacyPage**、**settingsBlockUpdateSecurityPage**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips**、**experienceBlockConsumerSpecificFeatures**、**startMenuLayoutXml**、**startMenuMode**、**logonBlockFastUserSwitching**、**startBlockUnpinningAppsFromTaskbar** の各プロパティを追加しました |
| 変更      | ベータ版    | [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) エンティティに、**allowPrinting**、**allowScreenCapture**、**allowTextSuggestion** の各プロパティを追加しました |
| 変更      | ベータ版    | [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) エンティティから、**blockPrinting**、**blockScreenCapture**、**blockTextSuggestion** の各プロパティを削除しました |
| 変更      | ベータ版    | [windowsAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsappx) エンティティに **identityName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsappx) エンティティで次のプロパティの型を変更しました:<br/>**applicableArchitectures** を [windowsArchitecture](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/windowsArchitecture) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsPhone81AppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) エンティティに **identityName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsPhone81AppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) エンティティで次のプロパティの型を変更しました:<br/>**applicableArchitectures** を [windowsArchitecture](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/windowsArchitecture) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsUniversalAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx) エンティティに、**identityName**、**identityPublisherHash**、**identityResourceIdentifier** の各プロパティを追加しました |
| 変更      | ベータ版    | [windowsUniversalAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx) エンティティで次のプロパティの型を変更しました:<br/>**applicableArchitectures** を [windowsArchitecture](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/windowsArchitecture) から String に変更しました<br/>**applicableDeviceTypes** を [windowsDeviceType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/windowsDeviceType) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) エンティティに **restartMode** プロパティを追加しました |
| 変更      | ベータ版    | [androidForWorkScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [androidScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに、**enterpriseCodeSigningCertificates**、**symantecCodeSigningCertificate**、**sideLoadingKeys**、**managedAppPolicies**、**iosManagedAppProtections**、**androidManagedAppProtections**、**defaultManagedAppProtections**、**targetedManagedAppConfigurations**、**mdmWindowsInformationProtectionPolicies**、**windowsInformationProtectionPolicies**、**managedAppRegistrations**、**managedAppStatuses** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティから、**appReportingOverview**、**enterpriseCerts**、**symantecCert** の各ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) エンティティに **deviceSettingStateSummaries** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) エンティティに **deviceSettingStateSummaries** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_shared_devicemanagement) エンティティに、**termsAndConditions**、**androidForWorkSettings**、**androidForWorkAppConfigurationSchemas**、**applePushNotificationCertificate**、**softwareUpdateStatusSummary**、**deviceCompliancePolicyDeviceStateSummary**、**complianceSettingStateSummaries**、**deviceConfigurationDeviceStateSummaries**、**mobileThreatDefenseConnectors** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [iosEducationDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration) エンティティから、**teacherRootCertificates**、**teacherIdentityCertificate**、**studentRootCertificates**、**studentIdentityCertificate** の各ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティで次のプロパティの型を変更しました:<br/>**deviceStatuses** を [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus) コレクションから [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) コレクションに変更しました<br/>**groupAssignments** を [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment) コレクションから [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment) コレクションに変更しました<br/> |
| 変更      | ベータ版    | [iosScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [macOSScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティに **deviceConfigurationStates** ナビゲーション プロパティと **deviceCompliancePolicyStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) エンティティに **deviceStatusSummary** ナビゲーション プロパティと **userStatusSummary** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [mobileApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) エンティティに **installSummary** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [organization](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_organization) エンティティから **sideLoadingKeys** ナビゲーション プロパティを削除しました |
| 変更      | ベータ版    | [windows81SCEPCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) エンティティに **managedDeviceCertificateStates** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | [appInstallationFailure](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) 複合型から、**applicationId**、**appName**、**platformId**、**userFailures**、**deviceFailures** の各プロパティを削除しました |
| 変更      | ベータ版    | [iosHomeScreenFolderPage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage) 複合型に **displayName** プロパティを追加しました |
| 変更      | ベータ版    | [iosHomeScreenPage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage) 複合型に **displayName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) 複合型に、**subjectName**、**description**、**expirationDateTime**、**certificate** の各プロパティを追加しました |
| 変更      | ベータ版    | [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) 複合型から **dataRecoveryCertificate** プロパティと **certificateFileName** プロパティを削除しました |
| 変更      | ベータ版    | [windowsPackageInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) 複合型に **displayName** プロパティを追加しました |
| 変更      | ベータ版    | [windowsPackageInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) 複合型で次のプロパティの型を変更しました:<br/>**applicableArchitecture** を [windowsArchitecture](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/windowsArchitecture) から String に変更しました<br/> |
| 変更      | ベータ版    | [windowsPackageInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) 複合型で次のプロパティを変更しました:<br/>**applicableArchitecture** を省略可能から必須に変更しました<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Microsoft Graph へのコントラクトの追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいリソース:</br>[コントラクト](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/contract) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Microsoft Graph へのドメイン操作の追加

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [ドメイン](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domain)に関数を追加しました。<br/>新しいエンティティ:</br>[domain](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/domainDnsUnavailableRecord)<br/>新しいアクション:</br>[forceDelete](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/api/domain_forcedelete)</br>[verify](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/api/domain_verify) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>スキーマ拡張機能を使用して Microsoft Graph にカスタム データを追加する

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Microsoft Graph を、[スキーマ拡張機能](https://developer.microsoft.com/ja-JP/graph/docs/concepts/extensibility_overview#schema-extensions-preview)を使用してアプリケーション データによって拡張します。これは、次のリソースでサポートされています。<br/>管理単位<br/>予定表イベント<br/>デバイス<br/>グループ<br/>メッセージ<br/>組織<br/>個人用連絡先<br/>投稿<br/>ユーザー<br/>次の例を参照してください。<br/>[スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](https://developer.microsoft.com/ja-JP/graph/docs/concepts/extensibility_schema_groups) |
| 追加        | ベータ版        | 検証済みの .com バニティ ドメインを必要とせずに、スキーマ拡張機能の定義を作成する別の方法が提供されました。詳しくは、[スキーマ拡張機能](https://developer.microsoft.com/ja-JP/graph/docs/concepts/extensibility_overview#schema-extensions-preview)を参照してください。 |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>オープン拡張機能を使用して Microsoft Graph にカスタム データを追加する

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 変更          | v1.0 およびベータ版 | 「Office 365 のデータ拡張機能」というこれまでの名称が「オープン拡張機能」に変更されました。 |
| 追加        | ベータ版          | [オープン拡張機能](https://developer.microsoft.com/ja-JP/graph/docs/concepts/extensibility_overview#open-extensions)をサポートする追加リソース: <br/>管理単位<br/>デバイス<br/>グループ<br/>組織<br/>ユーザー<br/>次の例を参照してください。<br/>[オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](https://developer.microsoft.com/ja-JP/graph/docs/concepts/extensibility_open_users) |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | [グループの復元と完全削除](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/directory)に関するサポートが追加されました。<br/>新しいエンティティ: deleteditems ナビゲーション プロパティを持つディレクトリ。 |
| 追加        | ベータ版        | 新しいエンティティ:</br>[Endpoint](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/endpoint) |
| 変更          | ベータ版        | [groups](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/group) における新たな [endpoints](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/api/group_list_endpoints) ナビゲーション プロパティ |
| 追加        | ベータ版        | 新しいエンティティ:</br>[licenseDetails](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/licensedetails) |
| 変更          | ベータ版        | [users](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/user) における新たな [licensedetails](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/api/user_list_licensedetails) ナビゲーション プロパティ |

### <a name="reports-apis"></a>レポート API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Office 365 レポートの新しいプレビュー API が導入されました。この API を使用すると、対象ビジネスにおけるユーザーの Office 365 サービスの使用法に関する使用状況レポートを取得できます。たとえば、サービスをよく利用してクォータに到達しそうなユーザーや、Office 365 ライセンスを必要としない可能性があるユーザーなどを識別できます。詳しくは、[レポート](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/report)を参照してください。 |

### <a name="directory-apis"></a>ディレクトリ API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティ:</br>[コントラクト](https://graph.microsoft.io/ja-JP/docs/api-reference/beta/resources/contract) |

## <a name="february-2017"></a>2017 年 2 月

### <a name="intune-apis"></a>Intune API

| 変更の種類 | バージョン | 説明                              |
| :---------- | :------ | :--------------------------------------- |
| 追加    | ベータ版    | 新しいエンティティを追加しました。<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/> |
| 追加    | ベータ版    | 新しい複合型を追加しました。<br/>[airPrintDestination](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/> |
| 追加    | ベータ版    | 
  [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティに [assign](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) アクションを追加しました |
| 追加    | ベータ版    | 
  [deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) エンティティに [scheduleActionsForRules](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules) アクションを追加しました |
| 追加    | ベータ版    | 
  [targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティに [updateTargetedSecurityGroups](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups) アクションを追加しました |
| 追加    | ベータ版    | 
  [resourceOperation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation) エンティティに [getScopesForUser](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user) 関数を追加しました |
| 変更      | ベータ版    | 
  [androidLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | 
  [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) エンティティに **assetTagTemplate**、**lockScreenFootnote**、**homeScreenDockIcons**、**homeScreenPages** の各プロパティを追加しました |
| 変更      | ベータ版    | 
  [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) エンティティから **deviceSharingAssetTagInformation**、**deviceSharingLockScreenFootnote**、**homeScreenLayoutDockIcons**、**homeScreenLayoutPages** の各プロパティを削除しました |
| 変更      | ベータ版    | 
  [iosGeneralDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) エンティティに **appsSingleAppModeBundleIds** プロパティを追加しました |
| 変更      | ベータ版    | 
  [iosLobApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp) エンティティから **manifest** プロパティを削除しました |
| 変更      | ベータ版    | 
  [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティに **createdDateTime**、**description**、**lastModifiedDateTime**、**displayName**、**version** の各プロパティを追加しました |
| 変更      | ベータ版    | 
  [managedAppPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) エンティティに **createdDateTime** プロパティと **lastModifiedDateTime** プロパティを追加しました |
| 変更      | ベータ版    | 
  [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) エンティティから **deviceRegistrationState** プロパティを削除しました |
| 変更      | ベータ版    | 
  [mobileAppContentFile](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) エンティティに **manifest** プロパティを追加しました |
| 変更      | ベータ版    | 
  [mobileAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) エンティティに **osDescription** プロパティと **userName** プロパティを追加しました |
| 変更      | ベータ版    | 
  [mobileAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) エンティティから **deviceType** プロパティを削除しました |
| 変更      | ベータ版    | 
  [mobileAppInstallStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) エンティティで次のプロパティの型を変更しました:<br/>**mobileAppInstallStatusValue** を Int32 から文字列に変更しました |
| 変更      | ベータ版    | 
  [targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティに **targetedSecurityGroupIds** プロパティと **targetedSecurityGroupsCount** プロパティを追加しました |
| 変更      | ベータ版    | 
  [targetedManagedAppConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) エンティティから **numberOfTargetedSecurityGroups** プロパティを削除しました |
| 変更      | ベータ版    | 
  [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_devices_user) エンティティに **id** プロパティを追加しました |
| 変更      | ベータ版    | 
  [windows10CertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) エンティティから **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue**、**certificateValidityPeriodScale** の各プロパティを削除しました |
| 変更      | ベータ版    | 
  [windows81CertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase) エンティティから **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue**、**certificateValidityPeriodScale** の各プロパティを削除しました |
| 変更      | ベータ版    | 
  [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration) エンティティから **applyToWindows10Mobile** プロパティを削除しました |
| 変更      | ベータ版    | 
  [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) エンティティに **enterpriseCerts**、**iosLobAppProvisioningConfigurations**、**symantecCert** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | 
  [deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) エンティティに **userStatusOverview** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | 
  [deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) エンティティに **userStatusOverview** ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | 
  [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) エンティティに **groupAssignments**、**deviceStatuses**、**userStatuses** の各ナビゲーション プロパティを追加しました |
| 変更      | ベータ版    | 
  [windows10VpnConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration) エンティティで次のプロパティの型を変更しました:<br/>
  **identityCertificate** を [windows10CertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) から [windowsCertificateProfileBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase) に変更しました |
| 変更      | ベータ版    | 
  [deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型に **deviceComplianceCheckinThresholdDays** プロパティと **isScheduledActionEnabled** プロパティを追加しました |
| 変更      | ベータ版    | 
  [deviceManagementSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 複合型から **windowsCommercialId** プロパティと **windowsCommercialIdLastModifiedTime** プロパティを削除しました |
| 変更      | ベータ版    | 
  [iosNotificationSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) 複合型に **bundleID**、**appName**、**publisher**、**enabled**、**showOnLockScreen** の各プロパティを追加しました |
| 変更      | ベータ版    | 
  [iosNotificationSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) 複合型から **bundleIdentifier**、**notificationsEnabled**、**showInLockScreen** の各プロパティを削除しました |



## <a name="january-2017"></a>2017 年 1 月

### <a name="outlook-calendar"></a>Outlook カレンダー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 
  [user](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user) リソースの新しいアクション [findMeetingTimes](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_findmeetingtimes)。 |
| 追加        | v1.0        | 新しい複合型 [attendeeBase](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/attendeebase)。attendee 型の型プロパティで構成されます。 |
| 追加        | v1.0        | 新しい複合型:<br/>[attendeeAvailability](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/timeslot) |
| 変更          | v1.0        | 
  [attendee](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/attendee) 複合型は、[recipient](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/recipient) から派生する attendeeBase から派生するようになりました。継承されたプロパティを含めて、以前と同じ **status**、**type**、**emailAddress** プロパティで構成されます。 |
| 追加        | ベータ版        | hexColor が、[calendar](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/calendar) リソースに追加されました。 |

### <a name="intune-apis"></a>Intune API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しいエンティティを追加しました。 <br/>[appReportingOverviewStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration) |
|追加|ベータ版|新しい複合型を追加しました。 <br/> [appInstallationFailure](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|削除|ベータ版|次の複合型を削除し、microsoft.graph.Json に置き換えました。<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|変更|ベータ版|次のエンティティで、プロパティの種類 appConfigComplianceStatus を complianceStatus に置き換えました。 <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|変更|ベータ版|リソース [managedAppStatusRaw](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw) について、プロパティ コンテンツの種類を managedAppSummary から Json に変更しました。|
|変更|ベータ版|GetUsersWithFlaggedAppRegistration 関数を [managedAppRegistration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration) コレクションから削除しました。|
|変更|ベータ版|
  [iosVppApp](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) エンティティの **vppToken** ナビゲーション プロパティは、包含されるコレクションではなくなりました。|
|変更|ベータ版|
  **deviceStatusOverview** プロパティが、[deviceConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) エンティティと [deviceCompliancePolicy](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) エンティティに追加されました。|
|変更|ベータ版|
  **appReportingOverview** プロパティが [deviceAppManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) シングルトンに追加されました。|
|変更|ベータ版|
  **deviceDisplayName** および **userPrincipalName** プロパティが、[deviceConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus)、[deviceComplianceDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus)、[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) の各エンティティに追加されました。|
|変更|ベータ版|
  **ruleName** プロパティが [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule) エンティティに追加されました。|
|変更|ベータ版|
  **devicesCount**、**userDisplayName**、**userPrincipalName** の各プロパティが、[deviceConfigurationUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus)、[deviceComplianceUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus)、[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus) の各エンティティに追加されました。|
|変更|ベータ版|
  [notificationMessageTemplates](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) コレクションが [deviceManagement](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement) シングルトンに追加されました。|
|変更|ベータ版|
  **isDefault**、**lastModifiedDateTime**、**locale**、**messageTemplate**、**subject** の各プロパティが [localizedNotificationMessage](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage) エンティティに追加されました。|
|変更|ベータ版|
  **azureActiveDirectoryDeviceId**、**deviceCategory**、**deviceRegistrationState**、**managementAgent** の各プロパティが [managedDevice](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice) エンティティに追加されました。|
|変更|ベータ版|
  **lastModifiedDateTime** プロパティが [mobileAppCategory](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory) エンティティに追加されました。|
|変更|ベータ版|
  **brandingOptions**、**defaultLocale**、**displayName**、**fromEmailAddress**、**lastModifiedDateTime**、**localizedNotificationMessages** の各プロパティが [notificationMessageTemplate](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) エンティティに追加されました。|
|変更|ベータ版|
  **appsAllowTrustedAppsSideloading**、**appsBlockWindowsStoreOriginatedApps**、**developerUnlockSetting**、**edgeBlockAccessToAboutFlags**、**edgeBlockDeveloperTools**、**edgeBlockExtensions**、**edgeBlockInPrivateBrowsing**、**edgeFirstRunUrl**、**edgeHomepageUrls**、**gameDvrBlocked**、**settingsBlockAddProvisioningPackage**、**settingsBlockChangeLanguage**、**settingsBlockChangePowerSleep**、**settingsBlockChangeRegion**、**settingsBlockChangeSystemTime**、**settingsBlockEditDeviceName**、**settingsBlockRemoveProvisioningPackage**、**sharedUserAppDataAllowed**、**smartScreenBlockPromptOverride**、**smartScreenBlockPromptOverrideForFiles**、**storageRestrictAppDataToSystemVolume**、**storageRestrictAppInstallToSystemVolume**、**webRtcBlockLocalhostIpAddress**、**windowsStoreBlockAutoUpdate**、**windowsStoreEnablePrivateStoreOnly** の各プロパティが、[windows10GeneralConfiguration](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) エンティティに追加されました。|

## <a name="december-2016"></a>2016 年 12 月

### <a name="delta-query"></a>デルタ クエリ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 
  [デルタ クエリ](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_overview)を実行するため、以下のエンティティに新しいデルタ関数が追加されました。<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>例については、以下をご覧ください。<br/>
  [グループへの増分の変更を取得する (プレビュー)](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_groups)<br/>
  [フォルダー内のメッセージへの増分の変更を取得する (プレビュー)](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_messages)<br/>
  [ユーザーへの増分の変更を取得する (プレビュー)](https://developer.microsoft.com/ja-JP/graph/docs/concepts/delta_query_users) |

### <a name="excel-apis"></a>Excel API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | workbookPivotTable リソース、pivotTables の refresh および refreshAll アクション、workbookRangeView リソース、フィルターされた範囲に対して実行して workbookRangeView をユーザーに返す visibleView アクション、visibleView からの行コレクションと範囲リソースの取得、範囲リソースからの columnsAfter、columnsBefore、resizedRange、rowsAbove、rowsBelow 関数、および新しいテーブル プロパティが追加されました。 |

### <a name="intune-apis"></a>Intune API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Microsoft Intune に、リソースとメソッド API が追加されました。これには、Azure ポータルでの Intune のパブリック プレビューをサポートする多数のリソースとメソッドのセットが含まれます。Intune サービスの詳細については、[Intune のドキュメント](https://go.microsoft.com/fwlink/?linkid=836405) をご覧ください。Intune のリソースと API の詳細については、「[Microsoft Graph での Intune の使用](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/intune_graph_overview)」をご覧ください。 |

## <a name="october-2016"></a>2016 年 10 月

### <a name="authorization-provider"></a>認証プロバイダー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 追加        | v1.0 およびベータ版 | v2.0 認証エンドポイントでは、[ビジネス シナリオでのデーモン プロセスおよび長時間実行プロセス](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-protocols-oauth-client-creds/)で使える client_credentials OAuth 許可がサポートされるようになりました。 |
| 追加        | v1.0 およびベータ版 | v2.0 認証エンドポイントでは、[管理者の同意エンドポイント](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)経由で、[管理者の同意を必要とするアクセス許可のスコープ](http://developer.microsoft.com/ja-JP/graph/docs/concepts/permissions_reference)がサポートされるようになりました。 |
| 追加        | v1.0 およびベータ版 | v2.0 認証エンドポイントでは、[管理者の同意エンドポイント](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)経由で、テナント内のすべてのユーザーに対する管理者の同意がサポートされるようになりました。 |

### <a name="invitation-apis"></a>招待 API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 招待エンティティの型に、招待するユーザー (**ゲスト**または**メンバー**) の種類を定義する invitedUserType プロパティが追加されました。 |
| 削除        | ベータ版        | 2016 年 11 月 11 日付けで、招待のエンティティ型から invitedToGroups プロパティが削除されます。このため、この API を使用して、招待したユーザーをグループに追加することができなくなります。代わりに、[メンバー追加 API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/group_post_members) を使ってユーザーをグループに追加することになります。 |

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
| 追加        | v1.0        | 
  [拡張プロパティ](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/extended-properties-overview)が、次のリソースでサポートされるようになりました: message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post。 |

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
| 追加        | v1.0        | アプリで v1.0 Outlook メール、カレンダー、連絡先の API を使用して、Exchange 2016 累積的な更新プログラム 3 (CU3) を使用したハイブリッド展開のオンプレミスのメールボックスにアクセスできます。REST API サポートの詳細については、特定の[ハイブリッド展開](https://developer.microsoft.com/ja-JP/graph/docs/overview/hybrid_rest_support)をご覧ください。**注:** v1.0 のこれらの API セットを使用している場合、特定のハイブリッド展開の要件を満たすオンプレミスのメールボックスで機能する、運用アプリを含むアプリを検出できるようになりました。この機能はプレビューでのみ使用できます。 |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | 2 つの場所のプロパティの型が identityRiskEvents エンドポイントの新しい複合型で置き換えられるスキーマ変更の一環として、次のプロパティが identityRiskEvents エンドポイントで変更/追加されました。</br>**location** は Edm.String から ComplexType signInLocation に変更されました。<br/>**previousLocation** は Edm.String から ComplexType signInLocation に変更されました。<br/>**signInLocation** は、city、state、countryOrRegion、geoCoordinates プロパティを含む新しい ComplexType です。<br/>**geoCoordinates** は latitude と longitude プロパティを含む新しい ComplexType です。 |

### <a name="invitation-manager"></a>招待マネージャー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 招待マネージャー API が、Microsoft Graph ベータ エンドポイントで利用可能になりました。招待マネージャー API を使用して、組織に外部ユーザーを追加するための招待状を作成します。招待の一環として、招待されたユーザーを Office 365 グループに追加することも選択できます。詳細については、[招待マネージャー](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/invitation)をご覧ください。 |

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
| 追加        | v1.0        | 
  **onlineMeetingUrl** プロパティが、[event](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/event) リソースに追加されました。 |
| 追加        | ベータ版        | event リソースに [forward](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/event_forward) アクションが追加されました。 |
| 追加        | ベータ版        | カレンダーの共有をサポートする次のプロパティが、[calendar](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/calendar) リソースに追加されました: **canEdit**、**canShare**、**canViewPrivateItems**、**isShared**、**isShareWithMe**、**owner**。 |

### <a name="outlook-mail"></a>Outlook メール

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | 
  [mailboxSettings](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/mailboxsettings) 複合型が追加されました。これには **automaticRepliesSetting**、**timeZone**、**language** プロパティが含まれています。 |
| 追加        | v1.0        | 
  **mailboxSettings** プロパティが [user](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user) リソースに追加されました。 |
| 追加        | ベータ版        | メッセージに含まれる[参照投稿](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/mention)の 1 つ以上のインスタンスを作成、一覧表示、取得、削除する機能のサポートが追加されました。参照投稿は、他のユーザーの注意を引きつけるためのメッセージ内のコールアウトをサポートしています。 |
| 追加        | ベータ版        | 
  [getMailTips](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/user_getmailtips) アクションのサポートが追加され、特定の受信者のすべてのメール ヒントを取得できるようになりました。次のリソースが追加されました: automaticRepliesMailTips、mailTips、mailTipsError。 |

### <a name="query-parameters"></a>クエリ パラメーター

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | 2016 年 9 月 26 日現在、$ プレフィックスなしのクエリ パラメーターがサポートされています。クエリ パラメーターの $ プレフィックスは、省略可能です。詳細については、ブログ投稿「[Microsoft Graph における $ プレフィックスのないクエリ パラメーターのサポート](http://dev.office.com/queryparametersinMicrosoftGraph)」をご覧ください。 |

### <a name="sharepoint"></a>SharePoint

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | SharePoint サイトへのアクセスと、[ID ごとの一覧表示](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/list_get) または [パス/URL](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/api/baseitem_getbyurl) ごとの一覧表示が可能になりました。 |
| 追加        | ベータ版        | 
  [listItem のインスタンスを一覧表示、作成、取得、削除](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/listitem)できるようになりました。 |

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
| 追加        | ベータ版        | いくつかのプロパティが削除され、対応するコレクションが連絡先エンドポイントに追加されたスキーマ変更の一環として、次のプロパティが連絡先エンドポイントに追加されました。_Websites Collection(ComplexType:Website)_、_Phones Collection (ComplexType:Phone)_、_PostalAddress Collection(ComplexType:PhysicalAddress)_。詳細については、ブログ投稿「[連絡先および People API で今後予定されている変更](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/)」をご覧ください。 |
| 削除        | ベータ版        | いくつかのプロパティが削除され、対応するコレクションが連絡先エンドポイントに追加されたスキーマ変更の一環として、次のプロパティが連絡先エンドポイントから削除されました。_BusinessHomePage_、_HomePhones_、_MobilePhone1_、_BusinessPhones_、_HomeAddress_、_BusinessAddress_、_OtherAddress_。詳細については、ブログ投稿「[連絡先および People API で今後予定されている変更](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/)」をご覧ください。 |

### <a name="excel-apis"></a>Excel API

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | v1.0        | Microsoft Graph の Excel REST API は一般公開されています。Office 365 の Excel ブックとの充実した高度な統合を構築できるようになりました。詳細については、ブログ投稿「[Microsoft Graph の新しい Excel REST API を使ってアプリをパワーアップする](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api)」をご覧ください。 |

### <a name="people"></a>複数のユーザー

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 変更          | ベータ版        | _WebSite_ プロパティの名前が _Websites_ に変更されました。詳細については、「[連絡先および People API で今後予定されている変更](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/)」をご覧ください。 |

### <a name="privileged-identity-management"></a>Privileged Identity Management

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | Privileged Identity Management (PIM) REST API が Microsoft Graph ベータ エンドポイントで利用可能になりました。[Privileged Identity Management](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-privileged-identity-management-configure/) では、グローバル管理者、課金管理者など、Azure AD の組織内でのロールのジャスト イン タイム アクティベーションが提供されます。発行された API を使用すると、特権ロールの割り当てを取得、更新して、ユーザーをロールにアクティブ化するアプリケーションを作成できます。詳細については、「[Microsoft Graph:ベータ版で利用可能な Azure AD Privileged Identity Management Preview API](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta)」と「[Azure AD Privileged Identity Management](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root)」を参照してください。 |

## <a name="july-2016"></a>2016 年 7 月

### <a name="administrative-units"></a>管理単位

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | 新しい管理単位のプレビュー API が導入されました。管理単位を使用すると、組織は Azure Active Directory を分割して、サブ部門に管理職務を委任できます。サブ部門は、地域、部署、コスト センターなどを表すことができます。これを Microsoft Graph API から管理できるようになりました。 |

## <a name="june-2016"></a>2016 年 6 月

### <a name="identityriskevents"></a>IdentityRiskEvents

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:-----------|:--------------|
|追加|ベータ版|新しい IdentityRiskEvents プレビュー API が導入されました。この API は、Azure Active Directory Identity Protection と連携して動作します。この API を使うと、Identity Protection によって生成されたリスク イベントに対してクエリを実行できます。詳細については、ブログ投稿「[Microsoft Graph の新しいプレビュー API の紹介:IdentityRiskEvents](http://dev.office.com/blogs/identityriskevents-api-preview)」をご覧ください。

### <a name="subscriptions"></a>サブスクリプション

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | _メール_と_連絡先_のサブスクリプションに対して、アプリ専用スコープがサポートされるようになりました。 |

## <a name="may-2016"></a>2016 年 5 月

### <a name="calendar"></a>カレンダー

|**変更の種類**|**バージョン**|**説明**|
|:--------------|:-----------|:--------------|
|重大な変更|ベータ版|findMeetingTimes API に対する変更です。詳細については、ブログ投稿「[Microsoft Graph findMeetingTimes API の更新](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update)」をご覧ください。この変更は、2016 年 5 月 19 日に有効になりました。

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
| 追加        | ベータ版        | 現在、Excel ブックのデータの読み取りと変更が可能な新しい Excel REST API を追加しているところです。データへのインサイトを提供することで、ユーザーが Excel ブックに保存されているコンテンツから価値を取得できるスマート アプリを構築できるようになりました。Excel の分析機能の活用、表とグラフの作成、および視覚に訴えるグラフ イメージの抽出などを、アプリ内からすべて実行できます。詳細については、「[Microsoft Graph での Excel の操作](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/beta/resources/excel)」をご覧ください。 |

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
| 追加        | v1.0 およびベータ版 | _internetMessageId_ プロパティが追加されました。メッセージ ID は、[RFC2822](http://www.ietf.org/rfc/rfc2822.txt) によって指定された形式です。 |
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
| 追加        | ベータ版        | サブスクリプション作成時の notificationUrl 検証。詳細については、「[Microsoft Graph の WebHooks の更新 - 2016 年 1 月](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016)」をご覧ください。 |
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
| 修正             | v1.0 およびベータ版 | directoryObjects にバインドされている呼び出しアクションが修正されました。このアクションは次のエラーで失敗していました。操作からの戻り値の型は、指定したエンティティ セットで使用できません。これは、次のアクションに適用されます: _microsoft.graph.checkMemberObjects_、_microsoft.graph.getMemberObjects_、_microsoft.graph.checkMemberGroups_、_microsoft.graph.assignLicense_、_microsoft.graph.changePassword_。 |

## <a name="december-2015"></a>2015 年 12 月

### <a name="contacts"></a>連絡先

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | mobilePhone プロパティが個人用連絡先エンティティ セットに追加されました。 |

### <a name="general"></a>全般

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正             | v1.0 およびベータ版 | 同じプロパティを複数回指定した $filter 式を使用する要求が修正されました。この要求は次の 500 エラーで失敗していました。同じキーを持つ項目が既に追加されています。 |
| 修正プログラム             | v1.0 およびベータ版 | アクション パラメーターの名前と値で大文字と小文字が区別されない問題を修正しました。 |
| 修正             | v1.0 およびベータ版 | 一部の埋め込み複合プロパティに null 値を含むペイロードの要求処理を修正しました。この要求は null 参照の例外で失敗していました。 |
| 追加        | v1.0 およびベータ版 | 複合型プロパティの並べ替えとフィルター処理のサポートが追加されました。 |
| 追加        | v1.0 およびベータ版 | 401 応答の www-authenticate ヘッダーに authorization_uri プロパティが追加されました。この URI は、トークンの取得フローを開始するために使用できます。 |
| 追加        | v1.0 およびベータ版 | ユーザーとグループ全体でエラー メッセージが改善されました。 |

### <a name="groups"></a>グループ

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正             | v1.0 およびベータ版 | 次のグループ アクションの呼び出しを修正しました: _microsoft.graph.addFavorite_、_microsoft.graph.removeFavorite_、_microsoft.graph.resetUnseenCount_。 |

### <a name="messages"></a>メッセージ

| **変更の種類** | **バージョン** | **説明**                          |
| :-------------- | :---------- | :--------------------------------------- |
| 追加        | ベータ版        | eventMessage の eventMessageRequest サブタイプと、startDateTime、endDateTime、location、type、recurrence、isOutOfDate プロパティが、eventMessage 型に追加されました。 |

### <a name="users"></a>ユーザー

| **変更の種類** | **バージョン**   | **説明**                          |
| :-------------- | :------------ | :--------------------------------------- |
| 修正             | v1.0 およびベータ版 | ユーザー プリンシパル名 (UPN) でユーザーを参照する場合に、他のユーザーで特定のユーザー プロパティを選択できてしまう問題を修正しました。 例: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| 修正             | v1.0 およびベータ版 | ユーザーにバインドされた _microsoft.graph.reminderView_ 関数の呼び出しを修正しました。この呼び出しは次のエラーで失敗していました。Microsoft.OutlookServices.Reminder 型で businessPhones という名前のプロパティは見つかりませんでした。 |
| 修正プログラム             | v1.0 およびベータ版 | 400 エラーで失敗していた、ユーザーの作成と更新 (POST/PATCH /v1.0/users) を修正しました。 |

