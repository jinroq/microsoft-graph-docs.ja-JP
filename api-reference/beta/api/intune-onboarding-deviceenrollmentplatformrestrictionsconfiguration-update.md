---
title: deviceEnrollmentPlatformRestrictionsConfiguration の更新
description: deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 880cbd1f25b7f596e6de193c9fcd3a69b10ba392
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981175"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="d8be9-103">deviceEnrollmentPlatformRestrictionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d8be9-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="d8be9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8be9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8be9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8be9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8be9-106">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d8be9-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8be9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8be9-107">Prerequisites</span></span>
<span data-ttu-id="d8be9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8be9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8be9-110">Permission type</span></span>|<span data-ttu-id="d8be9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8be9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8be9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8be9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8be9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8be9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8be9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8be9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8be9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8be9-115">Not supported.</span></span>|
|<span data-ttu-id="d8be9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8be9-116">Application</span></span>|<span data-ttu-id="d8be9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8be9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8be9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8be9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8be9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8be9-119">Request headers</span></span>
|<span data-ttu-id="d8be9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8be9-120">Header</span></span>|<span data-ttu-id="d8be9-121">値</span><span class="sxs-lookup"><span data-stu-id="d8be9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8be9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8be9-122">Authorization</span></span>|<span data-ttu-id="d8be9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8be9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8be9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d8be9-124">Accept</span></span>|<span data-ttu-id="d8be9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8be9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8be9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8be9-126">Request body</span></span>
<span data-ttu-id="d8be9-127">要求本文で、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8be9-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="d8be9-128">次の表に、[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d8be9-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="d8be9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8be9-129">Property</span></span>|<span data-ttu-id="d8be9-130">型</span><span class="sxs-lookup"><span data-stu-id="d8be9-130">Type</span></span>|<span data-ttu-id="d8be9-131">説明</span><span class="sxs-lookup"><span data-stu-id="d8be9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8be9-132">id</span><span class="sxs-lookup"><span data-stu-id="d8be9-132">id</span></span>|<span data-ttu-id="d8be9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d8be9-133">String</span></span>|<span data-ttu-id="d8be9-134">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="d8be9-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d8be9-135">displayName</span></span>|<span data-ttu-id="d8be9-136">String</span><span class="sxs-lookup"><span data-stu-id="d8be9-136">String</span></span>|<span data-ttu-id="d8be9-137">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="d8be9-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-138">description</span><span class="sxs-lookup"><span data-stu-id="d8be9-138">description</span></span>|<span data-ttu-id="d8be9-139">String</span><span class="sxs-lookup"><span data-stu-id="d8be9-139">String</span></span>|<span data-ttu-id="d8be9-140">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="d8be9-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-141">priority</span><span class="sxs-lookup"><span data-stu-id="d8be9-141">priority</span></span>|<span data-ttu-id="d8be9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d8be9-142">Int32</span></span>|<span data-ttu-id="d8be9-143">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8be9-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d8be9-144">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="d8be9-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="d8be9-145">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d8be9-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8be9-146">createdDateTime</span></span>|<span data-ttu-id="d8be9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8be9-147">DateTimeOffset</span></span>|<span data-ttu-id="d8be9-148">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="d8be9-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8be9-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d8be9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8be9-150">DateTimeOffset</span></span>|<span data-ttu-id="d8be9-151">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="d8be9-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-152">version</span><span class="sxs-lookup"><span data-stu-id="d8be9-152">version</span></span>|<span data-ttu-id="d8be9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d8be9-153">Int32</span></span>|<span data-ttu-id="d8be9-154">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="d8be9-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8be9-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-155">iosRestriction</span></span>|[<span data-ttu-id="d8be9-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-157">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Ios の制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="d8be9-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-158">windowsRestriction</span></span>|[<span data-ttu-id="d8be9-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-160">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows の制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="d8be9-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="d8be9-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-163">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows mobile の制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="d8be9-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-164">androidRestriction</span></span>|[<span data-ttu-id="d8be9-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-166">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Android の制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="d8be9-167">Androidforwork 制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="d8be9-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-169">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づいた、Android for work 制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="d8be9-170">macRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-170">macRestriction</span></span>|[<span data-ttu-id="d8be9-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-172">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="d8be9-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-173">macOSRestriction</span></span>|[<span data-ttu-id="d8be9-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d8be9-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d8be9-175">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="d8be9-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="d8be9-176">応答</span><span class="sxs-lookup"><span data-stu-id="d8be9-176">Response</span></span>
<span data-ttu-id="d8be9-177">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d8be9-177">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8be9-178">例</span><span class="sxs-lookup"><span data-stu-id="d8be9-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8be9-179">要求</span><span class="sxs-lookup"><span data-stu-id="d8be9-179">Request</span></span>
<span data-ttu-id="d8be9-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8be9-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="d8be9-181">応答</span><span class="sxs-lookup"><span data-stu-id="d8be9-181">Response</span></span>
<span data-ttu-id="d8be9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8be9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2403

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```





