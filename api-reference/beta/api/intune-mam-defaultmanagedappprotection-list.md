---
title: defaultManagedAppProtections のリスト
description: defaultManagedAppProtection オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cfcc6ff44cf818ea4e197e3c5393996d0785ddc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411366"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="86c4e-103">defaultManagedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="86c4e-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="86c4e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86c4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86c4e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86c4e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86c4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86c4e-107">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="86c4e-107">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86c4e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="86c4e-108">Prerequisites</span></span>
<span data-ttu-id="86c4e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86c4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86c4e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86c4e-111">Permission type</span></span>|<span data-ttu-id="86c4e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86c4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86c4e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86c4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86c4e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c4e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86c4e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86c4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86c4e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c4e-116">Not supported.</span></span>|
|<span data-ttu-id="86c4e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86c4e-117">Application</span></span>|<span data-ttu-id="86c4e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c4e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86c4e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86c4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="86c4e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86c4e-120">Request headers</span></span>
|<span data-ttu-id="86c4e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86c4e-121">Header</span></span>|<span data-ttu-id="86c4e-122">値</span><span class="sxs-lookup"><span data-stu-id="86c4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86c4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86c4e-123">Authorization</span></span>|<span data-ttu-id="86c4e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="86c4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86c4e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86c4e-125">Accept</span></span>|<span data-ttu-id="86c4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86c4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c4e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="86c4e-127">Request body</span></span>
<span data-ttu-id="86c4e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="86c4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86c4e-129">応答</span><span class="sxs-lookup"><span data-stu-id="86c4e-129">Response</span></span>
<span data-ttu-id="86c4e-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="86c4e-130">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c4e-131">例</span><span class="sxs-lookup"><span data-stu-id="86c4e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="86c4e-132">要求</span><span class="sxs-lookup"><span data-stu-id="86c4e-132">Request</span></span>
<span data-ttu-id="86c4e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86c4e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="86c4e-134">応答</span><span class="sxs-lookup"><span data-stu-id="86c4e-134">Response</span></span>
<span data-ttu-id="86c4e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86c4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3754

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
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true
    }
  ]
}
```




