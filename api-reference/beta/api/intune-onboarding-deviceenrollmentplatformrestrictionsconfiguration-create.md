---
title: deviceEnrollmentPlatformRestrictionsConfiguration の作成
description: 新しい deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 82ff5652cb70cb05f8df5620ba1ef59f601d6645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846929"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="15c43-103">deviceEnrollmentPlatformRestrictionsConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="15c43-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="15c43-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15c43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15c43-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15c43-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15c43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15c43-107">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="15c43-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15c43-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="15c43-108">Prerequisites</span></span>
<span data-ttu-id="15c43-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15c43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15c43-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15c43-111">Permission type</span></span>|<span data-ttu-id="15c43-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="15c43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15c43-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15c43-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15c43-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c43-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15c43-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15c43-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15c43-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c43-116">Not supported.</span></span>|
|<span data-ttu-id="15c43-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15c43-117">Application</span></span>|<span data-ttu-id="15c43-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c43-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15c43-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15c43-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15c43-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15c43-120">Request headers</span></span>
|<span data-ttu-id="15c43-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15c43-121">Header</span></span>|<span data-ttu-id="15c43-122">値</span><span class="sxs-lookup"><span data-stu-id="15c43-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15c43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15c43-123">Authorization</span></span>|<span data-ttu-id="15c43-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="15c43-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15c43-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15c43-125">Accept</span></span>|<span data-ttu-id="15c43-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15c43-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c43-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="15c43-127">Request body</span></span>
<span data-ttu-id="15c43-128">要求本文で、deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="15c43-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="15c43-129">次の表に、deviceEnrollmentPlatformRestrictionsConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="15c43-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="15c43-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15c43-130">Property</span></span>|<span data-ttu-id="15c43-131">種類</span><span class="sxs-lookup"><span data-stu-id="15c43-131">Type</span></span>|<span data-ttu-id="15c43-132">説明</span><span class="sxs-lookup"><span data-stu-id="15c43-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c43-133">ID</span><span class="sxs-lookup"><span data-stu-id="15c43-133">id</span></span>|<span data-ttu-id="15c43-134">String</span><span class="sxs-lookup"><span data-stu-id="15c43-134">String</span></span>|<span data-ttu-id="15c43-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15c43-136">displayName</span></span>|<span data-ttu-id="15c43-137">String</span><span class="sxs-lookup"><span data-stu-id="15c43-137">String</span></span>|<span data-ttu-id="15c43-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-139">説明</span><span class="sxs-lookup"><span data-stu-id="15c43-139">description</span></span>|<span data-ttu-id="15c43-140">String</span><span class="sxs-lookup"><span data-stu-id="15c43-140">String</span></span>|<span data-ttu-id="15c43-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-142">priority</span><span class="sxs-lookup"><span data-stu-id="15c43-142">priority</span></span>|<span data-ttu-id="15c43-143">Int32</span><span class="sxs-lookup"><span data-stu-id="15c43-143">Int32</span></span>|<span data-ttu-id="15c43-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15c43-145">createdDateTime</span></span>|<span data-ttu-id="15c43-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15c43-146">DateTimeOffset</span></span>|<span data-ttu-id="15c43-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15c43-148">lastModifiedDateTime</span></span>|<span data-ttu-id="15c43-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15c43-149">DateTimeOffset</span></span>|<span data-ttu-id="15c43-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-151">version</span><span class="sxs-lookup"><span data-stu-id="15c43-151">version</span></span>|<span data-ttu-id="15c43-152">Int32</span><span class="sxs-lookup"><span data-stu-id="15c43-152">Int32</span></span>|<span data-ttu-id="15c43-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="15c43-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15c43-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-154">iosRestriction</span></span>|[<span data-ttu-id="15c43-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-156">Not yet documented</span></span>|
|<span data-ttu-id="15c43-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-157">windowsRestriction</span></span>|[<span data-ttu-id="15c43-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-159">Not yet documented</span></span>|
|<span data-ttu-id="15c43-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="15c43-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-162">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-162">Not yet documented</span></span>|
|<span data-ttu-id="15c43-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-163">androidRestriction</span></span>|[<span data-ttu-id="15c43-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-165">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-165">Not yet documented</span></span>|
|<span data-ttu-id="15c43-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="15c43-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-168">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-168">Not yet documented</span></span>|
|<span data-ttu-id="15c43-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-169">macRestriction</span></span>|[<span data-ttu-id="15c43-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-171">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-171">Not yet documented</span></span>|
|<span data-ttu-id="15c43-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-172">macOSRestriction</span></span>|[<span data-ttu-id="15c43-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15c43-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15c43-174">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c43-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15c43-175">応答</span><span class="sxs-lookup"><span data-stu-id="15c43-175">Response</span></span>
<span data-ttu-id="15c43-176">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15c43-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15c43-177">例</span><span class="sxs-lookup"><span data-stu-id="15c43-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="15c43-178">要求</span><span class="sxs-lookup"><span data-stu-id="15c43-178">Request</span></span>
<span data-ttu-id="15c43-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15c43-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15c43-180">応答</span><span class="sxs-lookup"><span data-stu-id="15c43-180">Response</span></span>
<span data-ttu-id="15c43-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15c43-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





