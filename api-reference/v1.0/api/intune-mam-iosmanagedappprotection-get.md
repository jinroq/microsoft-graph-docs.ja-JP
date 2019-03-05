---
title: iosManagedAppProtection の取得
description: iosManagedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca7c0104d7d6fea9d8f7d1bdb3b0725f70ca9a93
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253065"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="64d22-103">iosManagedAppProtection の取得</span><span class="sxs-lookup"><span data-stu-id="64d22-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="64d22-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64d22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64d22-105">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="64d22-105">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64d22-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="64d22-106">Prerequisites</span></span>
<span data-ttu-id="64d22-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64d22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64d22-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64d22-109">Permission type</span></span>|<span data-ttu-id="64d22-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64d22-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64d22-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64d22-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64d22-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d22-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64d22-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64d22-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64d22-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64d22-114">Not supported.</span></span>|
|<span data-ttu-id="64d22-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64d22-115">Application</span></span>|<span data-ttu-id="64d22-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64d22-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64d22-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64d22-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64d22-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="64d22-118">Optional query parameters</span></span>
<span data-ttu-id="64d22-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="64d22-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64d22-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64d22-120">Request headers</span></span>
|<span data-ttu-id="64d22-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64d22-121">Header</span></span>|<span data-ttu-id="64d22-122">値</span><span class="sxs-lookup"><span data-stu-id="64d22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64d22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64d22-123">Authorization</span></span>|<span data-ttu-id="64d22-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="64d22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64d22-125">承諾</span><span class="sxs-lookup"><span data-stu-id="64d22-125">Accept</span></span>|<span data-ttu-id="64d22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64d22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64d22-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="64d22-127">Request body</span></span>
<span data-ttu-id="64d22-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="64d22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64d22-129">応答</span><span class="sxs-lookup"><span data-stu-id="64d22-129">Response</span></span>
<span data-ttu-id="64d22-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="64d22-130">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64d22-131">例</span><span class="sxs-lookup"><span data-stu-id="64d22-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64d22-132">要求</span><span class="sxs-lookup"><span data-stu-id="64d22-132">Request</span></span>
<span data-ttu-id="64d22-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64d22-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="64d22-134">応答</span><span class="sxs-lookup"><span data-stu-id="64d22-134">Response</span></span>
<span data-ttu-id="64d22-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64d22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1839

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
    "isAssigned": true,
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true
  }
}
```



