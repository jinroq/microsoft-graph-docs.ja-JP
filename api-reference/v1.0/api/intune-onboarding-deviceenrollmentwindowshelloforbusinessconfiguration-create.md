---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の作成
description: 新しい deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6fb875986a1d866d530932765cf88ef50cc4844
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254843"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="49831-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="49831-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="49831-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49831-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49831-105">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="49831-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49831-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="49831-106">Prerequisites</span></span>
<span data-ttu-id="49831-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49831-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49831-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49831-109">Permission type</span></span>|<span data-ttu-id="49831-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="49831-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49831-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49831-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49831-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49831-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49831-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49831-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49831-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49831-114">Not supported.</span></span>|
|<span data-ttu-id="49831-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49831-115">Application</span></span>|<span data-ttu-id="49831-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49831-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49831-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49831-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49831-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49831-118">Request headers</span></span>
|<span data-ttu-id="49831-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49831-119">Header</span></span>|<span data-ttu-id="49831-120">値</span><span class="sxs-lookup"><span data-stu-id="49831-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49831-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49831-121">Authorization</span></span>|<span data-ttu-id="49831-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="49831-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49831-123">承諾</span><span class="sxs-lookup"><span data-stu-id="49831-123">Accept</span></span>|<span data-ttu-id="49831-124">application/json</span><span class="sxs-lookup"><span data-stu-id="49831-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49831-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="49831-125">Request body</span></span>
<span data-ttu-id="49831-126">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="49831-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="49831-127">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="49831-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="49831-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49831-128">Property</span></span>|<span data-ttu-id="49831-129">型</span><span class="sxs-lookup"><span data-stu-id="49831-129">Type</span></span>|<span data-ttu-id="49831-130">説明</span><span class="sxs-lookup"><span data-stu-id="49831-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49831-131">id</span><span class="sxs-lookup"><span data-stu-id="49831-131">id</span></span>|<span data-ttu-id="49831-132">String</span><span class="sxs-lookup"><span data-stu-id="49831-132">String</span></span>|<span data-ttu-id="49831-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-134">displayName</span><span class="sxs-lookup"><span data-stu-id="49831-134">displayName</span></span>|<span data-ttu-id="49831-135">String</span><span class="sxs-lookup"><span data-stu-id="49831-135">String</span></span>|<span data-ttu-id="49831-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-137">説明</span><span class="sxs-lookup"><span data-stu-id="49831-137">description</span></span>|<span data-ttu-id="49831-138">String</span><span class="sxs-lookup"><span data-stu-id="49831-138">String</span></span>|<span data-ttu-id="49831-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-140">priority</span><span class="sxs-lookup"><span data-stu-id="49831-140">priority</span></span>|<span data-ttu-id="49831-141">Int32</span><span class="sxs-lookup"><span data-stu-id="49831-141">Int32</span></span>|<span data-ttu-id="49831-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49831-143">createdDateTime</span></span>|<span data-ttu-id="49831-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49831-144">DateTimeOffset</span></span>|<span data-ttu-id="49831-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49831-146">lastModifiedDateTime</span></span>|<span data-ttu-id="49831-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49831-147">DateTimeOffset</span></span>|<span data-ttu-id="49831-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-149">version</span><span class="sxs-lookup"><span data-stu-id="49831-149">version</span></span>|<span data-ttu-id="49831-150">Int32</span><span class="sxs-lookup"><span data-stu-id="49831-150">Int32</span></span>|<span data-ttu-id="49831-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="49831-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49831-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="49831-152">pinMinimumLength</span></span>|<span data-ttu-id="49831-153">Int32</span><span class="sxs-lookup"><span data-stu-id="49831-153">Int32</span></span>|<span data-ttu-id="49831-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-154">Not yet documented</span></span>|
|<span data-ttu-id="49831-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="49831-155">pinMaximumLength</span></span>|<span data-ttu-id="49831-156">Int32</span><span class="sxs-lookup"><span data-stu-id="49831-156">Int32</span></span>|<span data-ttu-id="49831-157">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-157">Not yet documented</span></span>|
|<span data-ttu-id="49831-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="49831-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="49831-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="49831-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="49831-160">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="49831-160">Not yet documented.</span></span> <span data-ttu-id="49831-161">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="49831-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="49831-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="49831-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="49831-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="49831-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="49831-164">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="49831-164">Not yet documented.</span></span> <span data-ttu-id="49831-165">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="49831-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="49831-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="49831-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="49831-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="49831-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="49831-168">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="49831-168">Not yet documented.</span></span> <span data-ttu-id="49831-169">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="49831-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="49831-170">state</span><span class="sxs-lookup"><span data-stu-id="49831-170">state</span></span>|[<span data-ttu-id="49831-171">購入</span><span class="sxs-lookup"><span data-stu-id="49831-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="49831-172">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="49831-172">Not yet documented.</span></span> <span data-ttu-id="49831-173">可能な値は `notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="49831-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="49831-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="49831-174">securityDeviceRequired</span></span>|<span data-ttu-id="49831-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="49831-175">Boolean</span></span>|<span data-ttu-id="49831-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-176">Not yet documented</span></span>|
|<span data-ttu-id="49831-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="49831-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="49831-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="49831-178">Boolean</span></span>|<span data-ttu-id="49831-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-179">Not yet documented</span></span>|
|<span data-ttu-id="49831-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="49831-180">remotePassportEnabled</span></span>|<span data-ttu-id="49831-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="49831-181">Boolean</span></span>|<span data-ttu-id="49831-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-182">Not yet documented</span></span>|
|<span data-ttu-id="49831-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="49831-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="49831-184">Int32</span><span class="sxs-lookup"><span data-stu-id="49831-184">Int32</span></span>|<span data-ttu-id="49831-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-185">Not yet documented</span></span>|
|<span data-ttu-id="49831-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="49831-186">pinExpirationInDays</span></span>|<span data-ttu-id="49831-187">Int32</span><span class="sxs-lookup"><span data-stu-id="49831-187">Int32</span></span>|<span data-ttu-id="49831-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49831-188">Not yet documented</span></span>|
|<span data-ttu-id="49831-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="49831-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="49831-190">購入</span><span class="sxs-lookup"><span data-stu-id="49831-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="49831-191">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="49831-191">Not yet documented.</span></span> <span data-ttu-id="49831-192">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="49831-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="49831-193">応答</span><span class="sxs-lookup"><span data-stu-id="49831-193">Response</span></span>
<span data-ttu-id="49831-194">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="49831-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49831-195">例</span><span class="sxs-lookup"><span data-stu-id="49831-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="49831-196">要求</span><span class="sxs-lookup"><span data-stu-id="49831-196">Request</span></span>
<span data-ttu-id="49831-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49831-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="49831-198">応答</span><span class="sxs-lookup"><span data-stu-id="49831-198">Response</span></span>
<span data-ttu-id="49831-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49831-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```



