---
title: deviceEnrollmentPlatformRestrictionsConfiguration の更新
description: deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b09aff97602974fbd4751a9392a8ff10796043
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139824"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="9f8fa-103">deviceEnrollmentPlatformRestrictionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9f8fa-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="9f8fa-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f8fa-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f8fa-106">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f8fa-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9f8fa-107">Prerequisites</span></span>
<span data-ttu-id="9f8fa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f8fa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f8fa-110">Permission type</span></span>|<span data-ttu-id="9f8fa-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f8fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f8fa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f8fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f8fa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f8fa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f8fa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f8fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f8fa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-115">Not supported.</span></span>|
|<span data-ttu-id="9f8fa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f8fa-116">Application</span></span>|<span data-ttu-id="9f8fa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f8fa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f8fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f8fa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f8fa-119">Request headers</span></span>
|<span data-ttu-id="9f8fa-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f8fa-120">Header</span></span>|<span data-ttu-id="9f8fa-121">値</span><span class="sxs-lookup"><span data-stu-id="9f8fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f8fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f8fa-122">Authorization</span></span>|<span data-ttu-id="9f8fa-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f8fa-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9f8fa-124">Accept</span></span>|<span data-ttu-id="9f8fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f8fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f8fa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f8fa-126">Request body</span></span>
<span data-ttu-id="9f8fa-127">要求本文で、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="9f8fa-128">次の表に、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="9f8fa-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f8fa-129">Property</span></span>|<span data-ttu-id="9f8fa-130">型</span><span class="sxs-lookup"><span data-stu-id="9f8fa-130">Type</span></span>|<span data-ttu-id="9f8fa-131">説明</span><span class="sxs-lookup"><span data-stu-id="9f8fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f8fa-132">id</span><span class="sxs-lookup"><span data-stu-id="9f8fa-132">id</span></span>|<span data-ttu-id="9f8fa-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9f8fa-133">String</span></span>|<span data-ttu-id="9f8fa-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="9f8fa-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9f8fa-135">displayName</span></span>|<span data-ttu-id="9f8fa-136">String</span><span class="sxs-lookup"><span data-stu-id="9f8fa-136">String</span></span>|<span data-ttu-id="9f8fa-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f8fa-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-138">説明</span><span class="sxs-lookup"><span data-stu-id="9f8fa-138">description</span></span>|<span data-ttu-id="9f8fa-139">String</span><span class="sxs-lookup"><span data-stu-id="9f8fa-139">String</span></span>|<span data-ttu-id="9f8fa-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f8fa-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-141">priority</span><span class="sxs-lookup"><span data-stu-id="9f8fa-141">priority</span></span>|<span data-ttu-id="9f8fa-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9f8fa-142">Int32</span></span>|<span data-ttu-id="9f8fa-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f8fa-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f8fa-144">createdDateTime</span></span>|<span data-ttu-id="9f8fa-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f8fa-145">DateTimeOffset</span></span>|<span data-ttu-id="9f8fa-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f8fa-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f8fa-147">lastModifiedDateTime</span></span>|<span data-ttu-id="9f8fa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f8fa-148">DateTimeOffset</span></span>|<span data-ttu-id="9f8fa-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f8fa-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-150">version</span><span class="sxs-lookup"><span data-stu-id="9f8fa-150">version</span></span>|<span data-ttu-id="9f8fa-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9f8fa-151">Int32</span></span>|<span data-ttu-id="9f8fa-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f8fa-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9f8fa-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-153">iosRestriction</span></span>|[<span data-ttu-id="9f8fa-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-155">Not yet documented</span></span>|
|<span data-ttu-id="9f8fa-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-156">windowsRestriction</span></span>|[<span data-ttu-id="9f8fa-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-158">Not yet documented</span></span>|
|<span data-ttu-id="9f8fa-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="9f8fa-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-161">Not yet documented</span></span>|
|<span data-ttu-id="9f8fa-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-162">androidRestriction</span></span>|[<span data-ttu-id="9f8fa-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-164">Not yet documented</span></span>|
|<span data-ttu-id="9f8fa-165">androidforwork 制限</span><span class="sxs-lookup"><span data-stu-id="9f8fa-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="9f8fa-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-167">Not yet documented</span></span>|
|<span data-ttu-id="9f8fa-168">macrestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-168">macRestriction</span></span>|[<span data-ttu-id="9f8fa-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-170">Not yet documented</span></span>|
|<span data-ttu-id="9f8fa-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-171">macOSRestriction</span></span>|[<span data-ttu-id="9f8fa-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9f8fa-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9f8fa-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f8fa-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9f8fa-174">応答</span><span class="sxs-lookup"><span data-stu-id="9f8fa-174">Response</span></span>
<span data-ttu-id="9f8fa-175">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f8fa-176">例</span><span class="sxs-lookup"><span data-stu-id="9f8fa-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f8fa-177">要求</span><span class="sxs-lookup"><span data-stu-id="9f8fa-177">Request</span></span>
<span data-ttu-id="9f8fa-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f8fa-179">応答</span><span class="sxs-lookup"><span data-stu-id="9f8fa-179">Response</span></span>
<span data-ttu-id="9f8fa-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f8fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




