---
title: managedDeviceOverview の更新
description: managedDeviceOverview オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 004ebc370c0223b807c722bd40ce53021379e00d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349582"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="e4bbc-103">managedDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="e4bbc-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="e4bbc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4bbc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4bbc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4bbc-107">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4bbc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e4bbc-108">Prerequisites</span></span>
<span data-ttu-id="e4bbc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bbc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4bbc-111">Permission type</span></span>|<span data-ttu-id="e4bbc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4bbc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4bbc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4bbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4bbc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bbc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4bbc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4bbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4bbc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-116">Not supported.</span></span>|
|<span data-ttu-id="e4bbc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4bbc-117">Application</span></span>|<span data-ttu-id="e4bbc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4bbc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4bbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="e4bbc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4bbc-120">Request headers</span></span>
|<span data-ttu-id="e4bbc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4bbc-121">Header</span></span>|<span data-ttu-id="e4bbc-122">値</span><span class="sxs-lookup"><span data-stu-id="e4bbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4bbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4bbc-123">Authorization</span></span>|<span data-ttu-id="e4bbc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4bbc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4bbc-125">Accept</span></span>|<span data-ttu-id="e4bbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4bbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4bbc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e4bbc-127">Request body</span></span>
<span data-ttu-id="e4bbc-128">要求本文で、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="e4bbc-129">次の表に、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="e4bbc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4bbc-130">Property</span></span>|<span data-ttu-id="e4bbc-131">種類</span><span class="sxs-lookup"><span data-stu-id="e4bbc-131">Type</span></span>|<span data-ttu-id="e4bbc-132">説明</span><span class="sxs-lookup"><span data-stu-id="e4bbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4bbc-133">ID</span><span class="sxs-lookup"><span data-stu-id="e4bbc-133">id</span></span>|<span data-ttu-id="e4bbc-134">String</span><span class="sxs-lookup"><span data-stu-id="e4bbc-134">String</span></span>|<span data-ttu-id="e4bbc-135">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="e4bbc-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="e4bbc-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e4bbc-136">enrolledDeviceCount</span></span>|<span data-ttu-id="e4bbc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bbc-137">Int32</span></span>|<span data-ttu-id="e4bbc-138">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-138">Total enrolled device count.</span></span> <span data-ttu-id="e4bbc-139">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="e4bbc-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="e4bbc-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="e4bbc-140">mdmEnrolledCount</span></span>|<span data-ttu-id="e4bbc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bbc-141">Int32</span></span>|<span data-ttu-id="e4bbc-142">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e4bbc-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="e4bbc-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e4bbc-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="e4bbc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bbc-144">Int32</span></span>|<span data-ttu-id="e4bbc-145">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e4bbc-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="e4bbc-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="e4bbc-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="e4bbc-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="e4bbc-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="e4bbc-148">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-148">Device operating system summary.</span></span>|
|<span data-ttu-id="e4bbc-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="e4bbc-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="e4bbc-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="e4bbc-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="e4bbc-151">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="e4bbc-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="e4bbc-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="e4bbc-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="e4bbc-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="e4bbc-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="e4bbc-154">モデルと、アカウントで管理されているデバイスのメーカーの meatadata</span><span class="sxs-lookup"><span data-stu-id="e4bbc-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="e4bbc-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4bbc-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e4bbc-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4bbc-156">DateTimeOffset</span></span>|<span data-ttu-id="e4bbc-157">デバイスの概要の最後の更新日時</span><span class="sxs-lookup"><span data-stu-id="e4bbc-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="e4bbc-158">応答</span><span class="sxs-lookup"><span data-stu-id="e4bbc-158">Response</span></span>
<span data-ttu-id="e4bbc-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4bbc-160">例</span><span class="sxs-lookup"><span data-stu-id="e4bbc-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4bbc-161">要求</span><span class="sxs-lookup"><span data-stu-id="e4bbc-161">Request</span></span>
<span data-ttu-id="e4bbc-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 947

{
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

### <a name="response"></a><span data-ttu-id="e4bbc-163">応答</span><span class="sxs-lookup"><span data-stu-id="e4bbc-163">Response</span></span>
<span data-ttu-id="e4bbc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e4bbc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





