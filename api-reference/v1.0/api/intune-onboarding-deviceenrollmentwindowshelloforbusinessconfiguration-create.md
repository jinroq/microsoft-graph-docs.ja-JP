---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の作成
description: 新しい deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f86fd9fc1a8028ab983dce46998046b1515c761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983080"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="69ede-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="69ede-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="69ede-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="69ede-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69ede-105">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="69ede-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69ede-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="69ede-106">Prerequisites</span></span>
<span data-ttu-id="69ede-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ede-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69ede-109">Permission type</span></span>|<span data-ttu-id="69ede-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69ede-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ede-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69ede-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69ede-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ede-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="69ede-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69ede-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ede-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-114">Not supported.</span></span>|
|<span data-ttu-id="69ede-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69ede-115">Application</span></span>|<span data-ttu-id="69ede-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ede-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69ede-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="69ede-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69ede-118">Request headers</span></span>
|<span data-ttu-id="69ede-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69ede-119">Header</span></span>|<span data-ttu-id="69ede-120">値</span><span class="sxs-lookup"><span data-stu-id="69ede-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ede-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69ede-121">Authorization</span></span>|<span data-ttu-id="69ede-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="69ede-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ede-123">Accept</span><span class="sxs-lookup"><span data-stu-id="69ede-123">Accept</span></span>|<span data-ttu-id="69ede-124">application/json</span><span class="sxs-lookup"><span data-stu-id="69ede-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ede-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="69ede-125">Request body</span></span>
<span data-ttu-id="69ede-126">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="69ede-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="69ede-127">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="69ede-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="69ede-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69ede-128">Property</span></span>|<span data-ttu-id="69ede-129">型</span><span class="sxs-lookup"><span data-stu-id="69ede-129">Type</span></span>|<span data-ttu-id="69ede-130">説明</span><span class="sxs-lookup"><span data-stu-id="69ede-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69ede-131">ID</span><span class="sxs-lookup"><span data-stu-id="69ede-131">id</span></span>|<span data-ttu-id="69ede-132">String</span><span class="sxs-lookup"><span data-stu-id="69ede-132">String</span></span>|<span data-ttu-id="69ede-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-134">displayName</span><span class="sxs-lookup"><span data-stu-id="69ede-134">displayName</span></span>|<span data-ttu-id="69ede-135">String</span><span class="sxs-lookup"><span data-stu-id="69ede-135">String</span></span>|<span data-ttu-id="69ede-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-137">説明</span><span class="sxs-lookup"><span data-stu-id="69ede-137">description</span></span>|<span data-ttu-id="69ede-138">String</span><span class="sxs-lookup"><span data-stu-id="69ede-138">String</span></span>|<span data-ttu-id="69ede-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-140">priority</span><span class="sxs-lookup"><span data-stu-id="69ede-140">priority</span></span>|<span data-ttu-id="69ede-141">Int32</span><span class="sxs-lookup"><span data-stu-id="69ede-141">Int32</span></span>|<span data-ttu-id="69ede-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69ede-143">createdDateTime</span></span>|<span data-ttu-id="69ede-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ede-144">DateTimeOffset</span></span>|<span data-ttu-id="69ede-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69ede-146">lastModifiedDateTime</span></span>|<span data-ttu-id="69ede-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ede-147">DateTimeOffset</span></span>|<span data-ttu-id="69ede-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-149">version</span><span class="sxs-lookup"><span data-stu-id="69ede-149">version</span></span>|<span data-ttu-id="69ede-150">Int32</span><span class="sxs-lookup"><span data-stu-id="69ede-150">Int32</span></span>|<span data-ttu-id="69ede-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ede-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="69ede-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="69ede-152">pinMinimumLength</span></span>|<span data-ttu-id="69ede-153">Int32</span><span class="sxs-lookup"><span data-stu-id="69ede-153">Int32</span></span>|<span data-ttu-id="69ede-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-154">Not yet documented</span></span>|
|<span data-ttu-id="69ede-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="69ede-155">pinMaximumLength</span></span>|<span data-ttu-id="69ede-156">Int32</span><span class="sxs-lookup"><span data-stu-id="69ede-156">Int32</span></span>|<span data-ttu-id="69ede-157">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-157">Not yet documented</span></span>|
|<span data-ttu-id="69ede-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="69ede-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="69ede-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="69ede-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="69ede-160">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-160">Not yet documented.</span></span> <span data-ttu-id="69ede-161">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="69ede-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="69ede-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="69ede-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="69ede-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="69ede-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="69ede-164">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-164">Not yet documented.</span></span> <span data-ttu-id="69ede-165">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="69ede-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="69ede-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="69ede-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="69ede-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="69ede-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="69ede-168">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-168">Not yet documented.</span></span> <span data-ttu-id="69ede-169">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="69ede-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="69ede-170">state</span><span class="sxs-lookup"><span data-stu-id="69ede-170">state</span></span>|[<span data-ttu-id="69ede-171">有効化</span><span class="sxs-lookup"><span data-stu-id="69ede-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="69ede-172">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-172">Not yet documented.</span></span> <span data-ttu-id="69ede-173">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="69ede-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="69ede-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="69ede-174">securityDeviceRequired</span></span>|<span data-ttu-id="69ede-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="69ede-175">Boolean</span></span>|<span data-ttu-id="69ede-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-176">Not yet documented</span></span>|
|<span data-ttu-id="69ede-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="69ede-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="69ede-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="69ede-178">Boolean</span></span>|<span data-ttu-id="69ede-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-179">Not yet documented</span></span>|
|<span data-ttu-id="69ede-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="69ede-180">remotePassportEnabled</span></span>|<span data-ttu-id="69ede-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="69ede-181">Boolean</span></span>|<span data-ttu-id="69ede-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-182">Not yet documented</span></span>|
|<span data-ttu-id="69ede-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="69ede-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="69ede-184">Int32</span><span class="sxs-lookup"><span data-stu-id="69ede-184">Int32</span></span>|<span data-ttu-id="69ede-185">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-185">Not yet documented</span></span>|
|<span data-ttu-id="69ede-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="69ede-186">pinExpirationInDays</span></span>|<span data-ttu-id="69ede-187">Int32</span><span class="sxs-lookup"><span data-stu-id="69ede-187">Int32</span></span>|<span data-ttu-id="69ede-188">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="69ede-188">Not yet documented</span></span>|
|<span data-ttu-id="69ede-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="69ede-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="69ede-190">有効化</span><span class="sxs-lookup"><span data-stu-id="69ede-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="69ede-191">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="69ede-191">Not yet documented.</span></span> <span data-ttu-id="69ede-192">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="69ede-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="69ede-193">応答</span><span class="sxs-lookup"><span data-stu-id="69ede-193">Response</span></span>
<span data-ttu-id="69ede-194">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69ede-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ede-195">例</span><span class="sxs-lookup"><span data-stu-id="69ede-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="69ede-196">要求</span><span class="sxs-lookup"><span data-stu-id="69ede-196">Request</span></span>
<span data-ttu-id="69ede-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69ede-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69ede-198">応答</span><span class="sxs-lookup"><span data-stu-id="69ede-198">Response</span></span>
<span data-ttu-id="69ede-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69ede-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



