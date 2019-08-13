---
title: UserExperienceAnalyticsMetric の更新
description: UserExperienceAnalyticsMetric オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43502ab7807a3e821011faa440704a11f9e3c9d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350474"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="84954-103">UserExperienceAnalyticsMetric の更新</span><span class="sxs-lookup"><span data-stu-id="84954-103">Update userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="84954-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84954-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84954-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="84954-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84954-106">[UserExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="84954-106">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84954-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="84954-107">Prerequisites</span></span>
<span data-ttu-id="84954-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84954-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84954-110">Permission type</span></span>|<span data-ttu-id="84954-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="84954-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84954-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84954-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84954-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84954-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84954-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84954-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84954-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84954-115">Not supported.</span></span>|
|<span data-ttu-id="84954-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84954-116">Application</span></span>|<span data-ttu-id="84954-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84954-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84954-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84954-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="84954-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84954-119">Request headers</span></span>
|<span data-ttu-id="84954-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84954-120">Header</span></span>|<span data-ttu-id="84954-121">値</span><span class="sxs-lookup"><span data-stu-id="84954-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84954-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84954-122">Authorization</span></span>|<span data-ttu-id="84954-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="84954-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84954-124">承諾</span><span class="sxs-lookup"><span data-stu-id="84954-124">Accept</span></span>|<span data-ttu-id="84954-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84954-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84954-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="84954-126">Request body</span></span>
<span data-ttu-id="84954-127">要求本文で、 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="84954-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="84954-128">次の表に、 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="84954-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="84954-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84954-129">Property</span></span>|<span data-ttu-id="84954-130">型</span><span class="sxs-lookup"><span data-stu-id="84954-130">Type</span></span>|<span data-ttu-id="84954-131">説明</span><span class="sxs-lookup"><span data-stu-id="84954-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84954-132">id</span><span class="sxs-lookup"><span data-stu-id="84954-132">id</span></span>|<span data-ttu-id="84954-133">文字列</span><span class="sxs-lookup"><span data-stu-id="84954-133">String</span></span>|<span data-ttu-id="84954-134">ユーザー experience analytics 指標の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="84954-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="84954-135">displayName</span><span class="sxs-lookup"><span data-stu-id="84954-135">displayName</span></span>|<span data-ttu-id="84954-136">String</span><span class="sxs-lookup"><span data-stu-id="84954-136">String</span></span>|<span data-ttu-id="84954-137">ユーザー experience analytics 指標の名前。</span><span class="sxs-lookup"><span data-stu-id="84954-137">The name of the user experience analytics metric.</span></span>|
|<span data-ttu-id="84954-138">value</span><span class="sxs-lookup"><span data-stu-id="84954-138">value</span></span>|<span data-ttu-id="84954-139">2 行分</span><span class="sxs-lookup"><span data-stu-id="84954-139">Double</span></span>|<span data-ttu-id="84954-140">ユーザー experience analytics 指標の値。</span><span class="sxs-lookup"><span data-stu-id="84954-140">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="84954-141">本体</span><span class="sxs-lookup"><span data-stu-id="84954-141">unit</span></span>|<span data-ttu-id="84954-142">String</span><span class="sxs-lookup"><span data-stu-id="84954-142">String</span></span>|<span data-ttu-id="84954-143">ユーザー experience analytics 指標の単位。</span><span class="sxs-lookup"><span data-stu-id="84954-143">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="84954-144">応答</span><span class="sxs-lookup"><span data-stu-id="84954-144">Response</span></span>
<span data-ttu-id="84954-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84954-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84954-146">例</span><span class="sxs-lookup"><span data-stu-id="84954-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="84954-147">要求</span><span class="sxs-lookup"><span data-stu-id="84954-147">Request</span></span>
<span data-ttu-id="84954-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84954-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "displayName": "Display Name value",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="84954-149">応答</span><span class="sxs-lookup"><span data-stu-id="84954-149">Response</span></span>
<span data-ttu-id="84954-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84954-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "displayName": "Display Name value",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```






