---
title: windows10EndpointProtectionConfigurations のリスト
description: windows10EndpointProtectionConfiguration オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 2177dc4261f61192ab149a4adc3ffa6e98a69b48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068444"
---
# <a name="list-windows10endpointprotectionconfigurations"></a>windows10EndpointProtectionConfigurations のリスト

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのコレクションを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 29008

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
      "id": "09709403-9403-0970-0394-700903947009",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "userRightsAccessCredentialManagerAsTrustedCaller": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsAllowAccessFromNetwork": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsBlockAccessFromNetwork": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsActAsPartOfTheOperatingSystem": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsLocalLogOn": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsBackupData": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsChangeSystemTime": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsCreateGlobalObjects": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsCreatePageFile": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsCreatePermanentSharedObjects": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsCreateSymbolicLinks": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsCreateToken": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsDebugPrograms": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsRemoteDesktopServicesLogOn": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsDelegation": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsGenerateSecurityAudits": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsImpersonateClient": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsIncreaseSchedulingPriority": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsLoadUnloadDrivers": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsLockMemory": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsManageAuditingAndSecurityLogs": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsManageVolumes": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsModifyFirmwareEnvironment": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsModifyObjectLabels": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsProfileSingleProcess": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsRemoteShutdown": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsRestoreData": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsTakeOwnership": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "userRightsRegisterProcessAsService": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "blocked",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "name": "Name value",
            "description": "Description value",
            "securityIdentifier": "Security Identifier value"
          }
        ]
      },
      "xboxServicesEnableXboxGameSaveTask": true,
      "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
      "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
      "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
      "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
      "localSecurityOptionsBlockMicrosoftAccounts": true,
      "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
      "localSecurityOptionsEnableAdministratorAccount": true,
      "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
      "localSecurityOptionsEnableGuestAccount": true,
      "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
      "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
      "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
      "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
      "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
      "localSecurityOptionsMachineInactivityLimit": 10,
      "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
      "localSecurityOptionsDoNotRequireCtrlAltDel": true,
      "localSecurityOptionsHideLastSignedInUser": true,
      "localSecurityOptionsHideUsernameAtSignIn": true,
      "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
      "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
      "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
      "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
      "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
      "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
      "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
      "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
      "lanManagerWorkstationEnableInsecureGuestLogons": true,
      "localSecurityOptionsClearVirtualMemoryPageFile": true,
      "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
      "localSecurityOptionsAllowUIAccessApplicationElevation": true,
      "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
      "localSecurityOptionsOnlyElevateSignedExecutables": true,
      "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
      "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
      "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
      "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
      "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
      "localSecurityOptionsUseAdminApprovalMode": true,
      "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
      "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
      "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
      "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
      "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
      "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
      "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
      "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
      "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
      "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
      "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
      "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
      "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
      "defenderSecurityCenterDisableAppBrowserUI": true,
      "defenderSecurityCenterDisableFamilyUI": true,
      "defenderSecurityCenterDisableHealthUI": true,
      "defenderSecurityCenterDisableNetworkUI": true,
      "defenderSecurityCenterDisableVirusUI": true,
      "defenderSecurityCenterDisableAccountUI": true,
      "defenderSecurityCenterDisableHardwareUI": true,
      "defenderSecurityCenterDisableRansomwareUI": true,
      "defenderSecurityCenterDisableSecureBootUI": true,
      "defenderSecurityCenterDisableTroubleshootingUI": true,
      "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
      "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
      "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
      "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
      "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
      "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
      "firewallBlockStatefulFTP": true,
      "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
      "firewallPreSharedKeyEncodingMethod": "none",
      "firewallIPSecExemptionsAllowNeighborDiscovery": true,
      "firewallIPSecExemptionsAllowICMP": true,
      "firewallIPSecExemptionsAllowRouterDiscovery": true,
      "firewallIPSecExemptionsAllowDHCP": true,
      "firewallCertificateRevocationListCheckMethod": "none",
      "firewallMergeKeyingModuleSettings": true,
      "firewallPacketQueueingMethod": "disabled",
      "firewallProfileDomain": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeRequired": true,
        "stealthModeBlocked": true,
        "incomingTrafficRequired": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsRequired": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsRequired": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyNotMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyNotMerged": true,
        "outboundConnectionsRequired": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsRequired": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "securedPacketExemptionBlocked": true,
        "policyRulesFromGroupPolicyMerged": true,
        "policyRulesFromGroupPolicyNotMerged": true
      },
      "firewallProfilePublic": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeRequired": true,
        "stealthModeBlocked": true,
        "incomingTrafficRequired": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsRequired": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsRequired": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyNotMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyNotMerged": true,
        "outboundConnectionsRequired": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsRequired": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "securedPacketExemptionBlocked": true,
        "policyRulesFromGroupPolicyMerged": true,
        "policyRulesFromGroupPolicyNotMerged": true
      },
      "firewallProfilePrivate": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeRequired": true,
        "stealthModeBlocked": true,
        "incomingTrafficRequired": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsRequired": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsRequired": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyNotMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyNotMerged": true,
        "outboundConnectionsRequired": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsRequired": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "securedPacketExemptionBlocked": true,
        "policyRulesFromGroupPolicyMerged": true,
        "policyRulesFromGroupPolicyNotMerged": true
      },
      "defenderAttackSurfaceReductionExcludedPaths": [
        "Defender Attack Surface Reduction Excluded Paths value"
      ],
      "defenderOfficeAppsOtherProcessInjectionType": "block",
      "defenderOfficeAppsOtherProcessInjection": "enable",
      "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
      "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
      "defenderOfficeAppsLaunchChildProcessType": "block",
      "defenderOfficeAppsLaunchChildProcess": "enable",
      "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
      "defenderOfficeMacroCodeAllowWin32Imports": "enable",
      "defenderScriptObfuscatedMacroCodeType": "block",
      "defenderScriptObfuscatedMacroCode": "enable",
      "defenderScriptDownloadedPayloadExecutionType": "block",
      "defenderScriptDownloadedPayloadExecution": "enable",
      "defenderPreventCredentialStealingType": "enable",
      "defenderProcessCreationType": "block",
      "defenderProcessCreation": "enable",
      "defenderUntrustedUSBProcessType": "block",
      "defenderUntrustedUSBProcess": "enable",
      "defenderUntrustedExecutableType": "block",
      "defenderUntrustedExecutable": "enable",
      "defenderEmailContentExecutionType": "block",
      "defenderEmailContentExecution": "enable",
      "defenderAdvancedRansomewareProtectionType": "enable",
      "defenderGuardMyFoldersType": "enable",
      "defenderGuardedFoldersAllowedAppPaths": [
        "Defender Guarded Folders Allowed App Paths value"
      ],
      "defenderAdditionalGuardedFolders": [
        "Defender Additional Guarded Folders value"
      ],
      "defenderNetworkProtectionType": "enable",
      "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
      "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
      "defenderSecurityCenterBlockExploitProtectionOverride": true,
      "appLockerApplicationControl": "enforceComponentsAndStoreApps",
      "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
      "deviceGuardEnableVirtualizationBasedSecurity": true,
      "deviceGuardEnableSecureBootWithDMA": true,
      "smartScreenEnableInShell": true,
      "smartScreenBlockOverrideForFiles": true,
      "applicationGuardEnabled": true,
      "applicationGuardEnabledOptions": "enabledForEdge",
      "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
      "applicationGuardBlockNonEnterpriseContent": true,
      "applicationGuardAllowPersistence": true,
      "applicationGuardForceAuditing": true,
      "applicationGuardBlockClipboardSharing": "blockBoth",
      "applicationGuardAllowPrintToPDF": true,
      "applicationGuardAllowPrintToXPS": true,
      "applicationGuardAllowPrintToLocalPrinters": true,
      "applicationGuardAllowPrintToNetworkPrinters": true,
      "applicationGuardAllowVirtualGPU": true,
      "applicationGuardAllowFileSaveOnHost": true,
      "bitLockerDisableWarningForOtherDiskEncryption": true,
      "bitLockerEnableStorageCardEncryptionOnMobile": true,
      "bitLockerEncryptDevice": true,
      "bitLockerSystemDrivePolicy": {
        "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
        "encryptionMethod": "aesCbc256",
        "startupAuthenticationRequired": true,
        "startupAuthenticationBlockWithoutTpmChip": true,
        "startupAuthenticationTpmUsage": "required",
        "startupAuthenticationTpmPinUsage": "required",
        "startupAuthenticationTpmKeyUsage": "required",
        "startupAuthenticationTpmPinAndKeyUsage": "required",
        "minimumPinLength": 0,
        "recoveryOptions": {
          "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
          "blockDataRecoveryAgent": true,
          "recoveryPasswordUsage": "required",
          "recoveryKeyUsage": "required",
          "hideRecoveryOptions": true,
          "enableRecoveryInformationSaveToStore": true,
          "recoveryInformationToStore": "passwordOnly",
          "enableBitLockerAfterRecoveryInformationToStore": true
        },
        "prebootRecoveryEnableMessageAndUrl": true,
        "prebootRecoveryMessage": "Preboot Recovery Message value",
        "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
      },
      "bitLockerFixedDrivePolicy": {
        "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
        "encryptionMethod": "aesCbc256",
        "requireEncryptionForWriteAccess": true,
        "recoveryOptions": {
          "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
          "blockDataRecoveryAgent": true,
          "recoveryPasswordUsage": "required",
          "recoveryKeyUsage": "required",
          "hideRecoveryOptions": true,
          "enableRecoveryInformationSaveToStore": true,
          "recoveryInformationToStore": "passwordOnly",
          "enableBitLockerAfterRecoveryInformationToStore": true
        }
      },
      "bitLockerRemovableDrivePolicy": {
        "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
        "encryptionMethod": "aesCbc256",
        "requireEncryptionForWriteAccess": true,
        "blockCrossOrganizationWriteAccess": true
      }
    }
  ]
}
```




