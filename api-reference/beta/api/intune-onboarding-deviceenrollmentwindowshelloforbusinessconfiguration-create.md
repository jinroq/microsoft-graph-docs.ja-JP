---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の作成
description: 新しい deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4db61460a7855e11f6c8fb51aa2656f25c10547e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151346"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="353d6-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="353d6-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="353d6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="353d6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="353d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="353d6-106">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="353d6-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="353d6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="353d6-107">Prerequisites</span></span>
<span data-ttu-id="353d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="353d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="353d6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="353d6-110">Permission type</span></span>|<span data-ttu-id="353d6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="353d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="353d6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="353d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="353d6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="353d6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="353d6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="353d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="353d6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-115">Not supported.</span></span>|
|<span data-ttu-id="353d6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="353d6-116">Application</span></span>|<span data-ttu-id="353d6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="353d6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="353d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="353d6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="353d6-119">Request headers</span></span>
|<span data-ttu-id="353d6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="353d6-120">Header</span></span>|<span data-ttu-id="353d6-121">値</span><span class="sxs-lookup"><span data-stu-id="353d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="353d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="353d6-122">Authorization</span></span>|<span data-ttu-id="353d6-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="353d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="353d6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="353d6-124">Accept</span></span>|<span data-ttu-id="353d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="353d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="353d6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="353d6-126">Request body</span></span>
<span data-ttu-id="353d6-127">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="353d6-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="353d6-128">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="353d6-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="353d6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="353d6-129">Property</span></span>|<span data-ttu-id="353d6-130">型</span><span class="sxs-lookup"><span data-stu-id="353d6-130">Type</span></span>|<span data-ttu-id="353d6-131">説明</span><span class="sxs-lookup"><span data-stu-id="353d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="353d6-132">id</span><span class="sxs-lookup"><span data-stu-id="353d6-132">id</span></span>|<span data-ttu-id="353d6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="353d6-133">String</span></span>|<span data-ttu-id="353d6-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="353d6-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="353d6-135">displayName</span></span>|<span data-ttu-id="353d6-136">String</span><span class="sxs-lookup"><span data-stu-id="353d6-136">String</span></span>|<span data-ttu-id="353d6-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="353d6-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-138">説明</span><span class="sxs-lookup"><span data-stu-id="353d6-138">description</span></span>|<span data-ttu-id="353d6-139">String</span><span class="sxs-lookup"><span data-stu-id="353d6-139">String</span></span>|<span data-ttu-id="353d6-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="353d6-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-141">priority</span><span class="sxs-lookup"><span data-stu-id="353d6-141">priority</span></span>|<span data-ttu-id="353d6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="353d6-142">Int32</span></span>|<span data-ttu-id="353d6-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="353d6-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="353d6-144">createdDateTime</span></span>|<span data-ttu-id="353d6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="353d6-145">DateTimeOffset</span></span>|<span data-ttu-id="353d6-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="353d6-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="353d6-147">lastModifiedDateTime</span></span>|<span data-ttu-id="353d6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="353d6-148">DateTimeOffset</span></span>|<span data-ttu-id="353d6-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="353d6-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-150">version</span><span class="sxs-lookup"><span data-stu-id="353d6-150">version</span></span>|<span data-ttu-id="353d6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="353d6-151">Int32</span></span>|<span data-ttu-id="353d6-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="353d6-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="353d6-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="353d6-153">pinMinimumLength</span></span>|<span data-ttu-id="353d6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="353d6-154">Int32</span></span>|<span data-ttu-id="353d6-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-155">Not yet documented</span></span>|
|<span data-ttu-id="353d6-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="353d6-156">pinMaximumLength</span></span>|<span data-ttu-id="353d6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="353d6-157">Int32</span></span>|<span data-ttu-id="353d6-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-158">Not yet documented</span></span>|
|<span data-ttu-id="353d6-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="353d6-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="353d6-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="353d6-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="353d6-161">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-161">Not yet documented.</span></span> <span data-ttu-id="353d6-162">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="353d6-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="353d6-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="353d6-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="353d6-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="353d6-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="353d6-165">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-165">Not yet documented.</span></span> <span data-ttu-id="353d6-166">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="353d6-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="353d6-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="353d6-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="353d6-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="353d6-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="353d6-169">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-169">Not yet documented.</span></span> <span data-ttu-id="353d6-170">可能な値は `allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="353d6-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="353d6-171">state</span><span class="sxs-lookup"><span data-stu-id="353d6-171">state</span></span>|[<span data-ttu-id="353d6-172">購入</span><span class="sxs-lookup"><span data-stu-id="353d6-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="353d6-173">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-173">Not yet documented.</span></span> <span data-ttu-id="353d6-174">可能な値は `notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="353d6-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="353d6-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="353d6-175">securityDeviceRequired</span></span>|<span data-ttu-id="353d6-176">ブール値</span><span class="sxs-lookup"><span data-stu-id="353d6-176">Boolean</span></span>|<span data-ttu-id="353d6-177">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-177">Not yet documented</span></span>|
|<span data-ttu-id="353d6-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="353d6-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="353d6-179">ブール値</span><span class="sxs-lookup"><span data-stu-id="353d6-179">Boolean</span></span>|<span data-ttu-id="353d6-180">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-180">Not yet documented</span></span>|
|<span data-ttu-id="353d6-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="353d6-181">remotePassportEnabled</span></span>|<span data-ttu-id="353d6-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="353d6-182">Boolean</span></span>|<span data-ttu-id="353d6-183">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-183">Not yet documented</span></span>|
|<span data-ttu-id="353d6-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="353d6-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="353d6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="353d6-185">Int32</span></span>|<span data-ttu-id="353d6-186">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-186">Not yet documented</span></span>|
|<span data-ttu-id="353d6-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="353d6-187">pinExpirationInDays</span></span>|<span data-ttu-id="353d6-188">Int32</span><span class="sxs-lookup"><span data-stu-id="353d6-188">Int32</span></span>|<span data-ttu-id="353d6-189">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="353d6-189">Not yet documented</span></span>|
|<span data-ttu-id="353d6-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="353d6-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="353d6-191">購入</span><span class="sxs-lookup"><span data-stu-id="353d6-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="353d6-192">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="353d6-192">Not yet documented.</span></span> <span data-ttu-id="353d6-193">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="353d6-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="353d6-194">応答</span><span class="sxs-lookup"><span data-stu-id="353d6-194">Response</span></span>
<span data-ttu-id="353d6-195">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="353d6-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="353d6-196">例</span><span class="sxs-lookup"><span data-stu-id="353d6-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="353d6-197">要求</span><span class="sxs-lookup"><span data-stu-id="353d6-197">Request</span></span>
<span data-ttu-id="353d6-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="353d6-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="353d6-199">応答</span><span class="sxs-lookup"><span data-stu-id="353d6-199">Response</span></span>
<span data-ttu-id="353d6-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="353d6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




