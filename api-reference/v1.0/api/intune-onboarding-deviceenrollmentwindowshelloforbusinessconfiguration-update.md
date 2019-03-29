---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3225f7fe36f5ec8a66df8424a06d8569b7c92efd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968638"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="c212e-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="c212e-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="c212e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c212e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c212e-105">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c212e-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c212e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c212e-106">Prerequisites</span></span>
<span data-ttu-id="c212e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c212e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c212e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c212e-109">Permission type</span></span>|<span data-ttu-id="c212e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c212e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c212e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c212e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c212e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c212e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c212e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c212e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c212e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-114">Not supported.</span></span>|
|<span data-ttu-id="c212e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c212e-115">Application</span></span>|<span data-ttu-id="c212e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c212e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c212e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c212e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c212e-118">Request headers</span></span>
|<span data-ttu-id="c212e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c212e-119">Header</span></span>|<span data-ttu-id="c212e-120">値</span><span class="sxs-lookup"><span data-stu-id="c212e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c212e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c212e-121">Authorization</span></span>|<span data-ttu-id="c212e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c212e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c212e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="c212e-123">Accept</span></span>|<span data-ttu-id="c212e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c212e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c212e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c212e-125">Request body</span></span>
<span data-ttu-id="c212e-126">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c212e-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="c212e-127">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c212e-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="c212e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c212e-128">Property</span></span>|<span data-ttu-id="c212e-129">型</span><span class="sxs-lookup"><span data-stu-id="c212e-129">Type</span></span>|<span data-ttu-id="c212e-130">説明</span><span class="sxs-lookup"><span data-stu-id="c212e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c212e-131">id</span><span class="sxs-lookup"><span data-stu-id="c212e-131">id</span></span>|<span data-ttu-id="c212e-132">String</span><span class="sxs-lookup"><span data-stu-id="c212e-132">String</span></span>|<span data-ttu-id="c212e-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c212e-134">displayName</span></span>|<span data-ttu-id="c212e-135">String</span><span class="sxs-lookup"><span data-stu-id="c212e-135">String</span></span>|<span data-ttu-id="c212e-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-137">description</span><span class="sxs-lookup"><span data-stu-id="c212e-137">description</span></span>|<span data-ttu-id="c212e-138">String</span><span class="sxs-lookup"><span data-stu-id="c212e-138">String</span></span>|<span data-ttu-id="c212e-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-140">priority</span><span class="sxs-lookup"><span data-stu-id="c212e-140">priority</span></span>|<span data-ttu-id="c212e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c212e-141">Int32</span></span>|<span data-ttu-id="c212e-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c212e-143">createdDateTime</span></span>|<span data-ttu-id="c212e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c212e-144">DateTimeOffset</span></span>|<span data-ttu-id="c212e-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c212e-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c212e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c212e-147">DateTimeOffset</span></span>|<span data-ttu-id="c212e-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-149">version</span><span class="sxs-lookup"><span data-stu-id="c212e-149">version</span></span>|<span data-ttu-id="c212e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c212e-150">Int32</span></span>|<span data-ttu-id="c212e-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c212e-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c212e-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c212e-152">pinMinimumLength</span></span>|<span data-ttu-id="c212e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c212e-153">Int32</span></span>|<span data-ttu-id="c212e-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-154">Not yet documented</span></span>|
|<span data-ttu-id="c212e-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="c212e-155">pinMaximumLength</span></span>|<span data-ttu-id="c212e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c212e-156">Int32</span></span>|<span data-ttu-id="c212e-157">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-157">Not yet documented</span></span>|
|<span data-ttu-id="c212e-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c212e-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="c212e-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="c212e-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c212e-160">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-160">Not yet documented.</span></span> <span data-ttu-id="c212e-161">使用可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="c212e-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c212e-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c212e-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="c212e-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="c212e-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c212e-164">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-164">Not yet documented.</span></span> <span data-ttu-id="c212e-165">使用可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="c212e-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c212e-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c212e-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="c212e-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="c212e-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c212e-168">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-168">Not yet documented.</span></span> <span data-ttu-id="c212e-169">使用可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="c212e-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c212e-170">state</span><span class="sxs-lookup"><span data-stu-id="c212e-170">state</span></span>|[<span data-ttu-id="c212e-171">購入</span><span class="sxs-lookup"><span data-stu-id="c212e-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="c212e-172">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-172">Not yet documented.</span></span> <span data-ttu-id="c212e-173">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="c212e-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="c212e-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="c212e-174">securityDeviceRequired</span></span>|<span data-ttu-id="c212e-175">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c212e-175">Boolean</span></span>|<span data-ttu-id="c212e-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-176">Not yet documented</span></span>|
|<span data-ttu-id="c212e-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="c212e-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="c212e-178">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c212e-178">Boolean</span></span>|<span data-ttu-id="c212e-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-179">Not yet documented</span></span>|
|<span data-ttu-id="c212e-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="c212e-180">remotePassportEnabled</span></span>|<span data-ttu-id="c212e-181">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c212e-181">Boolean</span></span>|<span data-ttu-id="c212e-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-182">Not yet documented</span></span>|
|<span data-ttu-id="c212e-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="c212e-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="c212e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c212e-184">Int32</span></span>|<span data-ttu-id="c212e-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-185">Not yet documented</span></span>|
|<span data-ttu-id="c212e-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="c212e-186">pinExpirationInDays</span></span>|<span data-ttu-id="c212e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="c212e-187">Int32</span></span>|<span data-ttu-id="c212e-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c212e-188">Not yet documented</span></span>|
|<span data-ttu-id="c212e-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="c212e-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="c212e-190">購入</span><span class="sxs-lookup"><span data-stu-id="c212e-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="c212e-191">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="c212e-191">Not yet documented.</span></span> <span data-ttu-id="c212e-192">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="c212e-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="c212e-193">応答</span><span class="sxs-lookup"><span data-stu-id="c212e-193">Response</span></span>
<span data-ttu-id="c212e-194">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c212e-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c212e-195">例</span><span class="sxs-lookup"><span data-stu-id="c212e-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="c212e-196">要求</span><span class="sxs-lookup"><span data-stu-id="c212e-196">Request</span></span>
<span data-ttu-id="c212e-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c212e-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c212e-198">応答</span><span class="sxs-lookup"><span data-stu-id="c212e-198">Response</span></span>
<span data-ttu-id="c212e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c212e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



