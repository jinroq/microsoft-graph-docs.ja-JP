---
title: deviceEnrollmentLimitConfiguration の作成
description: 新しい deviceEnrollmentLimitConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc7ab67dc44eec17a6e7a516967d3f3b0bc644ae
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401132"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ffe71-103">deviceEnrollmentLimitConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="ffe71-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="ffe71-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ffe71-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ffe71-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffe71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffe71-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffe71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffe71-107">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ffe71-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffe71-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ffe71-108">Prerequisites</span></span>
<span data-ttu-id="ffe71-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffe71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ffe71-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffe71-111">Permission type</span></span>|<span data-ttu-id="ffe71-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffe71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffe71-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffe71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffe71-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe71-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ffe71-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffe71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffe71-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffe71-116">Not supported.</span></span>|
|<span data-ttu-id="ffe71-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffe71-117">Application</span></span>|<span data-ttu-id="ffe71-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffe71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffe71-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffe71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ffe71-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffe71-120">Request headers</span></span>
|<span data-ttu-id="ffe71-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffe71-121">Header</span></span>|<span data-ttu-id="ffe71-122">値</span><span class="sxs-lookup"><span data-stu-id="ffe71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffe71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffe71-123">Authorization</span></span>|<span data-ttu-id="ffe71-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ffe71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffe71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffe71-125">Accept</span></span>|<span data-ttu-id="ffe71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffe71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffe71-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffe71-127">Request body</span></span>
<span data-ttu-id="ffe71-128">要求本文で、deviceEnrollmentLimitConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ffe71-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="ffe71-129">次の表に、deviceEnrollmentLimitConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ffe71-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="ffe71-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffe71-130">Property</span></span>|<span data-ttu-id="ffe71-131">型</span><span class="sxs-lookup"><span data-stu-id="ffe71-131">Type</span></span>|<span data-ttu-id="ffe71-132">説明</span><span class="sxs-lookup"><span data-stu-id="ffe71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe71-133">id</span><span class="sxs-lookup"><span data-stu-id="ffe71-133">id</span></span>|<span data-ttu-id="ffe71-134">String</span><span class="sxs-lookup"><span data-stu-id="ffe71-134">String</span></span>|<span data-ttu-id="ffe71-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ffe71-136">displayName</span></span>|<span data-ttu-id="ffe71-137">String</span><span class="sxs-lookup"><span data-stu-id="ffe71-137">String</span></span>|<span data-ttu-id="ffe71-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-139">説明</span><span class="sxs-lookup"><span data-stu-id="ffe71-139">description</span></span>|<span data-ttu-id="ffe71-140">String</span><span class="sxs-lookup"><span data-stu-id="ffe71-140">String</span></span>|<span data-ttu-id="ffe71-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-142">priority</span><span class="sxs-lookup"><span data-stu-id="ffe71-142">priority</span></span>|<span data-ttu-id="ffe71-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe71-143">Int32</span></span>|<span data-ttu-id="ffe71-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffe71-145">createdDateTime</span></span>|<span data-ttu-id="ffe71-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe71-146">DateTimeOffset</span></span>|<span data-ttu-id="ffe71-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffe71-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ffe71-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe71-149">DateTimeOffset</span></span>|<span data-ttu-id="ffe71-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-151">version</span><span class="sxs-lookup"><span data-stu-id="ffe71-151">version</span></span>|<span data-ttu-id="ffe71-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe71-152">Int32</span></span>|<span data-ttu-id="ffe71-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffe71-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffe71-154">limit</span><span class="sxs-lookup"><span data-stu-id="ffe71-154">limit</span></span>|<span data-ttu-id="ffe71-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe71-155">Int32</span></span>|<span data-ttu-id="ffe71-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ffe71-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ffe71-157">応答</span><span class="sxs-lookup"><span data-stu-id="ffe71-157">Response</span></span>
<span data-ttu-id="ffe71-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffe71-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffe71-159">例</span><span class="sxs-lookup"><span data-stu-id="ffe71-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffe71-160">要求</span><span class="sxs-lookup"><span data-stu-id="ffe71-160">Request</span></span>
<span data-ttu-id="ffe71-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffe71-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="ffe71-162">応答</span><span class="sxs-lookup"><span data-stu-id="ffe71-162">Response</span></span>
<span data-ttu-id="ffe71-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ffe71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




