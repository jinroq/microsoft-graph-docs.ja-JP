---
title: androidManagedAppProtections のリスト
description: androidManagedAppProtection オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8beb4d11f93732e5abcb594e9b8ea20fa244d45d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972656"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="97234-103">androidManagedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="97234-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="97234-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97234-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97234-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97234-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97234-106">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="97234-106">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97234-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="97234-107">Prerequisites</span></span>
<span data-ttu-id="97234-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97234-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97234-110">Permission type</span></span>|<span data-ttu-id="97234-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="97234-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97234-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97234-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97234-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97234-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="97234-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97234-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97234-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97234-115">Not supported.</span></span>|
|<span data-ttu-id="97234-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97234-116">Application</span></span>|<span data-ttu-id="97234-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97234-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97234-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97234-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="97234-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97234-119">Request headers</span></span>
|<span data-ttu-id="97234-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97234-120">Header</span></span>|<span data-ttu-id="97234-121">値</span><span class="sxs-lookup"><span data-stu-id="97234-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97234-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97234-122">Authorization</span></span>|<span data-ttu-id="97234-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="97234-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97234-124">承諾</span><span class="sxs-lookup"><span data-stu-id="97234-124">Accept</span></span>|<span data-ttu-id="97234-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97234-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97234-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="97234-126">Request body</span></span>
<span data-ttu-id="97234-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="97234-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97234-128">応答</span><span class="sxs-lookup"><span data-stu-id="97234-128">Response</span></span>
<span data-ttu-id="97234-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="97234-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97234-130">例</span><span class="sxs-lookup"><span data-stu-id="97234-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97234-131">要求</span><span class="sxs-lookup"><span data-stu-id="97234-131">Request</span></span>
<span data-ttu-id="97234-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97234-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="97234-133">応答</span><span class="sxs-lookup"><span data-stu-id="97234-133">Response</span></span>
<span data-ttu-id="97234-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="97234-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3247

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged",
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
      "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
      "requiredAndroidSafetyNetAppsVerificationType": "enabled",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe"
    }
  ]
}
```




