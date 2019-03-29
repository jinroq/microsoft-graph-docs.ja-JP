---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a9cd26f0a57df1e46f15ddf80599dd275c2adcf
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956878"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="61186-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="61186-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="61186-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61186-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61186-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61186-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61186-106">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="61186-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61186-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="61186-107">Prerequisites</span></span>
<span data-ttu-id="61186-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61186-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61186-110">Permission type</span></span>|<span data-ttu-id="61186-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="61186-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61186-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61186-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61186-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61186-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61186-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61186-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61186-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61186-115">Not supported.</span></span>|
|<span data-ttu-id="61186-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61186-116">Application</span></span>|<span data-ttu-id="61186-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61186-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61186-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61186-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="61186-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61186-119">Request headers</span></span>
|<span data-ttu-id="61186-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61186-120">Header</span></span>|<span data-ttu-id="61186-121">値</span><span class="sxs-lookup"><span data-stu-id="61186-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61186-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61186-122">Authorization</span></span>|<span data-ttu-id="61186-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="61186-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61186-124">承諾</span><span class="sxs-lookup"><span data-stu-id="61186-124">Accept</span></span>|<span data-ttu-id="61186-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61186-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61186-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="61186-126">Request body</span></span>
<span data-ttu-id="61186-127">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="61186-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="61186-128">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="61186-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="61186-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61186-129">Property</span></span>|<span data-ttu-id="61186-130">型</span><span class="sxs-lookup"><span data-stu-id="61186-130">Type</span></span>|<span data-ttu-id="61186-131">説明</span><span class="sxs-lookup"><span data-stu-id="61186-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61186-132">id</span><span class="sxs-lookup"><span data-stu-id="61186-132">id</span></span>|<span data-ttu-id="61186-133">String</span><span class="sxs-lookup"><span data-stu-id="61186-133">String</span></span>|<span data-ttu-id="61186-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="61186-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-135">displayName</span><span class="sxs-lookup"><span data-stu-id="61186-135">displayName</span></span>|<span data-ttu-id="61186-136">String</span><span class="sxs-lookup"><span data-stu-id="61186-136">String</span></span>|<span data-ttu-id="61186-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61186-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-138">description</span><span class="sxs-lookup"><span data-stu-id="61186-138">description</span></span>|<span data-ttu-id="61186-139">String</span><span class="sxs-lookup"><span data-stu-id="61186-139">String</span></span>|<span data-ttu-id="61186-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61186-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-141">priority</span><span class="sxs-lookup"><span data-stu-id="61186-141">priority</span></span>|<span data-ttu-id="61186-142">Int32</span><span class="sxs-lookup"><span data-stu-id="61186-142">Int32</span></span>|<span data-ttu-id="61186-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61186-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61186-144">createdDateTime</span></span>|<span data-ttu-id="61186-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61186-145">DateTimeOffset</span></span>|<span data-ttu-id="61186-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61186-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61186-147">lastModifiedDateTime</span></span>|<span data-ttu-id="61186-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61186-148">DateTimeOffset</span></span>|<span data-ttu-id="61186-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61186-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-150">version</span><span class="sxs-lookup"><span data-stu-id="61186-150">version</span></span>|<span data-ttu-id="61186-151">Int32</span><span class="sxs-lookup"><span data-stu-id="61186-151">Int32</span></span>|<span data-ttu-id="61186-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61186-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="61186-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="61186-153">pinMinimumLength</span></span>|<span data-ttu-id="61186-154">Int32</span><span class="sxs-lookup"><span data-stu-id="61186-154">Int32</span></span>|<span data-ttu-id="61186-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-155">Not yet documented</span></span>|
|<span data-ttu-id="61186-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="61186-156">pinMaximumLength</span></span>|<span data-ttu-id="61186-157">Int32</span><span class="sxs-lookup"><span data-stu-id="61186-157">Int32</span></span>|<span data-ttu-id="61186-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-158">Not yet documented</span></span>|
|<span data-ttu-id="61186-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="61186-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="61186-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="61186-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="61186-161">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="61186-161">Not yet documented.</span></span> <span data-ttu-id="61186-162">使用可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="61186-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="61186-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="61186-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="61186-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="61186-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="61186-165">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="61186-165">Not yet documented.</span></span> <span data-ttu-id="61186-166">使用可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="61186-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="61186-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="61186-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="61186-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="61186-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="61186-169">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="61186-169">Not yet documented.</span></span> <span data-ttu-id="61186-170">使用可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="61186-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="61186-171">state</span><span class="sxs-lookup"><span data-stu-id="61186-171">state</span></span>|[<span data-ttu-id="61186-172">購入</span><span class="sxs-lookup"><span data-stu-id="61186-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="61186-173">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="61186-173">Not yet documented.</span></span> <span data-ttu-id="61186-174">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="61186-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="61186-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="61186-175">securityDeviceRequired</span></span>|<span data-ttu-id="61186-176">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="61186-176">Boolean</span></span>|<span data-ttu-id="61186-177">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-177">Not yet documented</span></span>|
|<span data-ttu-id="61186-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="61186-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="61186-179">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="61186-179">Boolean</span></span>|<span data-ttu-id="61186-180">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-180">Not yet documented</span></span>|
|<span data-ttu-id="61186-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="61186-181">remotePassportEnabled</span></span>|<span data-ttu-id="61186-182">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="61186-182">Boolean</span></span>|<span data-ttu-id="61186-183">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-183">Not yet documented</span></span>|
|<span data-ttu-id="61186-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="61186-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="61186-185">Int32</span><span class="sxs-lookup"><span data-stu-id="61186-185">Int32</span></span>|<span data-ttu-id="61186-186">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-186">Not yet documented</span></span>|
|<span data-ttu-id="61186-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="61186-187">pinExpirationInDays</span></span>|<span data-ttu-id="61186-188">Int32</span><span class="sxs-lookup"><span data-stu-id="61186-188">Int32</span></span>|<span data-ttu-id="61186-189">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61186-189">Not yet documented</span></span>|
|<span data-ttu-id="61186-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="61186-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="61186-191">購入</span><span class="sxs-lookup"><span data-stu-id="61186-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="61186-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="61186-192">Not yet documented.</span></span> <span data-ttu-id="61186-193">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="61186-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="61186-194">応答</span><span class="sxs-lookup"><span data-stu-id="61186-194">Response</span></span>
<span data-ttu-id="61186-195">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="61186-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61186-196">例</span><span class="sxs-lookup"><span data-stu-id="61186-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="61186-197">要求</span><span class="sxs-lookup"><span data-stu-id="61186-197">Request</span></span>
<span data-ttu-id="61186-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61186-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61186-199">応答</span><span class="sxs-lookup"><span data-stu-id="61186-199">Response</span></span>
<span data-ttu-id="61186-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="61186-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




