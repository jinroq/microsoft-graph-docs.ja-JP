---
title: deviceEnrollmentLimitConfiguration の作成
description: 新しい deviceEnrollmentLimitConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95431986b1b8a47c723f493295b64989bb3db3d5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165353"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="18ed5-103">deviceEnrollmentLimitConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="18ed5-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="18ed5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18ed5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18ed5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18ed5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18ed5-106">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="18ed5-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18ed5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="18ed5-107">Prerequisites</span></span>
<span data-ttu-id="18ed5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18ed5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18ed5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18ed5-110">Permission type</span></span>|<span data-ttu-id="18ed5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18ed5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18ed5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18ed5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18ed5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18ed5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18ed5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18ed5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18ed5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18ed5-115">Not supported.</span></span>|
|<span data-ttu-id="18ed5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18ed5-116">Application</span></span>|<span data-ttu-id="18ed5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18ed5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18ed5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18ed5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18ed5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18ed5-119">Request headers</span></span>
|<span data-ttu-id="18ed5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18ed5-120">Header</span></span>|<span data-ttu-id="18ed5-121">値</span><span class="sxs-lookup"><span data-stu-id="18ed5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18ed5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18ed5-122">Authorization</span></span>|<span data-ttu-id="18ed5-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="18ed5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18ed5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="18ed5-124">Accept</span></span>|<span data-ttu-id="18ed5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18ed5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18ed5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="18ed5-126">Request body</span></span>
<span data-ttu-id="18ed5-127">要求本文で、deviceEnrollmentLimitConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18ed5-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="18ed5-128">次の表に、deviceEnrollmentLimitConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="18ed5-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="18ed5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18ed5-129">Property</span></span>|<span data-ttu-id="18ed5-130">型</span><span class="sxs-lookup"><span data-stu-id="18ed5-130">Type</span></span>|<span data-ttu-id="18ed5-131">説明</span><span class="sxs-lookup"><span data-stu-id="18ed5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18ed5-132">id</span><span class="sxs-lookup"><span data-stu-id="18ed5-132">id</span></span>|<span data-ttu-id="18ed5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="18ed5-133">String</span></span>|<span data-ttu-id="18ed5-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="18ed5-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="18ed5-135">displayName</span></span>|<span data-ttu-id="18ed5-136">String</span><span class="sxs-lookup"><span data-stu-id="18ed5-136">String</span></span>|<span data-ttu-id="18ed5-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18ed5-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-138">説明</span><span class="sxs-lookup"><span data-stu-id="18ed5-138">description</span></span>|<span data-ttu-id="18ed5-139">String</span><span class="sxs-lookup"><span data-stu-id="18ed5-139">String</span></span>|<span data-ttu-id="18ed5-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18ed5-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-141">priority</span><span class="sxs-lookup"><span data-stu-id="18ed5-141">priority</span></span>|<span data-ttu-id="18ed5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="18ed5-142">Int32</span></span>|<span data-ttu-id="18ed5-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18ed5-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18ed5-144">createdDateTime</span></span>|<span data-ttu-id="18ed5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18ed5-145">DateTimeOffset</span></span>|<span data-ttu-id="18ed5-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18ed5-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18ed5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="18ed5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18ed5-148">DateTimeOffset</span></span>|<span data-ttu-id="18ed5-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18ed5-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-150">version</span><span class="sxs-lookup"><span data-stu-id="18ed5-150">version</span></span>|<span data-ttu-id="18ed5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="18ed5-151">Int32</span></span>|<span data-ttu-id="18ed5-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18ed5-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="18ed5-153">limit</span><span class="sxs-lookup"><span data-stu-id="18ed5-153">limit</span></span>|<span data-ttu-id="18ed5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="18ed5-154">Int32</span></span>|<span data-ttu-id="18ed5-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="18ed5-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="18ed5-156">応答</span><span class="sxs-lookup"><span data-stu-id="18ed5-156">Response</span></span>
<span data-ttu-id="18ed5-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18ed5-157">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18ed5-158">例</span><span class="sxs-lookup"><span data-stu-id="18ed5-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="18ed5-159">要求</span><span class="sxs-lookup"><span data-stu-id="18ed5-159">Request</span></span>
<span data-ttu-id="18ed5-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18ed5-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18ed5-161">応答</span><span class="sxs-lookup"><span data-stu-id="18ed5-161">Response</span></span>
<span data-ttu-id="18ed5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18ed5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




