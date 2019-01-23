---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の作成
description: 新しい deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ac406b338d70761c8b14c9100d2eca4cedcb7fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416147"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="33eba-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="33eba-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="33eba-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33eba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33eba-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33eba-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33eba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33eba-107">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="33eba-107">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33eba-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="33eba-108">Prerequisites</span></span>
<span data-ttu-id="33eba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33eba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33eba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33eba-111">Permission type</span></span>|<span data-ttu-id="33eba-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33eba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33eba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33eba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33eba-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33eba-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="33eba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33eba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33eba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-116">Not supported.</span></span>|
|<span data-ttu-id="33eba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33eba-117">Application</span></span>|<span data-ttu-id="33eba-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33eba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33eba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33eba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33eba-120">Request headers</span></span>
|<span data-ttu-id="33eba-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33eba-121">Header</span></span>|<span data-ttu-id="33eba-122">値</span><span class="sxs-lookup"><span data-stu-id="33eba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33eba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33eba-123">Authorization</span></span>|<span data-ttu-id="33eba-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="33eba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33eba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33eba-125">Accept</span></span>|<span data-ttu-id="33eba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33eba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33eba-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="33eba-127">Request body</span></span>
<span data-ttu-id="33eba-128">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="33eba-128">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="33eba-129">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="33eba-129">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="33eba-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33eba-130">Property</span></span>|<span data-ttu-id="33eba-131">型</span><span class="sxs-lookup"><span data-stu-id="33eba-131">Type</span></span>|<span data-ttu-id="33eba-132">説明</span><span class="sxs-lookup"><span data-stu-id="33eba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33eba-133">id</span><span class="sxs-lookup"><span data-stu-id="33eba-133">id</span></span>|<span data-ttu-id="33eba-134">String</span><span class="sxs-lookup"><span data-stu-id="33eba-134">String</span></span>|<span data-ttu-id="33eba-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="33eba-136">displayName</span></span>|<span data-ttu-id="33eba-137">String</span><span class="sxs-lookup"><span data-stu-id="33eba-137">String</span></span>|<span data-ttu-id="33eba-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-139">説明</span><span class="sxs-lookup"><span data-stu-id="33eba-139">description</span></span>|<span data-ttu-id="33eba-140">String</span><span class="sxs-lookup"><span data-stu-id="33eba-140">String</span></span>|<span data-ttu-id="33eba-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-142">priority</span><span class="sxs-lookup"><span data-stu-id="33eba-142">priority</span></span>|<span data-ttu-id="33eba-143">Int32</span><span class="sxs-lookup"><span data-stu-id="33eba-143">Int32</span></span>|<span data-ttu-id="33eba-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33eba-145">createdDateTime</span></span>|<span data-ttu-id="33eba-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33eba-146">DateTimeOffset</span></span>|<span data-ttu-id="33eba-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33eba-148">lastModifiedDateTime</span></span>|<span data-ttu-id="33eba-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33eba-149">DateTimeOffset</span></span>|<span data-ttu-id="33eba-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-151">version</span><span class="sxs-lookup"><span data-stu-id="33eba-151">version</span></span>|<span data-ttu-id="33eba-152">Int32</span><span class="sxs-lookup"><span data-stu-id="33eba-152">Int32</span></span>|<span data-ttu-id="33eba-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="33eba-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="33eba-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="33eba-154">pinMinimumLength</span></span>|<span data-ttu-id="33eba-155">Int32</span><span class="sxs-lookup"><span data-stu-id="33eba-155">Int32</span></span>|<span data-ttu-id="33eba-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-156">Not yet documented</span></span>|
|<span data-ttu-id="33eba-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="33eba-157">pinMaximumLength</span></span>|<span data-ttu-id="33eba-158">Int32</span><span class="sxs-lookup"><span data-stu-id="33eba-158">Int32</span></span>|<span data-ttu-id="33eba-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-159">Not yet documented</span></span>|
|<span data-ttu-id="33eba-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="33eba-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="33eba-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="33eba-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="33eba-162">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-162">Not yet documented.</span></span> <span data-ttu-id="33eba-163">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="33eba-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="33eba-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="33eba-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="33eba-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="33eba-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="33eba-166">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-166">Not yet documented.</span></span> <span data-ttu-id="33eba-167">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="33eba-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="33eba-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="33eba-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="33eba-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="33eba-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="33eba-170">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-170">Not yet documented.</span></span> <span data-ttu-id="33eba-171">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="33eba-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="33eba-172">state</span><span class="sxs-lookup"><span data-stu-id="33eba-172">state</span></span>|[<span data-ttu-id="33eba-173">有効化</span><span class="sxs-lookup"><span data-stu-id="33eba-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="33eba-174">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-174">Not yet documented.</span></span> <span data-ttu-id="33eba-175">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="33eba-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="33eba-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="33eba-176">securityDeviceRequired</span></span>|<span data-ttu-id="33eba-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="33eba-177">Boolean</span></span>|<span data-ttu-id="33eba-178">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-178">Not yet documented</span></span>|
|<span data-ttu-id="33eba-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="33eba-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="33eba-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="33eba-180">Boolean</span></span>|<span data-ttu-id="33eba-181">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-181">Not yet documented</span></span>|
|<span data-ttu-id="33eba-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="33eba-182">remotePassportEnabled</span></span>|<span data-ttu-id="33eba-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="33eba-183">Boolean</span></span>|<span data-ttu-id="33eba-184">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-184">Not yet documented</span></span>|
|<span data-ttu-id="33eba-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="33eba-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="33eba-186">Int32</span><span class="sxs-lookup"><span data-stu-id="33eba-186">Int32</span></span>|<span data-ttu-id="33eba-187">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-187">Not yet documented</span></span>|
|<span data-ttu-id="33eba-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="33eba-188">pinExpirationInDays</span></span>|<span data-ttu-id="33eba-189">Int32</span><span class="sxs-lookup"><span data-stu-id="33eba-189">Int32</span></span>|<span data-ttu-id="33eba-190">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33eba-190">Not yet documented</span></span>|
|<span data-ttu-id="33eba-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="33eba-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="33eba-192">有効化</span><span class="sxs-lookup"><span data-stu-id="33eba-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="33eba-193">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="33eba-193">Not yet documented.</span></span> <span data-ttu-id="33eba-194">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="33eba-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="33eba-195">応答</span><span class="sxs-lookup"><span data-stu-id="33eba-195">Response</span></span>
<span data-ttu-id="33eba-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33eba-196">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33eba-197">例</span><span class="sxs-lookup"><span data-stu-id="33eba-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="33eba-198">要求</span><span class="sxs-lookup"><span data-stu-id="33eba-198">Request</span></span>
<span data-ttu-id="33eba-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33eba-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="33eba-200">応答</span><span class="sxs-lookup"><span data-stu-id="33eba-200">Response</span></span>
<span data-ttu-id="33eba-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33eba-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




