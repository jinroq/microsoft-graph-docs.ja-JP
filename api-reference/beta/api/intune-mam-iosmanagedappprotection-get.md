---
title: iosManagedAppProtection の取得
description: iosManagedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: b913d26ae7022cff368984b65fbbf6eaa85aaad2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310207"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="ad170-103">iosManagedAppProtection の取得</span><span class="sxs-lookup"><span data-stu-id="ad170-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="ad170-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad170-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad170-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad170-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad170-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad170-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad170-107">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ad170-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad170-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad170-108">Prerequisites</span></span>
<span data-ttu-id="ad170-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad170-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad170-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad170-111">Permission type</span></span>|<span data-ttu-id="ad170-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad170-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad170-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad170-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad170-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad170-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ad170-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad170-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad170-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad170-116">Not supported.</span></span>|
|<span data-ttu-id="ad170-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad170-117">Application</span></span>|<span data-ttu-id="ad170-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad170-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad170-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad170-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad170-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad170-120">Optional query parameters</span></span>
<span data-ttu-id="ad170-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ad170-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad170-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad170-122">Request headers</span></span>
|<span data-ttu-id="ad170-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad170-123">Header</span></span>|<span data-ttu-id="ad170-124">値</span><span class="sxs-lookup"><span data-stu-id="ad170-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad170-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad170-125">Authorization</span></span>|<span data-ttu-id="ad170-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ad170-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad170-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ad170-127">Accept</span></span>|<span data-ttu-id="ad170-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad170-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad170-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad170-129">Request body</span></span>
<span data-ttu-id="ad170-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad170-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad170-131">応答</span><span class="sxs-lookup"><span data-stu-id="ad170-131">Response</span></span>
<span data-ttu-id="ad170-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad170-132">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad170-133">例</span><span class="sxs-lookup"><span data-stu-id="ad170-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad170-134">要求</span><span class="sxs-lookup"><span data-stu-id="ad170-134">Request</span></span>
<span data-ttu-id="ad170-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad170-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="ad170-136">応答</span><span class="sxs-lookup"><span data-stu-id="ad170-136">Response</span></span>
<span data-ttu-id="ad170-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad170-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2736

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true,
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
    "allowedIosDeviceModels": "Allowed Ios Device Models value",
    "appActionIfIosDeviceModelNotAllowed": "wipe",
    "thirdPartyKeyboardsBlocked": true,
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true
  }
}
```





