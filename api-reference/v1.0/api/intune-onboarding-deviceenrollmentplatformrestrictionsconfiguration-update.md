---
title: deviceEnrollmentPlatformRestrictionsConfiguration の更新
description: deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a0fe37e0391c55a8b53a38d923543cb7b12f390
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974718"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="29260-103">deviceEnrollmentPlatformRestrictionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="29260-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="29260-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29260-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29260-105">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29260-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29260-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="29260-106">Prerequisites</span></span>
<span data-ttu-id="29260-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29260-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29260-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29260-109">Permission type</span></span>|<span data-ttu-id="29260-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29260-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29260-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29260-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29260-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29260-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29260-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29260-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29260-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29260-114">Not supported.</span></span>|
|<span data-ttu-id="29260-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29260-115">Application</span></span>|<span data-ttu-id="29260-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29260-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29260-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29260-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29260-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29260-118">Request headers</span></span>
|<span data-ttu-id="29260-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29260-119">Header</span></span>|<span data-ttu-id="29260-120">値</span><span class="sxs-lookup"><span data-stu-id="29260-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29260-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="29260-121">Authorization</span></span>|<span data-ttu-id="29260-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="29260-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29260-123">承諾</span><span class="sxs-lookup"><span data-stu-id="29260-123">Accept</span></span>|<span data-ttu-id="29260-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29260-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29260-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="29260-125">Request body</span></span>
<span data-ttu-id="29260-126">要求本文で、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="29260-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="29260-127">次の表に、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="29260-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="29260-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29260-128">Property</span></span>|<span data-ttu-id="29260-129">型</span><span class="sxs-lookup"><span data-stu-id="29260-129">Type</span></span>|<span data-ttu-id="29260-130">説明</span><span class="sxs-lookup"><span data-stu-id="29260-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29260-131">id</span><span class="sxs-lookup"><span data-stu-id="29260-131">id</span></span>|<span data-ttu-id="29260-132">文字列</span><span class="sxs-lookup"><span data-stu-id="29260-132">String</span></span>|<span data-ttu-id="29260-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-134">displayName</span><span class="sxs-lookup"><span data-stu-id="29260-134">displayName</span></span>|<span data-ttu-id="29260-135">String</span><span class="sxs-lookup"><span data-stu-id="29260-135">String</span></span>|<span data-ttu-id="29260-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-137">description</span><span class="sxs-lookup"><span data-stu-id="29260-137">description</span></span>|<span data-ttu-id="29260-138">String</span><span class="sxs-lookup"><span data-stu-id="29260-138">String</span></span>|<span data-ttu-id="29260-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-140">priority</span><span class="sxs-lookup"><span data-stu-id="29260-140">priority</span></span>|<span data-ttu-id="29260-141">Int32</span><span class="sxs-lookup"><span data-stu-id="29260-141">Int32</span></span>|<span data-ttu-id="29260-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29260-143">createdDateTime</span></span>|<span data-ttu-id="29260-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29260-144">DateTimeOffset</span></span>|<span data-ttu-id="29260-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29260-146">lastModifiedDateTime</span></span>|<span data-ttu-id="29260-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29260-147">DateTimeOffset</span></span>|<span data-ttu-id="29260-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-149">version</span><span class="sxs-lookup"><span data-stu-id="29260-149">version</span></span>|<span data-ttu-id="29260-150">Int32</span><span class="sxs-lookup"><span data-stu-id="29260-150">Int32</span></span>|<span data-ttu-id="29260-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29260-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29260-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-152">iosRestriction</span></span>|[<span data-ttu-id="29260-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="29260-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29260-154">Not yet documented</span></span>|
|<span data-ttu-id="29260-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-155">windowsRestriction</span></span>|[<span data-ttu-id="29260-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="29260-157">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29260-157">Not yet documented</span></span>|
|<span data-ttu-id="29260-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="29260-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="29260-160">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29260-160">Not yet documented</span></span>|
|<span data-ttu-id="29260-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-161">androidRestriction</span></span>|[<span data-ttu-id="29260-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="29260-163">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29260-163">Not yet documented</span></span>|
|<span data-ttu-id="29260-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-164">macOSRestriction</span></span>|[<span data-ttu-id="29260-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="29260-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="29260-166">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29260-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29260-167">応答</span><span class="sxs-lookup"><span data-stu-id="29260-167">Response</span></span>
<span data-ttu-id="29260-168">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29260-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29260-169">例</span><span class="sxs-lookup"><span data-stu-id="29260-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="29260-170">要求</span><span class="sxs-lookup"><span data-stu-id="29260-170">Request</span></span>
<span data-ttu-id="29260-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29260-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1650

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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="29260-172">応答</span><span class="sxs-lookup"><span data-stu-id="29260-172">Response</span></span>
<span data-ttu-id="29260-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29260-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```



