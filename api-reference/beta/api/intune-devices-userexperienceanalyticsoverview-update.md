---
title: UserExperienceAnalyticsOverview の更新
description: UserExperienceAnalyticsOverview オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb00499ea103b89dc45e1b5028858b0747f5163e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350472"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="4d02f-103">UserExperienceAnalyticsOverview の更新</span><span class="sxs-lookup"><span data-stu-id="4d02f-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="4d02f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d02f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d02f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d02f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d02f-106">[UserExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4d02f-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d02f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4d02f-107">Prerequisites</span></span>
<span data-ttu-id="4d02f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d02f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d02f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d02f-110">Permission type</span></span>|<span data-ttu-id="4d02f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d02f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d02f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d02f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d02f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d02f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4d02f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d02f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d02f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d02f-115">Not supported.</span></span>|
|<span data-ttu-id="4d02f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d02f-116">Application</span></span>|<span data-ttu-id="4d02f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d02f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d02f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d02f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="4d02f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d02f-119">Request headers</span></span>
|<span data-ttu-id="4d02f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d02f-120">Header</span></span>|<span data-ttu-id="4d02f-121">値</span><span class="sxs-lookup"><span data-stu-id="4d02f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d02f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d02f-122">Authorization</span></span>|<span data-ttu-id="4d02f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d02f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d02f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4d02f-124">Accept</span></span>|<span data-ttu-id="4d02f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d02f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d02f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d02f-126">Request body</span></span>
<span data-ttu-id="4d02f-127">要求本文で、 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d02f-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="4d02f-128">次の表に、 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4d02f-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="4d02f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d02f-129">Property</span></span>|<span data-ttu-id="4d02f-130">型</span><span class="sxs-lookup"><span data-stu-id="4d02f-130">Type</span></span>|<span data-ttu-id="4d02f-131">説明</span><span class="sxs-lookup"><span data-stu-id="4d02f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d02f-132">id</span><span class="sxs-lookup"><span data-stu-id="4d02f-132">id</span></span>|<span data-ttu-id="4d02f-133">String</span><span class="sxs-lookup"><span data-stu-id="4d02f-133">String</span></span>|<span data-ttu-id="4d02f-134">ユーザー experience analytics の概要の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="4d02f-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="4d02f-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="4d02f-135">overallScore</span></span>|<span data-ttu-id="4d02f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4d02f-136">Int32</span></span>|<span data-ttu-id="4d02f-137">ユーザー experience analytics 総合得点。</span><span class="sxs-lookup"><span data-stu-id="4d02f-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="4d02f-138">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="4d02f-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="4d02f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4d02f-139">Int32</span></span>|<span data-ttu-id="4d02f-140">ユーザーが analytics デバイスのブートパフォーマンス全体スコアを表示します。</span><span class="sxs-lookup"><span data-stu-id="4d02f-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="4d02f-141">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="4d02f-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="4d02f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4d02f-142">Int32</span></span>|<span data-ttu-id="4d02f-143">ユーザー操作分析のベストプラクティス全体のスコア。</span><span class="sxs-lookup"><span data-stu-id="4d02f-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="4d02f-144">insights</span><span class="sxs-lookup"><span data-stu-id="4d02f-144">insights</span></span>|<span data-ttu-id="4d02f-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4d02f-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="4d02f-146">ユーザー experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="4d02f-146">The user experience analytics insights.</span></span>|



## <a name="response"></a><span data-ttu-id="4d02f-147">応答</span><span class="sxs-lookup"><span data-stu-id="4d02f-147">Response</span></span>
<span data-ttu-id="4d02f-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4d02f-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d02f-149">例</span><span class="sxs-lookup"><span data-stu-id="4d02f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d02f-150">要求</span><span class="sxs-lookup"><span data-stu-id="4d02f-150">Request</span></span>
<span data-ttu-id="4d02f-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d02f-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4d02f-152">応答</span><span class="sxs-lookup"><span data-stu-id="4d02f-152">Response</span></span>
<span data-ttu-id="4d02f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d02f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 571

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```






