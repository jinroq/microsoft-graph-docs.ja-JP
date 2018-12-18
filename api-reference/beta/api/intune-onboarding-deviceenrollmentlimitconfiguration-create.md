---
title: deviceEnrollmentLimitConfiguration の作成
description: 新しい deviceEnrollmentLimitConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: fdb9fee09f43890280ef0beb79d6d57d9def67f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359669"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d38e6-103">deviceEnrollmentLimitConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="d38e6-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="d38e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d38e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d38e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d38e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d38e6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d38e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d38e6-107">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d38e6-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d38e6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d38e6-108">Prerequisites</span></span>
<span data-ttu-id="d38e6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d38e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38e6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d38e6-111">Permission type</span></span>|<span data-ttu-id="d38e6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d38e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d38e6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d38e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d38e6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d38e6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d38e6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d38e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d38e6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d38e6-116">Not supported.</span></span>|
|<span data-ttu-id="d38e6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d38e6-117">Application</span></span>|<span data-ttu-id="d38e6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d38e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d38e6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d38e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d38e6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d38e6-120">Request headers</span></span>
|<span data-ttu-id="d38e6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d38e6-121">Header</span></span>|<span data-ttu-id="d38e6-122">値</span><span class="sxs-lookup"><span data-stu-id="d38e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d38e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d38e6-123">Authorization</span></span>|<span data-ttu-id="d38e6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d38e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d38e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d38e6-125">Accept</span></span>|<span data-ttu-id="d38e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d38e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d38e6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d38e6-127">Request body</span></span>
<span data-ttu-id="d38e6-128">要求本文で、deviceEnrollmentLimitConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d38e6-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="d38e6-129">次の表に、deviceEnrollmentLimitConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d38e6-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="d38e6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d38e6-130">Property</span></span>|<span data-ttu-id="d38e6-131">種類</span><span class="sxs-lookup"><span data-stu-id="d38e6-131">Type</span></span>|<span data-ttu-id="d38e6-132">説明</span><span class="sxs-lookup"><span data-stu-id="d38e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d38e6-133">ID</span><span class="sxs-lookup"><span data-stu-id="d38e6-133">id</span></span>|<span data-ttu-id="d38e6-134">String</span><span class="sxs-lookup"><span data-stu-id="d38e6-134">String</span></span>|<span data-ttu-id="d38e6-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d38e6-136">displayName</span></span>|<span data-ttu-id="d38e6-137">String</span><span class="sxs-lookup"><span data-stu-id="d38e6-137">String</span></span>|<span data-ttu-id="d38e6-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-139">説明</span><span class="sxs-lookup"><span data-stu-id="d38e6-139">description</span></span>|<span data-ttu-id="d38e6-140">String</span><span class="sxs-lookup"><span data-stu-id="d38e6-140">String</span></span>|<span data-ttu-id="d38e6-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-142">priority</span><span class="sxs-lookup"><span data-stu-id="d38e6-142">priority</span></span>|<span data-ttu-id="d38e6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d38e6-143">Int32</span></span>|<span data-ttu-id="d38e6-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d38e6-145">createdDateTime</span></span>|<span data-ttu-id="d38e6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d38e6-146">DateTimeOffset</span></span>|<span data-ttu-id="d38e6-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d38e6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d38e6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d38e6-149">DateTimeOffset</span></span>|<span data-ttu-id="d38e6-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-151">version</span><span class="sxs-lookup"><span data-stu-id="d38e6-151">version</span></span>|<span data-ttu-id="d38e6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d38e6-152">Int32</span></span>|<span data-ttu-id="d38e6-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d38e6-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d38e6-154">limit</span><span class="sxs-lookup"><span data-stu-id="d38e6-154">limit</span></span>|<span data-ttu-id="d38e6-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d38e6-155">Int32</span></span>|<span data-ttu-id="d38e6-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d38e6-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d38e6-157">応答</span><span class="sxs-lookup"><span data-stu-id="d38e6-157">Response</span></span>
<span data-ttu-id="d38e6-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d38e6-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38e6-159">例</span><span class="sxs-lookup"><span data-stu-id="d38e6-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="d38e6-160">要求</span><span class="sxs-lookup"><span data-stu-id="d38e6-160">Request</span></span>
<span data-ttu-id="d38e6-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d38e6-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="d38e6-162">応答</span><span class="sxs-lookup"><span data-stu-id="d38e6-162">Response</span></span>
<span data-ttu-id="d38e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d38e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





