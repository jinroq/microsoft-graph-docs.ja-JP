---
title: deviceEnrollmentPlatformRestrictionsConfiguration の更新
description: deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 970462a8f993e8ef01f5c1359e865b625bfec611
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402301"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="83331-103">deviceEnrollmentPlatformRestrictionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="83331-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="83331-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83331-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83331-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83331-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83331-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83331-107">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="83331-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83331-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="83331-108">Prerequisites</span></span>
<span data-ttu-id="83331-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83331-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83331-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83331-111">Permission type</span></span>|<span data-ttu-id="83331-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="83331-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83331-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83331-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83331-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83331-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="83331-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83331-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83331-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83331-116">Not supported.</span></span>|
|<span data-ttu-id="83331-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83331-117">Application</span></span>|<span data-ttu-id="83331-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83331-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83331-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83331-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83331-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83331-120">Request headers</span></span>
|<span data-ttu-id="83331-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83331-121">Header</span></span>|<span data-ttu-id="83331-122">値</span><span class="sxs-lookup"><span data-stu-id="83331-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83331-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83331-123">Authorization</span></span>|<span data-ttu-id="83331-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="83331-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83331-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83331-125">Accept</span></span>|<span data-ttu-id="83331-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83331-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83331-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="83331-127">Request body</span></span>
<span data-ttu-id="83331-128">要求本文で、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="83331-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="83331-129">次の表に、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="83331-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="83331-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83331-130">Property</span></span>|<span data-ttu-id="83331-131">型</span><span class="sxs-lookup"><span data-stu-id="83331-131">Type</span></span>|<span data-ttu-id="83331-132">説明</span><span class="sxs-lookup"><span data-stu-id="83331-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83331-133">id</span><span class="sxs-lookup"><span data-stu-id="83331-133">id</span></span>|<span data-ttu-id="83331-134">String</span><span class="sxs-lookup"><span data-stu-id="83331-134">String</span></span>|<span data-ttu-id="83331-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-136">displayName</span><span class="sxs-lookup"><span data-stu-id="83331-136">displayName</span></span>|<span data-ttu-id="83331-137">String</span><span class="sxs-lookup"><span data-stu-id="83331-137">String</span></span>|<span data-ttu-id="83331-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-139">説明</span><span class="sxs-lookup"><span data-stu-id="83331-139">description</span></span>|<span data-ttu-id="83331-140">String</span><span class="sxs-lookup"><span data-stu-id="83331-140">String</span></span>|<span data-ttu-id="83331-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-142">priority</span><span class="sxs-lookup"><span data-stu-id="83331-142">priority</span></span>|<span data-ttu-id="83331-143">Int32</span><span class="sxs-lookup"><span data-stu-id="83331-143">Int32</span></span>|<span data-ttu-id="83331-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83331-145">createdDateTime</span></span>|<span data-ttu-id="83331-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83331-146">DateTimeOffset</span></span>|<span data-ttu-id="83331-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83331-148">lastModifiedDateTime</span></span>|<span data-ttu-id="83331-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83331-149">DateTimeOffset</span></span>|<span data-ttu-id="83331-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-151">version</span><span class="sxs-lookup"><span data-stu-id="83331-151">version</span></span>|<span data-ttu-id="83331-152">Int32</span><span class="sxs-lookup"><span data-stu-id="83331-152">Int32</span></span>|<span data-ttu-id="83331-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83331-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="83331-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-154">iosRestriction</span></span>|[<span data-ttu-id="83331-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-156">Not yet documented</span></span>|
|<span data-ttu-id="83331-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-157">windowsRestriction</span></span>|[<span data-ttu-id="83331-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-159">Not yet documented</span></span>|
|<span data-ttu-id="83331-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="83331-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-162">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-162">Not yet documented</span></span>|
|<span data-ttu-id="83331-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-163">androidRestriction</span></span>|[<span data-ttu-id="83331-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-165">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-165">Not yet documented</span></span>|
|<span data-ttu-id="83331-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="83331-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-168">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-168">Not yet documented</span></span>|
|<span data-ttu-id="83331-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-169">macRestriction</span></span>|[<span data-ttu-id="83331-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-171">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-171">Not yet documented</span></span>|
|<span data-ttu-id="83331-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-172">macOSRestriction</span></span>|[<span data-ttu-id="83331-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="83331-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="83331-174">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="83331-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="83331-175">応答</span><span class="sxs-lookup"><span data-stu-id="83331-175">Response</span></span>
<span data-ttu-id="83331-176">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83331-176">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83331-177">例</span><span class="sxs-lookup"><span data-stu-id="83331-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="83331-178">要求</span><span class="sxs-lookup"><span data-stu-id="83331-178">Request</span></span>
<span data-ttu-id="83331-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83331-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="83331-180">応答</span><span class="sxs-lookup"><span data-stu-id="83331-180">Response</span></span>
<span data-ttu-id="83331-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83331-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2403

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```




