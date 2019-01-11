---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の作成
description: 新しい deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd395803e5940855c3eb21e5ca1ca8b8b1ec3bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829492"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="7ae7b-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="7ae7b-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="7ae7b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ae7b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ae7b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ae7b-107">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-107">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ae7b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7ae7b-108">Prerequisites</span></span>
<span data-ttu-id="7ae7b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ae7b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ae7b-111">Permission type</span></span>|<span data-ttu-id="7ae7b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ae7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ae7b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ae7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ae7b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ae7b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ae7b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ae7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ae7b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-116">Not supported.</span></span>|
|<span data-ttu-id="7ae7b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ae7b-117">Application</span></span>|<span data-ttu-id="7ae7b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ae7b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ae7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ae7b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ae7b-120">Request headers</span></span>
|<span data-ttu-id="7ae7b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ae7b-121">Header</span></span>|<span data-ttu-id="7ae7b-122">値</span><span class="sxs-lookup"><span data-stu-id="7ae7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ae7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ae7b-123">Authorization</span></span>|<span data-ttu-id="7ae7b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ae7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ae7b-125">Accept</span></span>|<span data-ttu-id="7ae7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ae7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ae7b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ae7b-127">Request body</span></span>
<span data-ttu-id="7ae7b-128">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-128">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="7ae7b-129">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-129">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="7ae7b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ae7b-130">Property</span></span>|<span data-ttu-id="7ae7b-131">種類</span><span class="sxs-lookup"><span data-stu-id="7ae7b-131">Type</span></span>|<span data-ttu-id="7ae7b-132">説明</span><span class="sxs-lookup"><span data-stu-id="7ae7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ae7b-133">ID</span><span class="sxs-lookup"><span data-stu-id="7ae7b-133">id</span></span>|<span data-ttu-id="7ae7b-134">String</span><span class="sxs-lookup"><span data-stu-id="7ae7b-134">String</span></span>|<span data-ttu-id="7ae7b-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ae7b-136">displayName</span></span>|<span data-ttu-id="7ae7b-137">String</span><span class="sxs-lookup"><span data-stu-id="7ae7b-137">String</span></span>|<span data-ttu-id="7ae7b-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-139">説明</span><span class="sxs-lookup"><span data-stu-id="7ae7b-139">description</span></span>|<span data-ttu-id="7ae7b-140">String</span><span class="sxs-lookup"><span data-stu-id="7ae7b-140">String</span></span>|<span data-ttu-id="7ae7b-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-142">priority</span><span class="sxs-lookup"><span data-stu-id="7ae7b-142">priority</span></span>|<span data-ttu-id="7ae7b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7ae7b-143">Int32</span></span>|<span data-ttu-id="7ae7b-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ae7b-145">createdDateTime</span></span>|<span data-ttu-id="7ae7b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ae7b-146">DateTimeOffset</span></span>|<span data-ttu-id="7ae7b-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ae7b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7ae7b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ae7b-149">DateTimeOffset</span></span>|<span data-ttu-id="7ae7b-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-151">version</span><span class="sxs-lookup"><span data-stu-id="7ae7b-151">version</span></span>|<span data-ttu-id="7ae7b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7ae7b-152">Int32</span></span>|<span data-ttu-id="7ae7b-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7ae7b-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7ae7b-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7ae7b-154">pinMinimumLength</span></span>|<span data-ttu-id="7ae7b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="7ae7b-155">Int32</span></span>|<span data-ttu-id="7ae7b-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-156">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="7ae7b-157">pinMaximumLength</span></span>|<span data-ttu-id="7ae7b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7ae7b-158">Int32</span></span>|<span data-ttu-id="7ae7b-159">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-159">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="7ae7b-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="7ae7b-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="7ae7b-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="7ae7b-162">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-162">Not yet documented.</span></span> <span data-ttu-id="7ae7b-163">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="7ae7b-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="7ae7b-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="7ae7b-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="7ae7b-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="7ae7b-166">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-166">Not yet documented.</span></span> <span data-ttu-id="7ae7b-167">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="7ae7b-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="7ae7b-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="7ae7b-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="7ae7b-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="7ae7b-170">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-170">Not yet documented.</span></span> <span data-ttu-id="7ae7b-171">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="7ae7b-172">state</span><span class="sxs-lookup"><span data-stu-id="7ae7b-172">state</span></span>|[<span data-ttu-id="7ae7b-173">有効化</span><span class="sxs-lookup"><span data-stu-id="7ae7b-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ae7b-174">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-174">Not yet documented.</span></span> <span data-ttu-id="7ae7b-175">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7ae7b-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="7ae7b-176">securityDeviceRequired</span></span>|<span data-ttu-id="7ae7b-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ae7b-177">Boolean</span></span>|<span data-ttu-id="7ae7b-178">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-178">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="7ae7b-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="7ae7b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ae7b-180">Boolean</span></span>|<span data-ttu-id="7ae7b-181">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-181">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="7ae7b-182">remotePassportEnabled</span></span>|<span data-ttu-id="7ae7b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ae7b-183">Boolean</span></span>|<span data-ttu-id="7ae7b-184">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-184">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="7ae7b-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="7ae7b-186">Int32</span><span class="sxs-lookup"><span data-stu-id="7ae7b-186">Int32</span></span>|<span data-ttu-id="7ae7b-187">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-187">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="7ae7b-188">pinExpirationInDays</span></span>|<span data-ttu-id="7ae7b-189">Int32</span><span class="sxs-lookup"><span data-stu-id="7ae7b-189">Int32</span></span>|<span data-ttu-id="7ae7b-190">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7ae7b-190">Not yet documented</span></span>|
|<span data-ttu-id="7ae7b-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="7ae7b-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="7ae7b-192">有効化</span><span class="sxs-lookup"><span data-stu-id="7ae7b-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7ae7b-193">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-193">Not yet documented.</span></span> <span data-ttu-id="7ae7b-194">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ae7b-195">応答</span><span class="sxs-lookup"><span data-stu-id="7ae7b-195">Response</span></span>
<span data-ttu-id="7ae7b-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-196">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ae7b-197">例</span><span class="sxs-lookup"><span data-stu-id="7ae7b-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ae7b-198">要求</span><span class="sxs-lookup"><span data-stu-id="7ae7b-198">Request</span></span>
<span data-ttu-id="7ae7b-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 693

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
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

### <a name="response"></a><span data-ttu-id="7ae7b-200">応答</span><span class="sxs-lookup"><span data-stu-id="7ae7b-200">Response</span></span>
<span data-ttu-id="7ae7b-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ae7b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





