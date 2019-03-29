---
title: Get androidManagedAppProtection
description: androidManagedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e447ed9585dd01dfdf76a96a47170b8abb24b495
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974826"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="18f63-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="18f63-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="18f63-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18f63-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18f63-105">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18f63-105">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18f63-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="18f63-106">Prerequisites</span></span>
<span data-ttu-id="18f63-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18f63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f63-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18f63-109">Permission type</span></span>|<span data-ttu-id="18f63-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18f63-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18f63-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18f63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18f63-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="18f63-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="18f63-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18f63-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18f63-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18f63-114">Not supported.</span></span>|
|<span data-ttu-id="18f63-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18f63-115">Application</span></span>|<span data-ttu-id="18f63-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18f63-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18f63-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18f63-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18f63-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="18f63-118">Optional query parameters</span></span>
<span data-ttu-id="18f63-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="18f63-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18f63-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18f63-120">Request headers</span></span>
|<span data-ttu-id="18f63-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18f63-121">Header</span></span>|<span data-ttu-id="18f63-122">値</span><span class="sxs-lookup"><span data-stu-id="18f63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18f63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f63-123">Authorization</span></span>|<span data-ttu-id="18f63-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="18f63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18f63-125">承諾</span><span class="sxs-lookup"><span data-stu-id="18f63-125">Accept</span></span>|<span data-ttu-id="18f63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18f63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18f63-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18f63-127">Request body</span></span>
<span data-ttu-id="18f63-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18f63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18f63-129">応答</span><span class="sxs-lookup"><span data-stu-id="18f63-129">Response</span></span>
<span data-ttu-id="18f63-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18f63-130">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f63-131">例</span><span class="sxs-lookup"><span data-stu-id="18f63-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18f63-132">要求</span><span class="sxs-lookup"><span data-stu-id="18f63-132">Request</span></span>
<span data-ttu-id="18f63-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18f63-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="18f63-134">応答</span><span class="sxs-lookup"><span data-stu-id="18f63-134">Response</span></span>
<span data-ttu-id="18f63-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18f63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1967

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
    "isAssigned": true,
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
  }
}
```



