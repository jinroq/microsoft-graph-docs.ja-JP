---
title: managedDeviceOverview の更新
description: managedDeviceOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3808c35b9aae428975ed976b31634c27e7a41286
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980412"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="066bc-103">managedDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="066bc-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="066bc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="066bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="066bc-105">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="066bc-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="066bc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="066bc-106">Prerequisites</span></span>
<span data-ttu-id="066bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="066bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="066bc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="066bc-109">Permission type</span></span>|<span data-ttu-id="066bc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="066bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="066bc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="066bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="066bc-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="066bc-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="066bc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="066bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="066bc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066bc-114">Not supported.</span></span>|
|<span data-ttu-id="066bc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="066bc-115">Application</span></span>|<span data-ttu-id="066bc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="066bc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="066bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="066bc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="066bc-118">Request headers</span></span>
|<span data-ttu-id="066bc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="066bc-119">Header</span></span>|<span data-ttu-id="066bc-120">値</span><span class="sxs-lookup"><span data-stu-id="066bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="066bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="066bc-121">Authorization</span></span>|<span data-ttu-id="066bc-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="066bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="066bc-123">承諾</span><span class="sxs-lookup"><span data-stu-id="066bc-123">Accept</span></span>|<span data-ttu-id="066bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="066bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="066bc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="066bc-125">Request body</span></span>
<span data-ttu-id="066bc-126">要求本文で、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="066bc-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="066bc-127">次の表に、[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="066bc-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="066bc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="066bc-128">Property</span></span>|<span data-ttu-id="066bc-129">型</span><span class="sxs-lookup"><span data-stu-id="066bc-129">Type</span></span>|<span data-ttu-id="066bc-130">説明</span><span class="sxs-lookup"><span data-stu-id="066bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="066bc-131">id</span><span class="sxs-lookup"><span data-stu-id="066bc-131">id</span></span>|<span data-ttu-id="066bc-132">String</span><span class="sxs-lookup"><span data-stu-id="066bc-132">String</span></span>|<span data-ttu-id="066bc-133">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="066bc-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="066bc-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="066bc-134">enrolledDeviceCount</span></span>|<span data-ttu-id="066bc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="066bc-135">Int32</span></span>|<span data-ttu-id="066bc-136">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="066bc-136">Total enrolled device count.</span></span> <span data-ttu-id="066bc-137">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="066bc-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="066bc-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="066bc-138">mdmEnrolledCount</span></span>|<span data-ttu-id="066bc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="066bc-139">Int32</span></span>|<span data-ttu-id="066bc-140">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="066bc-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="066bc-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="066bc-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="066bc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="066bc-142">Int32</span></span>|<span data-ttu-id="066bc-143">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="066bc-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="066bc-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="066bc-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="066bc-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="066bc-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="066bc-146">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="066bc-146">Device operating system summary.</span></span>|
|<span data-ttu-id="066bc-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="066bc-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="066bc-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="066bc-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="066bc-149">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="066bc-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="066bc-150">応答</span><span class="sxs-lookup"><span data-stu-id="066bc-150">Response</span></span>
<span data-ttu-id="066bc-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="066bc-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="066bc-152">例</span><span class="sxs-lookup"><span data-stu-id="066bc-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="066bc-153">要求</span><span class="sxs-lookup"><span data-stu-id="066bc-153">Request</span></span>
<span data-ttu-id="066bc-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="066bc-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 685

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
  }
}
```

### <a name="response"></a><span data-ttu-id="066bc-155">応答</span><span class="sxs-lookup"><span data-stu-id="066bc-155">Response</span></span>
<span data-ttu-id="066bc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="066bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

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
  }
}
```



