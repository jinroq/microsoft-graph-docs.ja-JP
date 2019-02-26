---
title: deviceEnrollmentLimitConfiguration の作成
description: 新しい deviceEnrollmentLimitConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d6773086a44205a3ddb2c5603e2a898c5bfab10
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262154"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="3bda5-103">deviceEnrollmentLimitConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="3bda5-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="3bda5-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3bda5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bda5-105">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3bda5-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bda5-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3bda5-106">Prerequisites</span></span>
<span data-ttu-id="3bda5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bda5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3bda5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bda5-109">Permission type</span></span>|<span data-ttu-id="3bda5-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bda5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bda5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bda5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3bda5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bda5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3bda5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bda5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bda5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bda5-114">Not supported.</span></span>|
|<span data-ttu-id="3bda5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bda5-115">Application</span></span>|<span data-ttu-id="3bda5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bda5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bda5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bda5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3bda5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bda5-118">Request headers</span></span>
|<span data-ttu-id="3bda5-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bda5-119">Header</span></span>|<span data-ttu-id="3bda5-120">値</span><span class="sxs-lookup"><span data-stu-id="3bda5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bda5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bda5-121">Authorization</span></span>|<span data-ttu-id="3bda5-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3bda5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bda5-123">承諾</span><span class="sxs-lookup"><span data-stu-id="3bda5-123">Accept</span></span>|<span data-ttu-id="3bda5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3bda5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bda5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bda5-125">Request body</span></span>
<span data-ttu-id="3bda5-126">要求本文で、deviceEnrollmentLimitConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bda5-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="3bda5-127">次の表に、deviceEnrollmentLimitConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3bda5-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="3bda5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bda5-128">Property</span></span>|<span data-ttu-id="3bda5-129">型</span><span class="sxs-lookup"><span data-stu-id="3bda5-129">Type</span></span>|<span data-ttu-id="3bda5-130">説明</span><span class="sxs-lookup"><span data-stu-id="3bda5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bda5-131">id</span><span class="sxs-lookup"><span data-stu-id="3bda5-131">id</span></span>|<span data-ttu-id="3bda5-132">String</span><span class="sxs-lookup"><span data-stu-id="3bda5-132">String</span></span>|<span data-ttu-id="3bda5-133">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3bda5-134">displayName</span></span>|<span data-ttu-id="3bda5-135">String</span><span class="sxs-lookup"><span data-stu-id="3bda5-135">String</span></span>|<span data-ttu-id="3bda5-136">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-137">説明</span><span class="sxs-lookup"><span data-stu-id="3bda5-137">description</span></span>|<span data-ttu-id="3bda5-138">String</span><span class="sxs-lookup"><span data-stu-id="3bda5-138">String</span></span>|<span data-ttu-id="3bda5-139">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-140">priority</span><span class="sxs-lookup"><span data-stu-id="3bda5-140">priority</span></span>|<span data-ttu-id="3bda5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3bda5-141">Int32</span></span>|<span data-ttu-id="3bda5-142">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bda5-143">createdDateTime</span></span>|<span data-ttu-id="3bda5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bda5-144">DateTimeOffset</span></span>|<span data-ttu-id="3bda5-145">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bda5-146">lastModifiedDateTime</span></span>|<span data-ttu-id="3bda5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bda5-147">DateTimeOffset</span></span>|<span data-ttu-id="3bda5-148">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-149">version</span><span class="sxs-lookup"><span data-stu-id="3bda5-149">version</span></span>|<span data-ttu-id="3bda5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3bda5-150">Int32</span></span>|<span data-ttu-id="3bda5-151">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3bda5-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3bda5-152">limit</span><span class="sxs-lookup"><span data-stu-id="3bda5-152">limit</span></span>|<span data-ttu-id="3bda5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3bda5-153">Int32</span></span>|<span data-ttu-id="3bda5-154">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3bda5-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3bda5-155">応答</span><span class="sxs-lookup"><span data-stu-id="3bda5-155">Response</span></span>
<span data-ttu-id="3bda5-156">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3bda5-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bda5-157">例</span><span class="sxs-lookup"><span data-stu-id="3bda5-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bda5-158">要求</span><span class="sxs-lookup"><span data-stu-id="3bda5-158">Request</span></span>
<span data-ttu-id="3bda5-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bda5-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="3bda5-160">応答</span><span class="sxs-lookup"><span data-stu-id="3bda5-160">Response</span></span>
<span data-ttu-id="3bda5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bda5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



