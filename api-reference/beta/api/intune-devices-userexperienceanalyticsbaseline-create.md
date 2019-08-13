---
title: UserExperienceAnalyticsBaseline を作成する
description: 新しい userExperienceAnalyticsBaseline オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1877d4f6cc964e311025a10988803723b1806510
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350482"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="1dc8e-103">UserExperienceAnalyticsBaseline を作成する</span><span class="sxs-lookup"><span data-stu-id="1dc8e-103">Create userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="1dc8e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dc8e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc8e-106">新しい[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-106">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dc8e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1dc8e-107">Prerequisites</span></span>
<span data-ttu-id="1dc8e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc8e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dc8e-110">Permission type</span></span>|<span data-ttu-id="1dc8e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dc8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dc8e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dc8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dc8e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc8e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1dc8e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dc8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dc8e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-115">Not supported.</span></span>|
|<span data-ttu-id="1dc8e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dc8e-116">Application</span></span>|<span data-ttu-id="1dc8e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc8e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dc8e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dc8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="1dc8e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dc8e-119">Request headers</span></span>
|<span data-ttu-id="1dc8e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dc8e-120">Header</span></span>|<span data-ttu-id="1dc8e-121">値</span><span class="sxs-lookup"><span data-stu-id="1dc8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dc8e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc8e-122">Authorization</span></span>|<span data-ttu-id="1dc8e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dc8e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1dc8e-124">Accept</span></span>|<span data-ttu-id="1dc8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1dc8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dc8e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dc8e-126">Request body</span></span>
<span data-ttu-id="1dc8e-127">要求本文で、userExperienceAnalyticsBaseline オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-127">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="1dc8e-128">次の表に、userExperienceAnalyticsBaseline の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-128">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="1dc8e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dc8e-129">Property</span></span>|<span data-ttu-id="1dc8e-130">型</span><span class="sxs-lookup"><span data-stu-id="1dc8e-130">Type</span></span>|<span data-ttu-id="1dc8e-131">説明</span><span class="sxs-lookup"><span data-stu-id="1dc8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc8e-132">id</span><span class="sxs-lookup"><span data-stu-id="1dc8e-132">id</span></span>|<span data-ttu-id="1dc8e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1dc8e-133">String</span></span>|<span data-ttu-id="1dc8e-134">ユーザー experience analytics のベースラインの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="1dc8e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1dc8e-135">displayName</span></span>|<span data-ttu-id="1dc8e-136">String</span><span class="sxs-lookup"><span data-stu-id="1dc8e-136">String</span></span>|<span data-ttu-id="1dc8e-137">ユーザー experience analytics のベースラインの名前。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="1dc8e-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="1dc8e-138">overallScore</span></span>|<span data-ttu-id="1dc8e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc8e-139">Int32</span></span>|<span data-ttu-id="1dc8e-140">ユーザー experience analytics のベースラインの全体的なスコア。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="1dc8e-141">overallRegressionThreshold</span><span class="sxs-lookup"><span data-stu-id="1dc8e-141">overallRegressionThreshold</span></span>|<span data-ttu-id="1dc8e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc8e-142">Int32</span></span>|<span data-ttu-id="1dc8e-143">ユーザー experience analytics のベースラインの全体的な回帰しきい値。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-143">The overall regression threshold of the user experience analytics baseline.</span></span>|



## <a name="response"></a><span data-ttu-id="1dc8e-144">応答</span><span class="sxs-lookup"><span data-stu-id="1dc8e-144">Response</span></span>
<span data-ttu-id="1dc8e-145">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-145">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc8e-146">例</span><span class="sxs-lookup"><span data-stu-id="1dc8e-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dc8e-147">要求</span><span class="sxs-lookup"><span data-stu-id="1dc8e-147">Request</span></span>
<span data-ttu-id="1dc8e-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "overallRegressionThreshold": 10
}
```

### <a name="response"></a><span data-ttu-id="1dc8e-149">応答</span><span class="sxs-lookup"><span data-stu-id="1dc8e-149">Response</span></span>
<span data-ttu-id="1dc8e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1dc8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "overallRegressionThreshold": 10
}
```






