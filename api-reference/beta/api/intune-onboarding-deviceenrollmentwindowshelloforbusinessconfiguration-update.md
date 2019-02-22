---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 819083ad2081515555900d8dd44b9e039bab6711
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155952"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="f9173-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="f9173-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="f9173-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9173-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9173-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9173-106">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9173-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9173-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9173-107">Prerequisites</span></span>
<span data-ttu-id="f9173-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9173-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9173-110">Permission type</span></span>|<span data-ttu-id="f9173-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9173-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9173-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9173-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9173-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9173-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f9173-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9173-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9173-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-115">Not supported.</span></span>|
|<span data-ttu-id="f9173-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9173-116">Application</span></span>|<span data-ttu-id="f9173-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9173-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9173-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f9173-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9173-119">Request headers</span></span>
|<span data-ttu-id="f9173-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9173-120">Header</span></span>|<span data-ttu-id="f9173-121">値</span><span class="sxs-lookup"><span data-stu-id="f9173-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9173-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9173-122">Authorization</span></span>|<span data-ttu-id="f9173-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f9173-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9173-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f9173-124">Accept</span></span>|<span data-ttu-id="f9173-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9173-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9173-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9173-126">Request body</span></span>
<span data-ttu-id="f9173-127">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9173-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="f9173-128">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f9173-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="f9173-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9173-129">Property</span></span>|<span data-ttu-id="f9173-130">型</span><span class="sxs-lookup"><span data-stu-id="f9173-130">Type</span></span>|<span data-ttu-id="f9173-131">説明</span><span class="sxs-lookup"><span data-stu-id="f9173-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9173-132">id</span><span class="sxs-lookup"><span data-stu-id="f9173-132">id</span></span>|<span data-ttu-id="f9173-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f9173-133">String</span></span>|<span data-ttu-id="f9173-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="f9173-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f9173-135">displayName</span></span>|<span data-ttu-id="f9173-136">String</span><span class="sxs-lookup"><span data-stu-id="f9173-136">String</span></span>|<span data-ttu-id="f9173-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9173-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-138">説明</span><span class="sxs-lookup"><span data-stu-id="f9173-138">description</span></span>|<span data-ttu-id="f9173-139">String</span><span class="sxs-lookup"><span data-stu-id="f9173-139">String</span></span>|<span data-ttu-id="f9173-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9173-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-141">priority</span><span class="sxs-lookup"><span data-stu-id="f9173-141">priority</span></span>|<span data-ttu-id="f9173-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f9173-142">Int32</span></span>|<span data-ttu-id="f9173-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9173-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9173-144">createdDateTime</span></span>|<span data-ttu-id="f9173-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9173-145">DateTimeOffset</span></span>|<span data-ttu-id="f9173-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9173-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9173-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f9173-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9173-148">DateTimeOffset</span></span>|<span data-ttu-id="f9173-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9173-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-150">version</span><span class="sxs-lookup"><span data-stu-id="f9173-150">version</span></span>|<span data-ttu-id="f9173-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f9173-151">Int32</span></span>|<span data-ttu-id="f9173-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9173-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f9173-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f9173-153">pinMinimumLength</span></span>|<span data-ttu-id="f9173-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f9173-154">Int32</span></span>|<span data-ttu-id="f9173-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-155">Not yet documented</span></span>|
|<span data-ttu-id="f9173-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="f9173-156">pinMaximumLength</span></span>|<span data-ttu-id="f9173-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f9173-157">Int32</span></span>|<span data-ttu-id="f9173-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-158">Not yet documented</span></span>|
|<span data-ttu-id="f9173-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="f9173-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="f9173-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="f9173-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="f9173-161">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-161">Not yet documented.</span></span> <span data-ttu-id="f9173-162">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="f9173-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="f9173-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="f9173-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="f9173-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="f9173-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="f9173-165">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-165">Not yet documented.</span></span> <span data-ttu-id="f9173-166">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="f9173-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="f9173-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="f9173-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="f9173-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="f9173-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="f9173-169">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-169">Not yet documented.</span></span> <span data-ttu-id="f9173-170">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="f9173-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="f9173-171">state</span><span class="sxs-lookup"><span data-stu-id="f9173-171">state</span></span>|[<span data-ttu-id="f9173-172">購入</span><span class="sxs-lookup"><span data-stu-id="f9173-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9173-173">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-173">Not yet documented.</span></span> <span data-ttu-id="f9173-174">可能な値は `notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f9173-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f9173-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="f9173-175">securityDeviceRequired</span></span>|<span data-ttu-id="f9173-176">ブール値</span><span class="sxs-lookup"><span data-stu-id="f9173-176">Boolean</span></span>|<span data-ttu-id="f9173-177">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-177">Not yet documented</span></span>|
|<span data-ttu-id="f9173-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="f9173-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="f9173-179">ブール値</span><span class="sxs-lookup"><span data-stu-id="f9173-179">Boolean</span></span>|<span data-ttu-id="f9173-180">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-180">Not yet documented</span></span>|
|<span data-ttu-id="f9173-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="f9173-181">remotePassportEnabled</span></span>|<span data-ttu-id="f9173-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9173-182">Boolean</span></span>|<span data-ttu-id="f9173-183">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-183">Not yet documented</span></span>|
|<span data-ttu-id="f9173-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="f9173-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="f9173-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f9173-185">Int32</span></span>|<span data-ttu-id="f9173-186">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-186">Not yet documented</span></span>|
|<span data-ttu-id="f9173-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="f9173-187">pinExpirationInDays</span></span>|<span data-ttu-id="f9173-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f9173-188">Int32</span></span>|<span data-ttu-id="f9173-189">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9173-189">Not yet documented</span></span>|
|<span data-ttu-id="f9173-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="f9173-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="f9173-191">購入</span><span class="sxs-lookup"><span data-stu-id="f9173-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9173-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="f9173-192">Not yet documented.</span></span> <span data-ttu-id="f9173-193">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f9173-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f9173-194">応答</span><span class="sxs-lookup"><span data-stu-id="f9173-194">Response</span></span>
<span data-ttu-id="f9173-195">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f9173-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9173-196">例</span><span class="sxs-lookup"><span data-stu-id="f9173-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9173-197">要求</span><span class="sxs-lookup"><span data-stu-id="f9173-197">Request</span></span>
<span data-ttu-id="f9173-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9173-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f9173-199">応答</span><span class="sxs-lookup"><span data-stu-id="f9173-199">Response</span></span>
<span data-ttu-id="f9173-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9173-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




