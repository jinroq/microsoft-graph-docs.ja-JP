---
title: Get iosManagedAppRegistration
description: iosManagedAppRegistration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 378de4c81aa510b2732f6609143fe010f946031e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357279"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="b3f9a-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="b3f9a-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="b3f9a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3f9a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3f9a-106">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-106">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3f9a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3f9a-107">Prerequisites</span></span>
<span data-ttu-id="b3f9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3f9a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3f9a-110">Permission type</span></span>|<span data-ttu-id="b3f9a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3f9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3f9a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3f9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3f9a-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3f9a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b3f9a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3f9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3f9a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-115">Not supported.</span></span>|
|<span data-ttu-id="b3f9a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3f9a-116">Application</span></span>|<span data-ttu-id="b3f9a-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3f9a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3f9a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3f9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3f9a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b3f9a-119">Optional query parameters</span></span>
<span data-ttu-id="b3f9a-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3f9a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3f9a-121">Request headers</span></span>
|<span data-ttu-id="b3f9a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3f9a-122">Header</span></span>|<span data-ttu-id="b3f9a-123">値</span><span class="sxs-lookup"><span data-stu-id="b3f9a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3f9a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3f9a-124">Authorization</span></span>|<span data-ttu-id="b3f9a-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3f9a-126">承諾</span><span class="sxs-lookup"><span data-stu-id="b3f9a-126">Accept</span></span>|<span data-ttu-id="b3f9a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b3f9a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3f9a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3f9a-128">Request body</span></span>
<span data-ttu-id="b3f9a-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3f9a-130">応答</span><span class="sxs-lookup"><span data-stu-id="b3f9a-130">Response</span></span>
<span data-ttu-id="b3f9a-131">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-131">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3f9a-132">例</span><span class="sxs-lookup"><span data-stu-id="b3f9a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3f9a-133">要求</span><span class="sxs-lookup"><span data-stu-id="b3f9a-133">Request</span></span>
<span data-ttu-id="b3f9a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="b3f9a-135">応答</span><span class="sxs-lookup"><span data-stu-id="b3f9a-135">Response</span></span>
<span data-ttu-id="b3f9a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3f9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```






