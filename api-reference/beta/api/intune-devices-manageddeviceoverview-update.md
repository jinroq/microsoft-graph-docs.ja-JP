---
title: managedDeviceOverview の更新
description: managedDeviceOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e66b5f5eaaf35a593176ce32a41e2ab28dab9f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522658"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="3befe-103">managedDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="3befe-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="3befe-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3befe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3befe-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3befe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3befe-106">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3befe-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3befe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3befe-107">Prerequisites</span></span>
<span data-ttu-id="3befe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3befe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3befe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3befe-110">Permission type</span></span>|<span data-ttu-id="3befe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3befe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3befe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3befe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3befe-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3befe-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3befe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3befe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3befe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3befe-115">Not supported.</span></span>|
|<span data-ttu-id="3befe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3befe-116">Application</span></span>|<span data-ttu-id="3befe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3befe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3befe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3befe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="3befe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3befe-119">Request headers</span></span>
|<span data-ttu-id="3befe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3befe-120">Header</span></span>|<span data-ttu-id="3befe-121">値</span><span class="sxs-lookup"><span data-stu-id="3befe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3befe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3befe-122">Authorization</span></span>|<span data-ttu-id="3befe-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3befe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3befe-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3befe-124">Accept</span></span>|<span data-ttu-id="3befe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3befe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3befe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3befe-126">Request body</span></span>
<span data-ttu-id="3befe-127">要求本文で、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3befe-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="3befe-128">次の表に、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3befe-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="3befe-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3befe-129">Property</span></span>|<span data-ttu-id="3befe-130">型</span><span class="sxs-lookup"><span data-stu-id="3befe-130">Type</span></span>|<span data-ttu-id="3befe-131">説明</span><span class="sxs-lookup"><span data-stu-id="3befe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3befe-132">id</span><span class="sxs-lookup"><span data-stu-id="3befe-132">id</span></span>|<span data-ttu-id="3befe-133">String</span><span class="sxs-lookup"><span data-stu-id="3befe-133">String</span></span>|<span data-ttu-id="3befe-134">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="3befe-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="3befe-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3befe-135">enrolledDeviceCount</span></span>|<span data-ttu-id="3befe-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3befe-136">Int32</span></span>|<span data-ttu-id="3befe-137">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="3befe-137">Total enrolled device count.</span></span> <span data-ttu-id="3befe-138">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="3befe-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="3befe-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="3befe-139">mdmEnrolledCount</span></span>|<span data-ttu-id="3befe-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3befe-140">Int32</span></span>|<span data-ttu-id="3befe-141">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3befe-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="3befe-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3befe-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="3befe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3befe-143">Int32</span></span>|<span data-ttu-id="3befe-144">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3befe-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="3befe-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3befe-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="3befe-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3befe-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="3befe-147">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="3befe-147">Device operating system summary.</span></span>|
|<span data-ttu-id="3befe-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3befe-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="3befe-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3befe-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="3befe-150">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="3befe-150">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="3befe-151">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="3befe-151">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="3befe-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="3befe-152">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="3befe-153">アカウントの管理対象デバイスのモデルと製造 meatadata</span><span class="sxs-lookup"><span data-stu-id="3befe-153">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="3befe-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3befe-154">lastModifiedDateTime</span></span>|<span data-ttu-id="3befe-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3befe-155">DateTimeOffset</span></span>|<span data-ttu-id="3befe-156">デバイスの最終変更日時の概要</span><span class="sxs-lookup"><span data-stu-id="3befe-156">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="3befe-157">応答</span><span class="sxs-lookup"><span data-stu-id="3befe-157">Response</span></span>
<span data-ttu-id="3befe-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3befe-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3befe-159">例</span><span class="sxs-lookup"><span data-stu-id="3befe-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="3befe-160">要求</span><span class="sxs-lookup"><span data-stu-id="3befe-160">Request</span></span>
<span data-ttu-id="3befe-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3befe-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3befe-162">応答</span><span class="sxs-lookup"><span data-stu-id="3befe-162">Response</span></span>
<span data-ttu-id="3befe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3befe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





