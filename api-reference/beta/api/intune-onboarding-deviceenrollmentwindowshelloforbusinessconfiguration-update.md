---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 83b475f1fe467ad73d0bdc63a3c25e3a95761e83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411471"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="a1486-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a1486-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="a1486-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1486-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1486-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1486-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1486-107">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1486-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1486-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1486-108">Prerequisites</span></span>
<span data-ttu-id="a1486-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1486-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1486-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1486-111">Permission type</span></span>|<span data-ttu-id="a1486-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1486-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1486-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1486-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1486-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1486-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1486-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1486-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-116">Not supported.</span></span>|
|<span data-ttu-id="a1486-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1486-117">Application</span></span>|<span data-ttu-id="a1486-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1486-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1486-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a1486-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1486-120">Request headers</span></span>
|<span data-ttu-id="a1486-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1486-121">Header</span></span>|<span data-ttu-id="a1486-122">値</span><span class="sxs-lookup"><span data-stu-id="a1486-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1486-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1486-123">Authorization</span></span>|<span data-ttu-id="a1486-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a1486-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1486-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1486-125">Accept</span></span>|<span data-ttu-id="a1486-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1486-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1486-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1486-127">Request body</span></span>
<span data-ttu-id="a1486-128">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1486-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="a1486-129">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a1486-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="a1486-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1486-130">Property</span></span>|<span data-ttu-id="a1486-131">型</span><span class="sxs-lookup"><span data-stu-id="a1486-131">Type</span></span>|<span data-ttu-id="a1486-132">説明</span><span class="sxs-lookup"><span data-stu-id="a1486-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1486-133">id</span><span class="sxs-lookup"><span data-stu-id="a1486-133">id</span></span>|<span data-ttu-id="a1486-134">String</span><span class="sxs-lookup"><span data-stu-id="a1486-134">String</span></span>|<span data-ttu-id="a1486-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a1486-136">displayName</span></span>|<span data-ttu-id="a1486-137">String</span><span class="sxs-lookup"><span data-stu-id="a1486-137">String</span></span>|<span data-ttu-id="a1486-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-139">説明</span><span class="sxs-lookup"><span data-stu-id="a1486-139">description</span></span>|<span data-ttu-id="a1486-140">String</span><span class="sxs-lookup"><span data-stu-id="a1486-140">String</span></span>|<span data-ttu-id="a1486-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-142">priority</span><span class="sxs-lookup"><span data-stu-id="a1486-142">priority</span></span>|<span data-ttu-id="a1486-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a1486-143">Int32</span></span>|<span data-ttu-id="a1486-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1486-145">createdDateTime</span></span>|<span data-ttu-id="a1486-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1486-146">DateTimeOffset</span></span>|<span data-ttu-id="a1486-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1486-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a1486-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1486-149">DateTimeOffset</span></span>|<span data-ttu-id="a1486-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-151">version</span><span class="sxs-lookup"><span data-stu-id="a1486-151">version</span></span>|<span data-ttu-id="a1486-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a1486-152">Int32</span></span>|<span data-ttu-id="a1486-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a1486-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1486-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a1486-154">pinMinimumLength</span></span>|<span data-ttu-id="a1486-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a1486-155">Int32</span></span>|<span data-ttu-id="a1486-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-156">Not yet documented</span></span>|
|<span data-ttu-id="a1486-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a1486-157">pinMaximumLength</span></span>|<span data-ttu-id="a1486-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a1486-158">Int32</span></span>|<span data-ttu-id="a1486-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-159">Not yet documented</span></span>|
|<span data-ttu-id="a1486-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a1486-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a1486-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a1486-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a1486-162">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-162">Not yet documented.</span></span> <span data-ttu-id="a1486-163">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="a1486-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a1486-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a1486-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a1486-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a1486-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a1486-166">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-166">Not yet documented.</span></span> <span data-ttu-id="a1486-167">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="a1486-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a1486-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a1486-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a1486-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a1486-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a1486-170">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-170">Not yet documented.</span></span> <span data-ttu-id="a1486-171">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="a1486-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a1486-172">state</span><span class="sxs-lookup"><span data-stu-id="a1486-172">state</span></span>|[<span data-ttu-id="a1486-173">有効化</span><span class="sxs-lookup"><span data-stu-id="a1486-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a1486-174">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-174">Not yet documented.</span></span> <span data-ttu-id="a1486-175">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="a1486-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a1486-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a1486-176">securityDeviceRequired</span></span>|<span data-ttu-id="a1486-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1486-177">Boolean</span></span>|<span data-ttu-id="a1486-178">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-178">Not yet documented</span></span>|
|<span data-ttu-id="a1486-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a1486-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a1486-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1486-180">Boolean</span></span>|<span data-ttu-id="a1486-181">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-181">Not yet documented</span></span>|
|<span data-ttu-id="a1486-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="a1486-182">remotePassportEnabled</span></span>|<span data-ttu-id="a1486-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1486-183">Boolean</span></span>|<span data-ttu-id="a1486-184">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-184">Not yet documented</span></span>|
|<span data-ttu-id="a1486-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a1486-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="a1486-186">Int32</span><span class="sxs-lookup"><span data-stu-id="a1486-186">Int32</span></span>|<span data-ttu-id="a1486-187">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-187">Not yet documented</span></span>|
|<span data-ttu-id="a1486-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a1486-188">pinExpirationInDays</span></span>|<span data-ttu-id="a1486-189">Int32</span><span class="sxs-lookup"><span data-stu-id="a1486-189">Int32</span></span>|<span data-ttu-id="a1486-190">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1486-190">Not yet documented</span></span>|
|<span data-ttu-id="a1486-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="a1486-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="a1486-192">有効化</span><span class="sxs-lookup"><span data-stu-id="a1486-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a1486-193">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="a1486-193">Not yet documented.</span></span> <span data-ttu-id="a1486-194">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="a1486-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1486-195">応答</span><span class="sxs-lookup"><span data-stu-id="a1486-195">Response</span></span>
<span data-ttu-id="a1486-196">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a1486-196">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1486-197">例</span><span class="sxs-lookup"><span data-stu-id="a1486-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1486-198">要求</span><span class="sxs-lookup"><span data-stu-id="a1486-198">Request</span></span>
<span data-ttu-id="a1486-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1486-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1486-200">応答</span><span class="sxs-lookup"><span data-stu-id="a1486-200">Response</span></span>
<span data-ttu-id="a1486-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1486-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




