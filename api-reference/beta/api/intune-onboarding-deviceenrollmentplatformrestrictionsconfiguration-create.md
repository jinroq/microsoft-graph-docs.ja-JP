---
title: deviceEnrollmentPlatformRestrictionsConfiguration の作成
description: 新しい deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a7eeaef064a17d3c5650366d927ae83695ac704
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956081"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="5acd8-103">deviceEnrollmentPlatformRestrictionsConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="5acd8-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="5acd8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5acd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5acd8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5acd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5acd8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5acd8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5acd8-107">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5acd8-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5acd8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5acd8-108">Prerequisites</span></span>
<span data-ttu-id="5acd8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5acd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5acd8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5acd8-111">Permission type</span></span>|<span data-ttu-id="5acd8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5acd8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5acd8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5acd8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5acd8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5acd8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5acd8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5acd8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5acd8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5acd8-116">Not supported.</span></span>|
|<span data-ttu-id="5acd8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5acd8-117">Application</span></span>|<span data-ttu-id="5acd8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5acd8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5acd8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5acd8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5acd8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5acd8-120">Request headers</span></span>
|<span data-ttu-id="5acd8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5acd8-121">Header</span></span>|<span data-ttu-id="5acd8-122">値</span><span class="sxs-lookup"><span data-stu-id="5acd8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5acd8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5acd8-123">Authorization</span></span>|<span data-ttu-id="5acd8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5acd8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5acd8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5acd8-125">Accept</span></span>|<span data-ttu-id="5acd8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5acd8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5acd8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5acd8-127">Request body</span></span>
<span data-ttu-id="5acd8-128">要求本文で、deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5acd8-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="5acd8-129">次の表に、deviceEnrollmentPlatformRestrictionsConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5acd8-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="5acd8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5acd8-130">Property</span></span>|<span data-ttu-id="5acd8-131">型</span><span class="sxs-lookup"><span data-stu-id="5acd8-131">Type</span></span>|<span data-ttu-id="5acd8-132">説明</span><span class="sxs-lookup"><span data-stu-id="5acd8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5acd8-133">ID</span><span class="sxs-lookup"><span data-stu-id="5acd8-133">id</span></span>|<span data-ttu-id="5acd8-134">String</span><span class="sxs-lookup"><span data-stu-id="5acd8-134">String</span></span>|<span data-ttu-id="5acd8-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5acd8-136">displayName</span></span>|<span data-ttu-id="5acd8-137">String</span><span class="sxs-lookup"><span data-stu-id="5acd8-137">String</span></span>|<span data-ttu-id="5acd8-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-139">説明</span><span class="sxs-lookup"><span data-stu-id="5acd8-139">description</span></span>|<span data-ttu-id="5acd8-140">String</span><span class="sxs-lookup"><span data-stu-id="5acd8-140">String</span></span>|<span data-ttu-id="5acd8-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-142">priority</span><span class="sxs-lookup"><span data-stu-id="5acd8-142">priority</span></span>|<span data-ttu-id="5acd8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5acd8-143">Int32</span></span>|<span data-ttu-id="5acd8-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5acd8-145">createdDateTime</span></span>|<span data-ttu-id="5acd8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5acd8-146">DateTimeOffset</span></span>|<span data-ttu-id="5acd8-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5acd8-148">lastModifiedDateTime</span></span>|<span data-ttu-id="5acd8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5acd8-149">DateTimeOffset</span></span>|<span data-ttu-id="5acd8-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-151">version</span><span class="sxs-lookup"><span data-stu-id="5acd8-151">version</span></span>|<span data-ttu-id="5acd8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5acd8-152">Int32</span></span>|<span data-ttu-id="5acd8-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5acd8-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5acd8-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-154">iosRestriction</span></span>|[<span data-ttu-id="5acd8-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-156">Not yet documented</span></span>|
|<span data-ttu-id="5acd8-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-157">windowsRestriction</span></span>|[<span data-ttu-id="5acd8-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-159">Not yet documented</span></span>|
|<span data-ttu-id="5acd8-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="5acd8-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-162">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-162">Not yet documented</span></span>|
|<span data-ttu-id="5acd8-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-163">androidRestriction</span></span>|[<span data-ttu-id="5acd8-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-165">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-165">Not yet documented</span></span>|
|<span data-ttu-id="5acd8-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="5acd8-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-168">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-168">Not yet documented</span></span>|
|<span data-ttu-id="5acd8-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-169">macRestriction</span></span>|[<span data-ttu-id="5acd8-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-171">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-171">Not yet documented</span></span>|
|<span data-ttu-id="5acd8-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-172">macOSRestriction</span></span>|[<span data-ttu-id="5acd8-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5acd8-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5acd8-174">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5acd8-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5acd8-175">応答</span><span class="sxs-lookup"><span data-stu-id="5acd8-175">Response</span></span>
<span data-ttu-id="5acd8-176">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5acd8-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5acd8-177">例</span><span class="sxs-lookup"><span data-stu-id="5acd8-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="5acd8-178">要求</span><span class="sxs-lookup"><span data-stu-id="5acd8-178">Request</span></span>
<span data-ttu-id="5acd8-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5acd8-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 2295

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="5acd8-180">応答</span><span class="sxs-lookup"><span data-stu-id="5acd8-180">Response</span></span>
<span data-ttu-id="5acd8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5acd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





