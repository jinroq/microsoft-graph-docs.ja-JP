---
title: managedDeviceOverview の更新
description: managedDeviceOverview オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34271db88490fba3ac635892daac66bf9cf904b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424533"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="ad79e-103">managedDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="ad79e-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="ad79e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad79e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad79e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad79e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad79e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad79e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad79e-107">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ad79e-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad79e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad79e-108">Prerequisites</span></span>
<span data-ttu-id="ad79e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad79e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ad79e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad79e-111">Permission type</span></span>|<span data-ttu-id="ad79e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad79e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad79e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad79e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad79e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad79e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ad79e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad79e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad79e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad79e-116">Not supported.</span></span>|
|<span data-ttu-id="ad79e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad79e-117">Application</span></span>|<span data-ttu-id="ad79e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad79e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad79e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad79e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="ad79e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad79e-120">Request headers</span></span>
|<span data-ttu-id="ad79e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad79e-121">Header</span></span>|<span data-ttu-id="ad79e-122">値</span><span class="sxs-lookup"><span data-stu-id="ad79e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad79e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad79e-123">Authorization</span></span>|<span data-ttu-id="ad79e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ad79e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad79e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad79e-125">Accept</span></span>|<span data-ttu-id="ad79e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad79e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad79e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad79e-127">Request body</span></span>
<span data-ttu-id="ad79e-128">要求本文で、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad79e-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="ad79e-129">次の表に、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ad79e-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="ad79e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad79e-130">Property</span></span>|<span data-ttu-id="ad79e-131">型</span><span class="sxs-lookup"><span data-stu-id="ad79e-131">Type</span></span>|<span data-ttu-id="ad79e-132">説明</span><span class="sxs-lookup"><span data-stu-id="ad79e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad79e-133">id</span><span class="sxs-lookup"><span data-stu-id="ad79e-133">id</span></span>|<span data-ttu-id="ad79e-134">String</span><span class="sxs-lookup"><span data-stu-id="ad79e-134">String</span></span>|<span data-ttu-id="ad79e-135">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="ad79e-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="ad79e-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ad79e-136">enrolledDeviceCount</span></span>|<span data-ttu-id="ad79e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ad79e-137">Int32</span></span>|<span data-ttu-id="ad79e-138">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="ad79e-138">Total enrolled device count.</span></span> <span data-ttu-id="ad79e-139">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="ad79e-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="ad79e-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="ad79e-140">mdmEnrolledCount</span></span>|<span data-ttu-id="ad79e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ad79e-141">Int32</span></span>|<span data-ttu-id="ad79e-142">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ad79e-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="ad79e-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ad79e-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="ad79e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ad79e-144">Int32</span></span>|<span data-ttu-id="ad79e-145">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ad79e-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="ad79e-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ad79e-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="ad79e-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ad79e-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="ad79e-148">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="ad79e-148">Device operating system summary.</span></span>|
|<span data-ttu-id="ad79e-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ad79e-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="ad79e-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ad79e-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="ad79e-151">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="ad79e-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="ad79e-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="ad79e-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="ad79e-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="ad79e-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="ad79e-154">モデルと、アカウントで管理されているデバイスのメーカーの meatadata</span><span class="sxs-lookup"><span data-stu-id="ad79e-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="ad79e-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad79e-155">lastModifiedDateTime</span></span>|<span data-ttu-id="ad79e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad79e-156">DateTimeOffset</span></span>|<span data-ttu-id="ad79e-157">デバイスの概要の最後の更新日時</span><span class="sxs-lookup"><span data-stu-id="ad79e-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="ad79e-158">応答</span><span class="sxs-lookup"><span data-stu-id="ad79e-158">Response</span></span>
<span data-ttu-id="ad79e-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad79e-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad79e-160">例</span><span class="sxs-lookup"><span data-stu-id="ad79e-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad79e-161">要求</span><span class="sxs-lookup"><span data-stu-id="ad79e-161">Request</span></span>
<span data-ttu-id="ad79e-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad79e-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 943

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="ad79e-163">応答</span><span class="sxs-lookup"><span data-stu-id="ad79e-163">Response</span></span>
<span data-ttu-id="ad79e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad79e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1056

{
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
```




