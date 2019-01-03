---
title: deviceEnrollmentPlatformRestrictionsConfiguration の作成
description: 新しい deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 2815043ae2a0c6f8c2130c413b15337c05fc1749
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324263"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="9b4b3-103">deviceEnrollmentPlatformRestrictionsConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="9b4b3-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="9b4b3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b4b3-105">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b4b3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b4b3-106">Prerequisites</span></span>
<span data-ttu-id="9b4b3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4b3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b4b3-109">Permission type</span></span>|<span data-ttu-id="9b4b3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b4b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b4b3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b4b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b4b3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b4b3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b4b3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b4b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b4b3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-114">Not supported.</span></span>|
|<span data-ttu-id="9b4b3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b4b3-115">Application</span></span>|<span data-ttu-id="9b4b3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b4b3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b4b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9b4b3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b4b3-118">Request headers</span></span>
|<span data-ttu-id="9b4b3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b4b3-119">Header</span></span>|<span data-ttu-id="9b4b3-120">値</span><span class="sxs-lookup"><span data-stu-id="9b4b3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b4b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b4b3-121">Authorization</span></span>|<span data-ttu-id="9b4b3-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b4b3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9b4b3-123">Accept</span></span>|<span data-ttu-id="9b4b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b4b3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4b3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b4b3-125">Request body</span></span>
<span data-ttu-id="9b4b3-126">要求本文で、deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="9b4b3-127">次の表に、deviceEnrollmentPlatformRestrictionsConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="9b4b3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4b3-128">Property</span></span>|<span data-ttu-id="9b4b3-129">種類</span><span class="sxs-lookup"><span data-stu-id="9b4b3-129">Type</span></span>|<span data-ttu-id="9b4b3-130">説明</span><span class="sxs-lookup"><span data-stu-id="9b4b3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4b3-131">ID</span><span class="sxs-lookup"><span data-stu-id="9b4b3-131">id</span></span>|<span data-ttu-id="9b4b3-132">String</span><span class="sxs-lookup"><span data-stu-id="9b4b3-132">String</span></span>|<span data-ttu-id="9b4b3-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9b4b3-134">displayName</span></span>|<span data-ttu-id="9b4b3-135">String</span><span class="sxs-lookup"><span data-stu-id="9b4b3-135">String</span></span>|<span data-ttu-id="9b4b3-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-137">説明</span><span class="sxs-lookup"><span data-stu-id="9b4b3-137">description</span></span>|<span data-ttu-id="9b4b3-138">String</span><span class="sxs-lookup"><span data-stu-id="9b4b3-138">String</span></span>|<span data-ttu-id="9b4b3-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-140">priority</span><span class="sxs-lookup"><span data-stu-id="9b4b3-140">priority</span></span>|<span data-ttu-id="9b4b3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4b3-141">Int32</span></span>|<span data-ttu-id="9b4b3-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b4b3-143">createdDateTime</span></span>|<span data-ttu-id="9b4b3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b4b3-144">DateTimeOffset</span></span>|<span data-ttu-id="9b4b3-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b4b3-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9b4b3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b4b3-147">DateTimeOffset</span></span>|<span data-ttu-id="9b4b3-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-149">version</span><span class="sxs-lookup"><span data-stu-id="9b4b3-149">version</span></span>|<span data-ttu-id="9b4b3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4b3-150">Int32</span></span>|<span data-ttu-id="9b4b3-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b4b3-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9b4b3-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-152">iosRestriction</span></span>|[<span data-ttu-id="9b4b3-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9b4b3-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4b3-154">Not yet documented</span></span>|
|<span data-ttu-id="9b4b3-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-155">windowsRestriction</span></span>|[<span data-ttu-id="9b4b3-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9b4b3-157">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4b3-157">Not yet documented</span></span>|
|<span data-ttu-id="9b4b3-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="9b4b3-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9b4b3-160">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4b3-160">Not yet documented</span></span>|
|<span data-ttu-id="9b4b3-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-161">androidRestriction</span></span>|[<span data-ttu-id="9b4b3-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9b4b3-163">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4b3-163">Not yet documented</span></span>|
|<span data-ttu-id="9b4b3-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-164">macOSRestriction</span></span>|[<span data-ttu-id="9b4b3-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9b4b3-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9b4b3-166">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4b3-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b4b3-167">応答</span><span class="sxs-lookup"><span data-stu-id="9b4b3-167">Response</span></span>
<span data-ttu-id="9b4b3-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4b3-169">例</span><span class="sxs-lookup"><span data-stu-id="9b4b3-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b4b3-170">要求</span><span class="sxs-lookup"><span data-stu-id="9b4b3-170">Request</span></span>
<span data-ttu-id="9b4b3-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="9b4b3-172">応答</span><span class="sxs-lookup"><span data-stu-id="9b4b3-172">Response</span></span>
<span data-ttu-id="9b4b3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b4b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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


