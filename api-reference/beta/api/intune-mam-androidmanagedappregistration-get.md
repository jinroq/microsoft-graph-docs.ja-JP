---
title: Get androidManagedAppRegistration
description: androidManagedAppRegistration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9589f637d1b62d8664e42b4a6e0092b972bff48
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784284"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="e5992-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e5992-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="e5992-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5992-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5992-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5992-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5992-106">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e5992-106">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5992-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5992-107">Prerequisites</span></span>
<span data-ttu-id="e5992-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5992-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5992-110">Permission type</span></span>|<span data-ttu-id="e5992-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5992-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5992-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5992-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5992-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5992-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e5992-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5992-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5992-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5992-115">Not supported.</span></span>|
|<span data-ttu-id="e5992-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5992-116">Application</span></span>|<span data-ttu-id="e5992-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5992-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5992-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5992-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5992-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e5992-119">Optional query parameters</span></span>
<span data-ttu-id="e5992-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e5992-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5992-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5992-121">Request headers</span></span>
|<span data-ttu-id="e5992-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5992-122">Header</span></span>|<span data-ttu-id="e5992-123">値</span><span class="sxs-lookup"><span data-stu-id="e5992-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5992-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5992-124">Authorization</span></span>|<span data-ttu-id="e5992-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5992-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5992-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e5992-126">Accept</span></span>|<span data-ttu-id="e5992-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5992-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5992-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5992-128">Request body</span></span>
<span data-ttu-id="e5992-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e5992-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5992-130">応答</span><span class="sxs-lookup"><span data-stu-id="e5992-130">Response</span></span>
<span data-ttu-id="e5992-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5992-131">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5992-132">例</span><span class="sxs-lookup"><span data-stu-id="e5992-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5992-133">要求</span><span class="sxs-lookup"><span data-stu-id="e5992-133">Request</span></span>
<span data-ttu-id="e5992-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5992-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="e5992-135">応答</span><span class="sxs-lookup"><span data-stu-id="e5992-135">Response</span></span>
<span data-ttu-id="e5992-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5992-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "managedDeviceId": "Managed Device Id value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
      "packageId": "Package Id value"
    },
    "id": "0e064997-4997-0e06-9749-060e9749060e",
    "version": "Version value",
    "patchVersion": "Patch Version value"
  }
}
```





