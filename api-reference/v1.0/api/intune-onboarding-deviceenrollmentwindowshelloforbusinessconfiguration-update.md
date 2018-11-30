---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: f91067a57dc4da7dc7d4850f72fbe267f364c6e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024280"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="67bec-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="67bec-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="67bec-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67bec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67bec-105">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="67bec-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67bec-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="67bec-106">Prerequisites</span></span>
<span data-ttu-id="67bec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bec-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67bec-109">Permission type</span></span>|<span data-ttu-id="67bec-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67bec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67bec-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67bec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67bec-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bec-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67bec-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67bec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67bec-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-114">Not supported.</span></span>|
|<span data-ttu-id="67bec-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67bec-115">Application</span></span>|<span data-ttu-id="67bec-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67bec-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67bec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="67bec-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67bec-118">Request headers</span></span>
|<span data-ttu-id="67bec-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67bec-119">Header</span></span>|<span data-ttu-id="67bec-120">値</span><span class="sxs-lookup"><span data-stu-id="67bec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67bec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67bec-121">Authorization</span></span>|<span data-ttu-id="67bec-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="67bec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67bec-123">Accept</span><span class="sxs-lookup"><span data-stu-id="67bec-123">Accept</span></span>|<span data-ttu-id="67bec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67bec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bec-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67bec-125">Request body</span></span>
<span data-ttu-id="67bec-126">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67bec-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="67bec-127">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67bec-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="67bec-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67bec-128">Property</span></span>|<span data-ttu-id="67bec-129">型</span><span class="sxs-lookup"><span data-stu-id="67bec-129">Type</span></span>|<span data-ttu-id="67bec-130">説明</span><span class="sxs-lookup"><span data-stu-id="67bec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bec-131">id</span><span class="sxs-lookup"><span data-stu-id="67bec-131">id</span></span>|<span data-ttu-id="67bec-132">String</span><span class="sxs-lookup"><span data-stu-id="67bec-132">String</span></span>|<span data-ttu-id="67bec-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-134">displayName</span><span class="sxs-lookup"><span data-stu-id="67bec-134">displayName</span></span>|<span data-ttu-id="67bec-135">String</span><span class="sxs-lookup"><span data-stu-id="67bec-135">String</span></span>|<span data-ttu-id="67bec-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-137">説明</span><span class="sxs-lookup"><span data-stu-id="67bec-137">description</span></span>|<span data-ttu-id="67bec-138">String</span><span class="sxs-lookup"><span data-stu-id="67bec-138">String</span></span>|<span data-ttu-id="67bec-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-140">priority</span><span class="sxs-lookup"><span data-stu-id="67bec-140">priority</span></span>|<span data-ttu-id="67bec-141">Int32</span><span class="sxs-lookup"><span data-stu-id="67bec-141">Int32</span></span>|<span data-ttu-id="67bec-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67bec-143">createdDateTime</span></span>|<span data-ttu-id="67bec-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bec-144">DateTimeOffset</span></span>|<span data-ttu-id="67bec-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67bec-146">lastModifiedDateTime</span></span>|<span data-ttu-id="67bec-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bec-147">DateTimeOffset</span></span>|<span data-ttu-id="67bec-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-149">version</span><span class="sxs-lookup"><span data-stu-id="67bec-149">version</span></span>|<span data-ttu-id="67bec-150">Int32</span><span class="sxs-lookup"><span data-stu-id="67bec-150">Int32</span></span>|<span data-ttu-id="67bec-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67bec-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="67bec-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="67bec-152">pinMinimumLength</span></span>|<span data-ttu-id="67bec-153">Int32</span><span class="sxs-lookup"><span data-stu-id="67bec-153">Int32</span></span>|<span data-ttu-id="67bec-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-154">Not yet documented</span></span>|
|<span data-ttu-id="67bec-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="67bec-155">pinMaximumLength</span></span>|<span data-ttu-id="67bec-156">Int32</span><span class="sxs-lookup"><span data-stu-id="67bec-156">Int32</span></span>|<span data-ttu-id="67bec-157">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-157">Not yet documented</span></span>|
|<span data-ttu-id="67bec-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="67bec-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="67bec-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="67bec-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="67bec-160">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-160">Not yet documented.</span></span> <span data-ttu-id="67bec-161">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="67bec-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="67bec-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="67bec-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="67bec-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="67bec-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="67bec-164">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-164">Not yet documented.</span></span> <span data-ttu-id="67bec-165">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="67bec-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="67bec-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="67bec-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="67bec-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="67bec-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="67bec-168">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-168">Not yet documented.</span></span> <span data-ttu-id="67bec-169">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="67bec-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="67bec-170">ステート</span><span class="sxs-lookup"><span data-stu-id="67bec-170">state</span></span>|[<span data-ttu-id="67bec-171">有効化</span><span class="sxs-lookup"><span data-stu-id="67bec-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="67bec-172">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-172">Not yet documented.</span></span> <span data-ttu-id="67bec-173">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="67bec-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="67bec-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="67bec-174">securityDeviceRequired</span></span>|<span data-ttu-id="67bec-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="67bec-175">Boolean</span></span>|<span data-ttu-id="67bec-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-176">Not yet documented</span></span>|
|<span data-ttu-id="67bec-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="67bec-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="67bec-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="67bec-178">Boolean</span></span>|<span data-ttu-id="67bec-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-179">Not yet documented</span></span>|
|<span data-ttu-id="67bec-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="67bec-180">remotePassportEnabled</span></span>|<span data-ttu-id="67bec-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="67bec-181">Boolean</span></span>|<span data-ttu-id="67bec-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-182">Not yet documented</span></span>|
|<span data-ttu-id="67bec-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="67bec-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="67bec-184">Int32</span><span class="sxs-lookup"><span data-stu-id="67bec-184">Int32</span></span>|<span data-ttu-id="67bec-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-185">Not yet documented</span></span>|
|<span data-ttu-id="67bec-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="67bec-186">pinExpirationInDays</span></span>|<span data-ttu-id="67bec-187">Int32</span><span class="sxs-lookup"><span data-stu-id="67bec-187">Int32</span></span>|<span data-ttu-id="67bec-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67bec-188">Not yet documented</span></span>|
|<span data-ttu-id="67bec-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="67bec-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="67bec-190">有効化</span><span class="sxs-lookup"><span data-stu-id="67bec-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="67bec-191">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="67bec-191">Not yet documented.</span></span> <span data-ttu-id="67bec-192">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="67bec-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="67bec-193">応答</span><span class="sxs-lookup"><span data-stu-id="67bec-193">Response</span></span>
<span data-ttu-id="67bec-194">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="67bec-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67bec-195">例</span><span class="sxs-lookup"><span data-stu-id="67bec-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="67bec-196">要求</span><span class="sxs-lookup"><span data-stu-id="67bec-196">Request</span></span>
<span data-ttu-id="67bec-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67bec-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67bec-198">応答</span><span class="sxs-lookup"><span data-stu-id="67bec-198">Response</span></span>
<span data-ttu-id="67bec-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67bec-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



