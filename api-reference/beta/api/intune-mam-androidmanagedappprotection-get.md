---
title: Get androidManagedAppProtection
description: androidManagedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 877b7da27203c4fe625d0a5a4a187d62f96d5471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340503"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="16059-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="16059-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="16059-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16059-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16059-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16059-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16059-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16059-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16059-107">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="16059-107">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16059-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16059-108">Prerequisites</span></span>
<span data-ttu-id="16059-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16059-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16059-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16059-111">Permission type</span></span>|<span data-ttu-id="16059-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16059-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16059-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16059-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16059-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16059-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="16059-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16059-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16059-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16059-116">Not supported.</span></span>|
|<span data-ttu-id="16059-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16059-117">Application</span></span>|<span data-ttu-id="16059-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16059-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16059-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16059-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16059-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="16059-120">Optional query parameters</span></span>
<span data-ttu-id="16059-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="16059-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="16059-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16059-122">Request headers</span></span>
|<span data-ttu-id="16059-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16059-123">Header</span></span>|<span data-ttu-id="16059-124">値</span><span class="sxs-lookup"><span data-stu-id="16059-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16059-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16059-125">Authorization</span></span>|<span data-ttu-id="16059-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16059-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16059-127">Accept</span><span class="sxs-lookup"><span data-stu-id="16059-127">Accept</span></span>|<span data-ttu-id="16059-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16059-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16059-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="16059-129">Request body</span></span>
<span data-ttu-id="16059-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16059-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16059-131">応答</span><span class="sxs-lookup"><span data-stu-id="16059-131">Response</span></span>
<span data-ttu-id="16059-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16059-132">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16059-133">例</span><span class="sxs-lookup"><span data-stu-id="16059-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="16059-134">要求</span><span class="sxs-lookup"><span data-stu-id="16059-134">Request</span></span>
<span data-ttu-id="16059-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16059-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="16059-136">応答</span><span class="sxs-lookup"><span data-stu-id="16059-136">Response</span></span>
<span data-ttu-id="16059-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16059-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2705

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
  }
}
```




