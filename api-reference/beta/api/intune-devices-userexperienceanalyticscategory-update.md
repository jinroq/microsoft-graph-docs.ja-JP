---
title: UserExperienceAnalyticsCategory の更新
description: UserExperienceAnalyticsCategory オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f99c4bd2090f751b0a54df6ad408cda463266605
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350476"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="a07b8-103">UserExperienceAnalyticsCategory の更新</span><span class="sxs-lookup"><span data-stu-id="a07b8-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="a07b8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a07b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a07b8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a07b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a07b8-106">[UserExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a07b8-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a07b8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a07b8-107">Prerequisites</span></span>
<span data-ttu-id="a07b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a07b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a07b8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a07b8-110">Permission type</span></span>|<span data-ttu-id="a07b8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a07b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a07b8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a07b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a07b8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07b8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a07b8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a07b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a07b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a07b8-115">Not supported.</span></span>|
|<span data-ttu-id="a07b8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a07b8-116">Application</span></span>|<span data-ttu-id="a07b8-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07b8-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a07b8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a07b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="a07b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a07b8-119">Request headers</span></span>
|<span data-ttu-id="a07b8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a07b8-120">Header</span></span>|<span data-ttu-id="a07b8-121">値</span><span class="sxs-lookup"><span data-stu-id="a07b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a07b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a07b8-122">Authorization</span></span>|<span data-ttu-id="a07b8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a07b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a07b8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a07b8-124">Accept</span></span>|<span data-ttu-id="a07b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a07b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a07b8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a07b8-126">Request body</span></span>
<span data-ttu-id="a07b8-127">要求本文で、 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a07b8-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="a07b8-128">次の表に、 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a07b8-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="a07b8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a07b8-129">Property</span></span>|<span data-ttu-id="a07b8-130">型</span><span class="sxs-lookup"><span data-stu-id="a07b8-130">Type</span></span>|<span data-ttu-id="a07b8-131">説明</span><span class="sxs-lookup"><span data-stu-id="a07b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a07b8-132">id</span><span class="sxs-lookup"><span data-stu-id="a07b8-132">id</span></span>|<span data-ttu-id="a07b8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a07b8-133">String</span></span>|<span data-ttu-id="a07b8-134">ユーザー experience analytics カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a07b8-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="a07b8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a07b8-135">displayName</span></span>|<span data-ttu-id="a07b8-136">String</span><span class="sxs-lookup"><span data-stu-id="a07b8-136">String</span></span>|<span data-ttu-id="a07b8-137">ユーザー experience analytics カテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="a07b8-137">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="a07b8-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="a07b8-138">overallScore</span></span>|<span data-ttu-id="a07b8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a07b8-139">Int32</span></span>|<span data-ttu-id="a07b8-140">ユーザー experience analytics カテゴリの全体的なスコア。</span><span class="sxs-lookup"><span data-stu-id="a07b8-140">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="a07b8-141">insights</span><span class="sxs-lookup"><span data-stu-id="a07b8-141">insights</span></span>|<span data-ttu-id="a07b8-142">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a07b8-142">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a07b8-143">ユーザー experience analytics カテゴリの洞察。</span><span class="sxs-lookup"><span data-stu-id="a07b8-143">The insights for the user experience analytics category.</span></span>|



## <a name="response"></a><span data-ttu-id="a07b8-144">応答</span><span class="sxs-lookup"><span data-stu-id="a07b8-144">Response</span></span>
<span data-ttu-id="a07b8-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a07b8-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07b8-146">例</span><span class="sxs-lookup"><span data-stu-id="a07b8-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="a07b8-147">要求</span><span class="sxs-lookup"><span data-stu-id="a07b8-147">Request</span></span>
<span data-ttu-id="a07b8-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a07b8-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 484

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "displayName": "Display Name value",
  "overallScore": 12,
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

### <a name="response"></a><span data-ttu-id="a07b8-149">応答</span><span class="sxs-lookup"><span data-stu-id="a07b8-149">Response</span></span>
<span data-ttu-id="a07b8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a07b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 533

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "displayName": "Display Name value",
  "overallScore": 12,
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






