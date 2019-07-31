---
title: defaultManagedAppProtections のリスト
description: defaultManagedAppProtection オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1926ee6c006096c674bcd0c2ecea02a100782735
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994895"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="d3e9e-103">defaultManagedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="d3e9e-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="d3e9e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3e9e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3e9e-106">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-106">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3e9e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d3e9e-107">Prerequisites</span></span>
<span data-ttu-id="d3e9e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e9e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3e9e-110">Permission type</span></span>|<span data-ttu-id="d3e9e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3e9e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3e9e-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3e9e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3e9e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3e9e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-115">Not supported.</span></span>|
|<span data-ttu-id="d3e9e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3e9e-116">Application</span></span>|<span data-ttu-id="d3e9e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3e9e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3e9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="d3e9e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3e9e-119">Request headers</span></span>
|<span data-ttu-id="d3e9e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3e9e-120">Header</span></span>|<span data-ttu-id="d3e9e-121">値</span><span class="sxs-lookup"><span data-stu-id="d3e9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3e9e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3e9e-122">Authorization</span></span>|<span data-ttu-id="d3e9e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3e9e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d3e9e-124">Accept</span></span>|<span data-ttu-id="d3e9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3e9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3e9e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3e9e-126">Request body</span></span>
<span data-ttu-id="d3e9e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3e9e-128">応答</span><span class="sxs-lookup"><span data-stu-id="d3e9e-128">Response</span></span>
<span data-ttu-id="d3e9e-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-129">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e9e-130">例</span><span class="sxs-lookup"><span data-stu-id="d3e9e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3e9e-131">要求</span><span class="sxs-lookup"><span data-stu-id="d3e9e-131">Request</span></span>
<span data-ttu-id="d3e9e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="d3e9e-133">応答</span><span class="sxs-lookup"><span data-stu-id="d3e9e-133">Response</span></span>
<span data-ttu-id="d3e9e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e9e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4315

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "77064c51-4c51-7706-514c-0677514c0677",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
      "allowedOutboundClipboardSharingExceptionLength": 14,
      "notificationRestriction": "blockOrganizationalData",
      "appDataEncryptionType": "afterDeviceRestart",
      "screenCaptureBlocked": true,
      "encryptAppData": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "faceIdBlocked": true,
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "wipe",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true,
      "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
      "requiredAndroidSafetyNetAppsVerificationType": "enabled",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
      "customBrowserProtocol": "Custom Browser Protocol value",
      "customBrowserPackageId": "Custom Browser Package Id value",
      "customBrowserDisplayName": "Custom Browser Display Name value"
    }
  ]
}
```





