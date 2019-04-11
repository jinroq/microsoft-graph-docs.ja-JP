---
title: deviceEnrollmentPlatformRestrictionsConfiguration の作成
description: 新しい deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189a1be56f2f6b444202b1a7e945500e321515d2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778629"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="0ad21-103">deviceEnrollmentPlatformRestrictionsConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="0ad21-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="0ad21-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ad21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ad21-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ad21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad21-106">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0ad21-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ad21-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ad21-107">Prerequisites</span></span>
<span data-ttu-id="0ad21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ad21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ad21-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ad21-110">Permission type</span></span>|<span data-ttu-id="0ad21-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ad21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ad21-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ad21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ad21-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ad21-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ad21-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ad21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ad21-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ad21-115">Not supported.</span></span>|
|<span data-ttu-id="0ad21-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ad21-116">Application</span></span>|<span data-ttu-id="0ad21-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ad21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ad21-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ad21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ad21-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ad21-119">Request headers</span></span>
|<span data-ttu-id="0ad21-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ad21-120">Header</span></span>|<span data-ttu-id="0ad21-121">値</span><span class="sxs-lookup"><span data-stu-id="0ad21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ad21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ad21-122">Authorization</span></span>|<span data-ttu-id="0ad21-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ad21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ad21-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0ad21-124">Accept</span></span>|<span data-ttu-id="0ad21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ad21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ad21-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ad21-126">Request body</span></span>
<span data-ttu-id="0ad21-127">要求本文で、deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ad21-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="0ad21-128">次の表に、deviceEnrollmentPlatformRestrictionsConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0ad21-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="0ad21-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ad21-129">Property</span></span>|<span data-ttu-id="0ad21-130">型</span><span class="sxs-lookup"><span data-stu-id="0ad21-130">Type</span></span>|<span data-ttu-id="0ad21-131">説明</span><span class="sxs-lookup"><span data-stu-id="0ad21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad21-132">id</span><span class="sxs-lookup"><span data-stu-id="0ad21-132">id</span></span>|<span data-ttu-id="0ad21-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0ad21-133">String</span></span>|<span data-ttu-id="0ad21-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="0ad21-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0ad21-135">displayName</span></span>|<span data-ttu-id="0ad21-136">String</span><span class="sxs-lookup"><span data-stu-id="0ad21-136">String</span></span>|<span data-ttu-id="0ad21-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ad21-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-138">説明</span><span class="sxs-lookup"><span data-stu-id="0ad21-138">description</span></span>|<span data-ttu-id="0ad21-139">String</span><span class="sxs-lookup"><span data-stu-id="0ad21-139">String</span></span>|<span data-ttu-id="0ad21-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ad21-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-141">priority</span><span class="sxs-lookup"><span data-stu-id="0ad21-141">priority</span></span>|<span data-ttu-id="0ad21-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0ad21-142">Int32</span></span>|<span data-ttu-id="0ad21-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ad21-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ad21-144">createdDateTime</span></span>|<span data-ttu-id="0ad21-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ad21-145">DateTimeOffset</span></span>|<span data-ttu-id="0ad21-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ad21-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ad21-147">lastModifiedDateTime</span></span>|<span data-ttu-id="0ad21-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ad21-148">DateTimeOffset</span></span>|<span data-ttu-id="0ad21-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ad21-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-150">version</span><span class="sxs-lookup"><span data-stu-id="0ad21-150">version</span></span>|<span data-ttu-id="0ad21-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0ad21-151">Int32</span></span>|<span data-ttu-id="0ad21-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ad21-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0ad21-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-153">iosRestriction</span></span>|[<span data-ttu-id="0ad21-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-155">Not yet documented</span></span>|
|<span data-ttu-id="0ad21-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-156">windowsRestriction</span></span>|[<span data-ttu-id="0ad21-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-158">Not yet documented</span></span>|
|<span data-ttu-id="0ad21-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="0ad21-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-161">Not yet documented</span></span>|
|<span data-ttu-id="0ad21-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-162">androidRestriction</span></span>|[<span data-ttu-id="0ad21-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-164">Not yet documented</span></span>|
|<span data-ttu-id="0ad21-165">androidforwork 制限</span><span class="sxs-lookup"><span data-stu-id="0ad21-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="0ad21-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-167">Not yet documented</span></span>|
|<span data-ttu-id="0ad21-168">macrestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-168">macRestriction</span></span>|[<span data-ttu-id="0ad21-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-170">Not yet documented</span></span>|
|<span data-ttu-id="0ad21-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-171">macOSRestriction</span></span>|[<span data-ttu-id="0ad21-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0ad21-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0ad21-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ad21-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0ad21-174">応答</span><span class="sxs-lookup"><span data-stu-id="0ad21-174">Response</span></span>
<span data-ttu-id="0ad21-175">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ad21-175">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ad21-176">例</span><span class="sxs-lookup"><span data-stu-id="0ad21-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ad21-177">要求</span><span class="sxs-lookup"><span data-stu-id="0ad21-177">Request</span></span>
<span data-ttu-id="0ad21-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ad21-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="0ad21-179">応答</span><span class="sxs-lookup"><span data-stu-id="0ad21-179">Response</span></span>
<span data-ttu-id="0ad21-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ad21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





