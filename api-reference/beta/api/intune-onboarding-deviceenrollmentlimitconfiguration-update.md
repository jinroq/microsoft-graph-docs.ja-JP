---
title: deviceEnrollmentLimitConfiguration の更新
description: deviceEnrollmentLimitConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 2d285ad19e907e40494c5ff7da9e112be3a20112
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329513"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ac9ed-103">deviceEnrollmentLimitConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ac9ed-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="ac9ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac9ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac9ed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac9ed-107">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac9ed-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ac9ed-108">Prerequisites</span></span>
<span data-ttu-id="ac9ed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac9ed-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac9ed-111">Permission type</span></span>|<span data-ttu-id="ac9ed-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac9ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac9ed-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac9ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac9ed-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac9ed-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac9ed-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac9ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac9ed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-116">Not supported.</span></span>|
|<span data-ttu-id="ac9ed-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac9ed-117">Application</span></span>|<span data-ttu-id="ac9ed-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac9ed-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac9ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ac9ed-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac9ed-120">Request headers</span></span>
|<span data-ttu-id="ac9ed-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac9ed-121">Header</span></span>|<span data-ttu-id="ac9ed-122">値</span><span class="sxs-lookup"><span data-stu-id="ac9ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac9ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac9ed-123">Authorization</span></span>|<span data-ttu-id="ac9ed-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac9ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac9ed-125">Accept</span></span>|<span data-ttu-id="ac9ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac9ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac9ed-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac9ed-127">Request body</span></span>
<span data-ttu-id="ac9ed-128">要求本文で、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="ac9ed-129">次の表に、[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="ac9ed-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac9ed-130">Property</span></span>|<span data-ttu-id="ac9ed-131">種類</span><span class="sxs-lookup"><span data-stu-id="ac9ed-131">Type</span></span>|<span data-ttu-id="ac9ed-132">説明</span><span class="sxs-lookup"><span data-stu-id="ac9ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac9ed-133">ID</span><span class="sxs-lookup"><span data-stu-id="ac9ed-133">id</span></span>|<span data-ttu-id="ac9ed-134">String</span><span class="sxs-lookup"><span data-stu-id="ac9ed-134">String</span></span>|<span data-ttu-id="ac9ed-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ac9ed-136">displayName</span></span>|<span data-ttu-id="ac9ed-137">String</span><span class="sxs-lookup"><span data-stu-id="ac9ed-137">String</span></span>|<span data-ttu-id="ac9ed-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-139">説明</span><span class="sxs-lookup"><span data-stu-id="ac9ed-139">description</span></span>|<span data-ttu-id="ac9ed-140">String</span><span class="sxs-lookup"><span data-stu-id="ac9ed-140">String</span></span>|<span data-ttu-id="ac9ed-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-142">priority</span><span class="sxs-lookup"><span data-stu-id="ac9ed-142">priority</span></span>|<span data-ttu-id="ac9ed-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9ed-143">Int32</span></span>|<span data-ttu-id="ac9ed-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac9ed-145">createdDateTime</span></span>|<span data-ttu-id="ac9ed-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac9ed-146">DateTimeOffset</span></span>|<span data-ttu-id="ac9ed-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac9ed-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ac9ed-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac9ed-149">DateTimeOffset</span></span>|<span data-ttu-id="ac9ed-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-151">version</span><span class="sxs-lookup"><span data-stu-id="ac9ed-151">version</span></span>|<span data-ttu-id="ac9ed-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9ed-152">Int32</span></span>|<span data-ttu-id="ac9ed-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac9ed-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ed-154">limit</span><span class="sxs-lookup"><span data-stu-id="ac9ed-154">limit</span></span>|<span data-ttu-id="ac9ed-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9ed-155">Int32</span></span>|<span data-ttu-id="ac9ed-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ac9ed-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ac9ed-157">応答</span><span class="sxs-lookup"><span data-stu-id="ac9ed-157">Response</span></span>
<span data-ttu-id="ac9ed-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac9ed-159">例</span><span class="sxs-lookup"><span data-stu-id="ac9ed-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac9ed-160">要求</span><span class="sxs-lookup"><span data-stu-id="ac9ed-160">Request</span></span>
<span data-ttu-id="ac9ed-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="ac9ed-162">応答</span><span class="sxs-lookup"><span data-stu-id="ac9ed-162">Response</span></span>
<span data-ttu-id="ac9ed-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac9ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




