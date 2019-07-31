---
title: WindowsManagedDevices を一覧表示する
description: WindowsManagedDevice オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88c6f305b9293ebc52af243fe82790ae3ec6ceae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985736"
---
# <a name="list-windowsmanageddevices"></a><span data-ttu-id="1dd2b-103">WindowsManagedDevices を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1dd2b-103">List windowsManagedDevices</span></span>

> <span data-ttu-id="1dd2b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dd2b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dd2b-106">[Windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-106">List properties and relationships of the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dd2b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1dd2b-107">Prerequisites</span></span>
<span data-ttu-id="1dd2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd2b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dd2b-110">Permission type</span></span>|<span data-ttu-id="1dd2b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dd2b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dd2b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dd2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dd2b-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dd2b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1dd2b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dd2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dd2b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-115">Not supported.</span></span>|
|<span data-ttu-id="1dd2b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dd2b-116">Application</span></span>|<span data-ttu-id="1dd2b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dd2b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dd2b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="1dd2b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dd2b-119">Request headers</span></span>
|<span data-ttu-id="1dd2b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dd2b-120">Header</span></span>|<span data-ttu-id="1dd2b-121">値</span><span class="sxs-lookup"><span data-stu-id="1dd2b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dd2b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dd2b-122">Authorization</span></span>|<span data-ttu-id="1dd2b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dd2b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1dd2b-124">Accept</span></span>|<span data-ttu-id="1dd2b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1dd2b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd2b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dd2b-126">Request body</span></span>
<span data-ttu-id="1dd2b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dd2b-128">応答</span><span class="sxs-lookup"><span data-stu-id="1dd2b-128">Response</span></span>
<span data-ttu-id="1dd2b-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-129">If successful, this method returns a `200 OK` response code and a collection of [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd2b-130">例</span><span class="sxs-lookup"><span data-stu-id="1dd2b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dd2b-131">要求</span><span class="sxs-lookup"><span data-stu-id="1dd2b-131">Request</span></span>
<span data-ttu-id="1dd2b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices
```

### <a name="response"></a><span data-ttu-id="1dd2b-133">応答</span><span class="sxs-lookup"><span data-stu-id="1dd2b-133">Response</span></span>
<span data-ttu-id="1dd2b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1dd2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8039

{
  "value": [
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
      }
    }
  ]
}
```





