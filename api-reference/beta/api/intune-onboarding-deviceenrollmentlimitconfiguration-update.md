---
title: deviceEnrollmentLimitConfiguration の更新
description: deviceEnrollmentLimitConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 775eba06cce66394f448f305d10f80ca9ec16822
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772357"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="80964-103">deviceEnrollmentLimitConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="80964-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="80964-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80964-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80964-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80964-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80964-106">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="80964-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80964-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="80964-107">Prerequisites</span></span>
<span data-ttu-id="80964-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80964-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80964-110">Permission type</span></span>|<span data-ttu-id="80964-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="80964-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80964-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80964-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80964-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80964-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80964-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80964-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80964-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80964-115">Not supported.</span></span>|
|<span data-ttu-id="80964-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80964-116">Application</span></span>|<span data-ttu-id="80964-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80964-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80964-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80964-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80964-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80964-119">Request headers</span></span>
|<span data-ttu-id="80964-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80964-120">Header</span></span>|<span data-ttu-id="80964-121">値</span><span class="sxs-lookup"><span data-stu-id="80964-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80964-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80964-122">Authorization</span></span>|<span data-ttu-id="80964-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="80964-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80964-124">承諾</span><span class="sxs-lookup"><span data-stu-id="80964-124">Accept</span></span>|<span data-ttu-id="80964-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80964-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80964-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="80964-126">Request body</span></span>
<span data-ttu-id="80964-127">要求本文で、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="80964-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="80964-128">次の表に、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="80964-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="80964-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80964-129">Property</span></span>|<span data-ttu-id="80964-130">型</span><span class="sxs-lookup"><span data-stu-id="80964-130">Type</span></span>|<span data-ttu-id="80964-131">説明</span><span class="sxs-lookup"><span data-stu-id="80964-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80964-132">id</span><span class="sxs-lookup"><span data-stu-id="80964-132">id</span></span>|<span data-ttu-id="80964-133">文字列</span><span class="sxs-lookup"><span data-stu-id="80964-133">String</span></span>|<span data-ttu-id="80964-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="80964-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-135">displayName</span><span class="sxs-lookup"><span data-stu-id="80964-135">displayName</span></span>|<span data-ttu-id="80964-136">String</span><span class="sxs-lookup"><span data-stu-id="80964-136">String</span></span>|<span data-ttu-id="80964-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80964-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-138">説明</span><span class="sxs-lookup"><span data-stu-id="80964-138">description</span></span>|<span data-ttu-id="80964-139">String</span><span class="sxs-lookup"><span data-stu-id="80964-139">String</span></span>|<span data-ttu-id="80964-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80964-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-141">priority</span><span class="sxs-lookup"><span data-stu-id="80964-141">priority</span></span>|<span data-ttu-id="80964-142">Int32</span><span class="sxs-lookup"><span data-stu-id="80964-142">Int32</span></span>|<span data-ttu-id="80964-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80964-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80964-144">createdDateTime</span></span>|<span data-ttu-id="80964-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80964-145">DateTimeOffset</span></span>|<span data-ttu-id="80964-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80964-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80964-147">lastModifiedDateTime</span></span>|<span data-ttu-id="80964-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80964-148">DateTimeOffset</span></span>|<span data-ttu-id="80964-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80964-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-150">version</span><span class="sxs-lookup"><span data-stu-id="80964-150">version</span></span>|<span data-ttu-id="80964-151">Int32</span><span class="sxs-lookup"><span data-stu-id="80964-151">Int32</span></span>|<span data-ttu-id="80964-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80964-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="80964-153">limit</span><span class="sxs-lookup"><span data-stu-id="80964-153">limit</span></span>|<span data-ttu-id="80964-154">Int32</span><span class="sxs-lookup"><span data-stu-id="80964-154">Int32</span></span>|<span data-ttu-id="80964-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="80964-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="80964-156">応答</span><span class="sxs-lookup"><span data-stu-id="80964-156">Response</span></span>
<span data-ttu-id="80964-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80964-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80964-158">例</span><span class="sxs-lookup"><span data-stu-id="80964-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="80964-159">要求</span><span class="sxs-lookup"><span data-stu-id="80964-159">Request</span></span>
<span data-ttu-id="80964-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80964-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80964-161">応答</span><span class="sxs-lookup"><span data-stu-id="80964-161">Response</span></span>
<span data-ttu-id="80964-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





