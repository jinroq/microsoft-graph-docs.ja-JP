---
title: Get managedDeviceOverview
description: managedDeviceOverview オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 36ca13e182e5a7e1a8e84b2d4af15a4090e15835
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987090"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="5f675-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5f675-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="5f675-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f675-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f675-106">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5f675-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f675-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f675-107">Prerequisites</span></span>
<span data-ttu-id="5f675-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f675-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f675-110">Permission type</span></span>|<span data-ttu-id="5f675-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f675-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f675-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f675-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f675-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f675-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5f675-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f675-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f675-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f675-115">Not supported.</span></span>|
|<span data-ttu-id="5f675-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f675-116">Application</span></span>|<span data-ttu-id="5f675-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f675-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f675-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f675-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f675-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5f675-119">Optional query parameters</span></span>
<span data-ttu-id="5f675-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5f675-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f675-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f675-121">Request headers</span></span>
|<span data-ttu-id="5f675-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f675-122">Header</span></span>|<span data-ttu-id="5f675-123">値</span><span class="sxs-lookup"><span data-stu-id="5f675-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f675-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f675-124">Authorization</span></span>|<span data-ttu-id="5f675-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f675-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f675-126">承諾</span><span class="sxs-lookup"><span data-stu-id="5f675-126">Accept</span></span>|<span data-ttu-id="5f675-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5f675-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f675-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f675-128">Request body</span></span>
<span data-ttu-id="5f675-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5f675-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f675-130">応答</span><span class="sxs-lookup"><span data-stu-id="5f675-130">Response</span></span>
<span data-ttu-id="5f675-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5f675-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f675-132">例</span><span class="sxs-lookup"><span data-stu-id="5f675-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f675-133">要求</span><span class="sxs-lookup"><span data-stu-id="5f675-133">Request</span></span>
<span data-ttu-id="5f675-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f675-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="5f675-135">応答</span><span class="sxs-lookup"><span data-stu-id="5f675-135">Response</span></span>
<span data-ttu-id="5f675-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f675-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1139

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    },
    "managedDeviceModelsAndManufacturers": {
      "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
      "deviceModels": [
        "Device Models value"
      ],
      "deviceManufacturers": [
        "Device Manufacturers value"
      ]
    },
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





