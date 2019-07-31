---
title: deviceEnrollmentLimitConfiguration の更新
description: deviceEnrollmentLimitConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 806452c46f6a9c01c8fa418a55e19b5bb0040fc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994083"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="77a5b-103">deviceEnrollmentLimitConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="77a5b-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="77a5b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77a5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77a5b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77a5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77a5b-106">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="77a5b-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77a5b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="77a5b-107">Prerequisites</span></span>
<span data-ttu-id="77a5b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77a5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a5b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77a5b-110">Permission type</span></span>|<span data-ttu-id="77a5b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="77a5b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77a5b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77a5b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77a5b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a5b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77a5b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77a5b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77a5b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77a5b-115">Not supported.</span></span>|
|<span data-ttu-id="77a5b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77a5b-116">Application</span></span>|<span data-ttu-id="77a5b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77a5b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77a5b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77a5b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="77a5b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77a5b-119">Request headers</span></span>
|<span data-ttu-id="77a5b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77a5b-120">Header</span></span>|<span data-ttu-id="77a5b-121">値</span><span class="sxs-lookup"><span data-stu-id="77a5b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77a5b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a5b-122">Authorization</span></span>|<span data-ttu-id="77a5b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="77a5b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77a5b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="77a5b-124">Accept</span></span>|<span data-ttu-id="77a5b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77a5b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77a5b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77a5b-126">Request body</span></span>
<span data-ttu-id="77a5b-127">要求本文で、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77a5b-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="77a5b-128">次の表に、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="77a5b-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="77a5b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77a5b-129">Property</span></span>|<span data-ttu-id="77a5b-130">型</span><span class="sxs-lookup"><span data-stu-id="77a5b-130">Type</span></span>|<span data-ttu-id="77a5b-131">説明</span><span class="sxs-lookup"><span data-stu-id="77a5b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77a5b-132">id</span><span class="sxs-lookup"><span data-stu-id="77a5b-132">id</span></span>|<span data-ttu-id="77a5b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="77a5b-133">String</span></span>|<span data-ttu-id="77a5b-134">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="77a5b-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="77a5b-135">displayName</span></span>|<span data-ttu-id="77a5b-136">String</span><span class="sxs-lookup"><span data-stu-id="77a5b-136">String</span></span>|<span data-ttu-id="77a5b-137">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="77a5b-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-138">description</span><span class="sxs-lookup"><span data-stu-id="77a5b-138">description</span></span>|<span data-ttu-id="77a5b-139">String</span><span class="sxs-lookup"><span data-stu-id="77a5b-139">String</span></span>|<span data-ttu-id="77a5b-140">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="77a5b-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-141">priority</span><span class="sxs-lookup"><span data-stu-id="77a5b-141">priority</span></span>|<span data-ttu-id="77a5b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="77a5b-142">Int32</span></span>|<span data-ttu-id="77a5b-143">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="77a5b-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="77a5b-144">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="77a5b-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="77a5b-145">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="77a5b-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77a5b-146">createdDateTime</span></span>|<span data-ttu-id="77a5b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a5b-147">DateTimeOffset</span></span>|<span data-ttu-id="77a5b-148">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="77a5b-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77a5b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="77a5b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77a5b-150">DateTimeOffset</span></span>|<span data-ttu-id="77a5b-151">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="77a5b-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-152">version</span><span class="sxs-lookup"><span data-stu-id="77a5b-152">version</span></span>|<span data-ttu-id="77a5b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="77a5b-153">Int32</span></span>|<span data-ttu-id="77a5b-154">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="77a5b-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="77a5b-155">limit</span><span class="sxs-lookup"><span data-stu-id="77a5b-155">limit</span></span>|<span data-ttu-id="77a5b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="77a5b-156">Int32</span></span>|<span data-ttu-id="77a5b-157">ユーザーが登録できるデバイスの最大数</span><span class="sxs-lookup"><span data-stu-id="77a5b-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="77a5b-158">応答</span><span class="sxs-lookup"><span data-stu-id="77a5b-158">Response</span></span>
<span data-ttu-id="77a5b-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77a5b-159">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77a5b-160">例</span><span class="sxs-lookup"><span data-stu-id="77a5b-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="77a5b-161">要求</span><span class="sxs-lookup"><span data-stu-id="77a5b-161">Request</span></span>
<span data-ttu-id="77a5b-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77a5b-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="77a5b-163">応答</span><span class="sxs-lookup"><span data-stu-id="77a5b-163">Response</span></span>
<span data-ttu-id="77a5b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77a5b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```





