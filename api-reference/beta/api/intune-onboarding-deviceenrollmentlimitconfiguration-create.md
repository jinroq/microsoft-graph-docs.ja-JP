---
title: deviceEnrollmentLimitConfiguration の作成
description: 新しい deviceEnrollmentLimitConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13b0759a423f2202a93a65c2aeea9b5af5824ed0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798454"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="f156a-103">deviceEnrollmentLimitConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="f156a-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="f156a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f156a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f156a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f156a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f156a-106">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f156a-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f156a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f156a-107">Prerequisites</span></span>
<span data-ttu-id="f156a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f156a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f156a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f156a-110">Permission type</span></span>|<span data-ttu-id="f156a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f156a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f156a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f156a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f156a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f156a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f156a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f156a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f156a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f156a-115">Not supported.</span></span>|
|<span data-ttu-id="f156a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f156a-116">Application</span></span>|<span data-ttu-id="f156a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f156a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f156a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f156a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f156a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f156a-119">Request headers</span></span>
|<span data-ttu-id="f156a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f156a-120">Header</span></span>|<span data-ttu-id="f156a-121">値</span><span class="sxs-lookup"><span data-stu-id="f156a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f156a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f156a-122">Authorization</span></span>|<span data-ttu-id="f156a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f156a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f156a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f156a-124">Accept</span></span>|<span data-ttu-id="f156a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f156a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f156a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f156a-126">Request body</span></span>
<span data-ttu-id="f156a-127">要求本文で、deviceEnrollmentLimitConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f156a-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="f156a-128">次の表に、deviceEnrollmentLimitConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f156a-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="f156a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f156a-129">Property</span></span>|<span data-ttu-id="f156a-130">型</span><span class="sxs-lookup"><span data-stu-id="f156a-130">Type</span></span>|<span data-ttu-id="f156a-131">説明</span><span class="sxs-lookup"><span data-stu-id="f156a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f156a-132">id</span><span class="sxs-lookup"><span data-stu-id="f156a-132">id</span></span>|<span data-ttu-id="f156a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f156a-133">String</span></span>|<span data-ttu-id="f156a-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="f156a-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f156a-135">displayName</span></span>|<span data-ttu-id="f156a-136">String</span><span class="sxs-lookup"><span data-stu-id="f156a-136">String</span></span>|<span data-ttu-id="f156a-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f156a-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-138">説明</span><span class="sxs-lookup"><span data-stu-id="f156a-138">description</span></span>|<span data-ttu-id="f156a-139">String</span><span class="sxs-lookup"><span data-stu-id="f156a-139">String</span></span>|<span data-ttu-id="f156a-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f156a-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-141">priority</span><span class="sxs-lookup"><span data-stu-id="f156a-141">priority</span></span>|<span data-ttu-id="f156a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f156a-142">Int32</span></span>|<span data-ttu-id="f156a-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f156a-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f156a-144">createdDateTime</span></span>|<span data-ttu-id="f156a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f156a-145">DateTimeOffset</span></span>|<span data-ttu-id="f156a-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f156a-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f156a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f156a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f156a-148">DateTimeOffset</span></span>|<span data-ttu-id="f156a-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f156a-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-150">version</span><span class="sxs-lookup"><span data-stu-id="f156a-150">version</span></span>|<span data-ttu-id="f156a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f156a-151">Int32</span></span>|<span data-ttu-id="f156a-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f156a-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f156a-153">limit</span><span class="sxs-lookup"><span data-stu-id="f156a-153">limit</span></span>|<span data-ttu-id="f156a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f156a-154">Int32</span></span>|<span data-ttu-id="f156a-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f156a-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f156a-156">応答</span><span class="sxs-lookup"><span data-stu-id="f156a-156">Response</span></span>
<span data-ttu-id="f156a-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f156a-157">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f156a-158">例</span><span class="sxs-lookup"><span data-stu-id="f156a-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f156a-159">要求</span><span class="sxs-lookup"><span data-stu-id="f156a-159">Request</span></span>
<span data-ttu-id="f156a-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f156a-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f156a-161">応答</span><span class="sxs-lookup"><span data-stu-id="f156a-161">Response</span></span>
<span data-ttu-id="f156a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f156a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





