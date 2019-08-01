---
title: Get defaultManagedAppProtection
description: defaultManagedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81579f10f7f6d20b9925c0424e20b21729ec9ecf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020718"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="cacbc-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cacbc-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="cacbc-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cacbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cacbc-105">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cacbc-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cacbc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cacbc-106">Prerequisites</span></span>
<span data-ttu-id="cacbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cacbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cacbc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cacbc-109">Permission type</span></span>|<span data-ttu-id="cacbc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cacbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cacbc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cacbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cacbc-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cacbc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cacbc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cacbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cacbc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cacbc-114">Not supported.</span></span>|
|<span data-ttu-id="cacbc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cacbc-115">Application</span></span>|<span data-ttu-id="cacbc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cacbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cacbc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cacbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cacbc-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cacbc-118">Optional query parameters</span></span>
<span data-ttu-id="cacbc-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cacbc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cacbc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cacbc-120">Request headers</span></span>
|<span data-ttu-id="cacbc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cacbc-121">Header</span></span>|<span data-ttu-id="cacbc-122">値</span><span class="sxs-lookup"><span data-stu-id="cacbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cacbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cacbc-123">Authorization</span></span>|<span data-ttu-id="cacbc-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cacbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cacbc-125">承諾</span><span class="sxs-lookup"><span data-stu-id="cacbc-125">Accept</span></span>|<span data-ttu-id="cacbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cacbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cacbc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cacbc-127">Request body</span></span>
<span data-ttu-id="cacbc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cacbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cacbc-129">応答</span><span class="sxs-lookup"><span data-stu-id="cacbc-129">Response</span></span>
<span data-ttu-id="cacbc-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cacbc-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cacbc-131">例</span><span class="sxs-lookup"><span data-stu-id="cacbc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cacbc-132">要求</span><span class="sxs-lookup"><span data-stu-id="cacbc-132">Request</span></span>
<span data-ttu-id="cacbc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cacbc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="cacbc-134">応答</span><span class="sxs-lookup"><span data-stu-id="cacbc-134">Response</span></span>
<span data-ttu-id="cacbc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cacbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "faceIdBlocked": true
  }
}
```



