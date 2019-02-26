---
title: Get managedDeviceOverview
description: managedDeviceOverview オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25921cddc534f60d90c8347c69f3b3df89cecbbc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143247"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="1a306-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a306-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="1a306-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a306-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a306-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a306-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a306-106">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1a306-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a306-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a306-107">Prerequisites</span></span>
<span data-ttu-id="1a306-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a306-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1a306-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a306-110">Permission type</span></span>|<span data-ttu-id="1a306-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a306-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a306-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a306-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a306-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a306-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1a306-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a306-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a306-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a306-115">Not supported.</span></span>|
|<span data-ttu-id="1a306-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a306-116">Application</span></span>|<span data-ttu-id="1a306-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a306-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a306-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a306-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a306-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1a306-119">Optional query parameters</span></span>
<span data-ttu-id="1a306-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1a306-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a306-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a306-121">Request headers</span></span>
|<span data-ttu-id="1a306-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a306-122">Header</span></span>|<span data-ttu-id="1a306-123">値</span><span class="sxs-lookup"><span data-stu-id="1a306-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a306-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a306-124">Authorization</span></span>|<span data-ttu-id="1a306-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a306-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a306-126">承諾</span><span class="sxs-lookup"><span data-stu-id="1a306-126">Accept</span></span>|<span data-ttu-id="1a306-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1a306-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a306-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a306-128">Request body</span></span>
<span data-ttu-id="1a306-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a306-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a306-130">応答</span><span class="sxs-lookup"><span data-stu-id="1a306-130">Response</span></span>
<span data-ttu-id="1a306-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a306-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a306-132">例</span><span class="sxs-lookup"><span data-stu-id="1a306-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a306-133">要求</span><span class="sxs-lookup"><span data-stu-id="1a306-133">Request</span></span>
<span data-ttu-id="1a306-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a306-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="1a306-135">応答</span><span class="sxs-lookup"><span data-stu-id="1a306-135">Response</span></span>
<span data-ttu-id="1a306-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a306-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




