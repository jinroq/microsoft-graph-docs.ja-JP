---
title: deviceEnrollmentLimitConfiguration の更新
description: deviceEnrollmentLimitConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 842c9d6c1cf6e805850317bb804cb8905c189134
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254178"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="b3893-103">deviceEnrollmentLimitConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="b3893-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="b3893-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3893-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3893-105">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b3893-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3893-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3893-106">Prerequisites</span></span>
<span data-ttu-id="b3893-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3893-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3893-109">Permission type</span></span>|<span data-ttu-id="b3893-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3893-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3893-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3893-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3893-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3893-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3893-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3893-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3893-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3893-114">Not supported.</span></span>|
|<span data-ttu-id="b3893-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3893-115">Application</span></span>|<span data-ttu-id="b3893-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3893-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3893-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3893-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3893-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3893-118">Request headers</span></span>
|<span data-ttu-id="b3893-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3893-119">Header</span></span>|<span data-ttu-id="b3893-120">値</span><span class="sxs-lookup"><span data-stu-id="b3893-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3893-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3893-121">Authorization</span></span>|<span data-ttu-id="b3893-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3893-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3893-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b3893-123">Accept</span></span>|<span data-ttu-id="b3893-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3893-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3893-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3893-125">Request body</span></span>
<span data-ttu-id="b3893-126">要求本文で、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3893-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="b3893-127">次の表に、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b3893-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="b3893-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3893-128">Property</span></span>|<span data-ttu-id="b3893-129">型</span><span class="sxs-lookup"><span data-stu-id="b3893-129">Type</span></span>|<span data-ttu-id="b3893-130">説明</span><span class="sxs-lookup"><span data-stu-id="b3893-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3893-131">id</span><span class="sxs-lookup"><span data-stu-id="b3893-131">id</span></span>|<span data-ttu-id="b3893-132">String</span><span class="sxs-lookup"><span data-stu-id="b3893-132">String</span></span>|<span data-ttu-id="b3893-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b3893-134">displayName</span></span>|<span data-ttu-id="b3893-135">String</span><span class="sxs-lookup"><span data-stu-id="b3893-135">String</span></span>|<span data-ttu-id="b3893-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-137">説明</span><span class="sxs-lookup"><span data-stu-id="b3893-137">description</span></span>|<span data-ttu-id="b3893-138">String</span><span class="sxs-lookup"><span data-stu-id="b3893-138">String</span></span>|<span data-ttu-id="b3893-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-140">priority</span><span class="sxs-lookup"><span data-stu-id="b3893-140">priority</span></span>|<span data-ttu-id="b3893-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b3893-141">Int32</span></span>|<span data-ttu-id="b3893-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3893-143">createdDateTime</span></span>|<span data-ttu-id="b3893-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3893-144">DateTimeOffset</span></span>|<span data-ttu-id="b3893-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3893-146">lastModifiedDateTime</span></span>|<span data-ttu-id="b3893-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3893-147">DateTimeOffset</span></span>|<span data-ttu-id="b3893-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-149">version</span><span class="sxs-lookup"><span data-stu-id="b3893-149">version</span></span>|<span data-ttu-id="b3893-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b3893-150">Int32</span></span>|<span data-ttu-id="b3893-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b3893-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b3893-152">limit</span><span class="sxs-lookup"><span data-stu-id="b3893-152">limit</span></span>|<span data-ttu-id="b3893-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b3893-153">Int32</span></span>|<span data-ttu-id="b3893-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3893-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3893-155">応答</span><span class="sxs-lookup"><span data-stu-id="b3893-155">Response</span></span>
<span data-ttu-id="b3893-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b3893-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3893-157">例</span><span class="sxs-lookup"><span data-stu-id="b3893-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3893-158">要求</span><span class="sxs-lookup"><span data-stu-id="b3893-158">Request</span></span>
<span data-ttu-id="b3893-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3893-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="b3893-160">応答</span><span class="sxs-lookup"><span data-stu-id="b3893-160">Response</span></span>
<span data-ttu-id="b3893-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3893-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



