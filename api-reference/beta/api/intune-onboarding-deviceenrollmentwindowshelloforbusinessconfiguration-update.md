---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 102812ca13e4826cddad4d1d7afc4fe54f33a5d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973378"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1b017-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1b017-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="1b017-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1b017-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b017-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b017-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b017-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b017-107">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1b017-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b017-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1b017-108">Prerequisites</span></span>
<span data-ttu-id="1b017-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b017-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b017-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b017-111">Permission type</span></span>|<span data-ttu-id="1b017-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b017-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b017-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b017-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b017-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b017-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b017-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b017-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b017-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-116">Not supported.</span></span>|
|<span data-ttu-id="1b017-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b017-117">Application</span></span>|<span data-ttu-id="1b017-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b017-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b017-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1b017-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b017-120">Request headers</span></span>
|<span data-ttu-id="1b017-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b017-121">Header</span></span>|<span data-ttu-id="1b017-122">値</span><span class="sxs-lookup"><span data-stu-id="1b017-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b017-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b017-123">Authorization</span></span>|<span data-ttu-id="1b017-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1b017-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b017-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b017-125">Accept</span></span>|<span data-ttu-id="1b017-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b017-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b017-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b017-127">Request body</span></span>
<span data-ttu-id="1b017-128">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1b017-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="1b017-129">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1b017-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="1b017-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b017-130">Property</span></span>|<span data-ttu-id="1b017-131">型</span><span class="sxs-lookup"><span data-stu-id="1b017-131">Type</span></span>|<span data-ttu-id="1b017-132">説明</span><span class="sxs-lookup"><span data-stu-id="1b017-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b017-133">ID</span><span class="sxs-lookup"><span data-stu-id="1b017-133">id</span></span>|<span data-ttu-id="1b017-134">String</span><span class="sxs-lookup"><span data-stu-id="1b017-134">String</span></span>|<span data-ttu-id="1b017-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1b017-136">displayName</span></span>|<span data-ttu-id="1b017-137">String</span><span class="sxs-lookup"><span data-stu-id="1b017-137">String</span></span>|<span data-ttu-id="1b017-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-139">説明</span><span class="sxs-lookup"><span data-stu-id="1b017-139">description</span></span>|<span data-ttu-id="1b017-140">String</span><span class="sxs-lookup"><span data-stu-id="1b017-140">String</span></span>|<span data-ttu-id="1b017-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-142">priority</span><span class="sxs-lookup"><span data-stu-id="1b017-142">priority</span></span>|<span data-ttu-id="1b017-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1b017-143">Int32</span></span>|<span data-ttu-id="1b017-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b017-145">createdDateTime</span></span>|<span data-ttu-id="1b017-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b017-146">DateTimeOffset</span></span>|<span data-ttu-id="1b017-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b017-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1b017-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b017-149">DateTimeOffset</span></span>|<span data-ttu-id="1b017-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-151">version</span><span class="sxs-lookup"><span data-stu-id="1b017-151">version</span></span>|<span data-ttu-id="1b017-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1b017-152">Int32</span></span>|<span data-ttu-id="1b017-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b017-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b017-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1b017-154">pinMinimumLength</span></span>|<span data-ttu-id="1b017-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1b017-155">Int32</span></span>|<span data-ttu-id="1b017-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-156">Not yet documented</span></span>|
|<span data-ttu-id="1b017-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1b017-157">pinMaximumLength</span></span>|<span data-ttu-id="1b017-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1b017-158">Int32</span></span>|<span data-ttu-id="1b017-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-159">Not yet documented</span></span>|
|<span data-ttu-id="1b017-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1b017-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1b017-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1b017-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1b017-162">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-162">Not yet documented.</span></span> <span data-ttu-id="1b017-163">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="1b017-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1b017-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1b017-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1b017-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1b017-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1b017-166">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-166">Not yet documented.</span></span> <span data-ttu-id="1b017-167">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="1b017-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1b017-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1b017-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1b017-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1b017-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1b017-170">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-170">Not yet documented.</span></span> <span data-ttu-id="1b017-171">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="1b017-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1b017-172">state</span><span class="sxs-lookup"><span data-stu-id="1b017-172">state</span></span>|[<span data-ttu-id="1b017-173">有効化</span><span class="sxs-lookup"><span data-stu-id="1b017-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1b017-174">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-174">Not yet documented.</span></span> <span data-ttu-id="1b017-175">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="1b017-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1b017-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1b017-176">securityDeviceRequired</span></span>|<span data-ttu-id="1b017-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b017-177">Boolean</span></span>|<span data-ttu-id="1b017-178">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-178">Not yet documented</span></span>|
|<span data-ttu-id="1b017-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1b017-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1b017-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b017-180">Boolean</span></span>|<span data-ttu-id="1b017-181">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-181">Not yet documented</span></span>|
|<span data-ttu-id="1b017-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="1b017-182">remotePassportEnabled</span></span>|<span data-ttu-id="1b017-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b017-183">Boolean</span></span>|<span data-ttu-id="1b017-184">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-184">Not yet documented</span></span>|
|<span data-ttu-id="1b017-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1b017-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="1b017-186">Int32</span><span class="sxs-lookup"><span data-stu-id="1b017-186">Int32</span></span>|<span data-ttu-id="1b017-187">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-187">Not yet documented</span></span>|
|<span data-ttu-id="1b017-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1b017-188">pinExpirationInDays</span></span>|<span data-ttu-id="1b017-189">Int32</span><span class="sxs-lookup"><span data-stu-id="1b017-189">Int32</span></span>|<span data-ttu-id="1b017-190">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b017-190">Not yet documented</span></span>|
|<span data-ttu-id="1b017-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="1b017-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="1b017-192">有効化</span><span class="sxs-lookup"><span data-stu-id="1b017-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1b017-193">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="1b017-193">Not yet documented.</span></span> <span data-ttu-id="1b017-194">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="1b017-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1b017-195">応答</span><span class="sxs-lookup"><span data-stu-id="1b017-195">Response</span></span>
<span data-ttu-id="1b017-196">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1b017-196">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b017-197">例</span><span class="sxs-lookup"><span data-stu-id="1b017-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b017-198">要求</span><span class="sxs-lookup"><span data-stu-id="1b017-198">Request</span></span>
<span data-ttu-id="1b017-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1b017-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="1b017-200">応答</span><span class="sxs-lookup"><span data-stu-id="1b017-200">Response</span></span>
<span data-ttu-id="1b017-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1b017-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





