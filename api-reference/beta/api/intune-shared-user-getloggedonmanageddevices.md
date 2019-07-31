---
title: getLoggedOnManagedDevices 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db9db9ebdd30d80761d8bdfdd6064109bf6d9339
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979667"
---
# <a name="getloggedonmanageddevices-function"></a><span data-ttu-id="29e98-103">getLoggedOnManagedDevices 関数</span><span class="sxs-lookup"><span data-stu-id="29e98-103">getLoggedOnManagedDevices function</span></span>

> <span data-ttu-id="29e98-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="29e98-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29e98-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29e98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29e98-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29e98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29e98-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29e98-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29e98-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="29e98-108">Prerequisites</span></span>

<span data-ttu-id="29e98-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29e98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29e98-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29e98-111">Permission type</span></span>|<span data-ttu-id="29e98-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29e98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29e98-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29e98-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="29e98-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="29e98-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="29e98-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29e98-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="29e98-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29e98-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29e98-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29e98-117">Not supported.</span></span>|
|<span data-ttu-id="29e98-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29e98-118">Application</span></span>|<span data-ttu-id="29e98-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29e98-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29e98-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29e98-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getLoggedOnManagedDevices
```

## <a name="request-headers"></a><span data-ttu-id="29e98-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29e98-121">Request headers</span></span>

|<span data-ttu-id="29e98-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29e98-122">Header</span></span>|<span data-ttu-id="29e98-123">値</span><span class="sxs-lookup"><span data-stu-id="29e98-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29e98-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="29e98-124">Authorization</span></span>|<span data-ttu-id="29e98-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="29e98-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29e98-126">承諾</span><span class="sxs-lookup"><span data-stu-id="29e98-126">Accept</span></span>|<span data-ttu-id="29e98-127">application/json</span><span class="sxs-lookup"><span data-stu-id="29e98-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29e98-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="29e98-128">Request body</span></span>

<span data-ttu-id="29e98-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29e98-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29e98-130">応答</span><span class="sxs-lookup"><span data-stu-id="29e98-130">Response</span></span>

<span data-ttu-id="29e98-131">成功した場合、この関数`200 OK`は応答コードと、応答本文で[manageddevice](../resources/intune-devices-manageddevice.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="29e98-131">If successful, this function returns a `200 OK` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29e98-132">例</span><span class="sxs-lookup"><span data-stu-id="29e98-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="29e98-133">要求</span><span class="sxs-lookup"><span data-stu-id="29e98-133">Request</span></span>

<span data-ttu-id="29e98-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29e98-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getLoggedOnManagedDevices
```

### <a name="response"></a><span data-ttu-id="29e98-135">応答</span><span class="sxs-lookup"><span data-stu-id="29e98-135">Response</span></span>

<span data-ttu-id="29e98-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29e98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70",
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
      "remoteAssistanceSessionErrorString": "Remote Assistance Session Error String value",
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
      "isAutopilotEnrolled": true,
      "requestUserEnrollmentApproval": true,
      "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00"
    }
  ]
}
```



