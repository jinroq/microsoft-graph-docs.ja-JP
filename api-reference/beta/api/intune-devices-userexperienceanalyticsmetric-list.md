---
title: リスト userExperienceAnalyticsMetrics
description: UserExperienceAnalyticsMetric オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eff204bba76ec0f84d9a904f3a78fecb97320437
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311696"
---
# <a name="list-userexperienceanalyticsmetrics"></a><span data-ttu-id="426dd-103">リスト userExperienceAnalyticsMetrics</span><span class="sxs-lookup"><span data-stu-id="426dd-103">List userExperienceAnalyticsMetrics</span></span>

> <span data-ttu-id="426dd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="426dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="426dd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="426dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="426dd-106">[UserExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="426dd-106">List properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="426dd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="426dd-107">Prerequisites</span></span>
<span data-ttu-id="426dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="426dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="426dd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="426dd-110">Permission type</span></span>|<span data-ttu-id="426dd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="426dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="426dd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="426dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="426dd-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="426dd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="426dd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="426dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="426dd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="426dd-115">Not supported.</span></span>|
|<span data-ttu-id="426dd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="426dd-116">Application</span></span>|<span data-ttu-id="426dd-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="426dd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="426dd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="426dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="426dd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="426dd-119">Request headers</span></span>
|<span data-ttu-id="426dd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="426dd-120">Header</span></span>|<span data-ttu-id="426dd-121">値</span><span class="sxs-lookup"><span data-stu-id="426dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="426dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="426dd-122">Authorization</span></span>|<span data-ttu-id="426dd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="426dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="426dd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="426dd-124">Accept</span></span>|<span data-ttu-id="426dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="426dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="426dd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="426dd-126">Request body</span></span>
<span data-ttu-id="426dd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="426dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="426dd-128">応答</span><span class="sxs-lookup"><span data-stu-id="426dd-128">Response</span></span>
<span data-ttu-id="426dd-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="426dd-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="426dd-130">例</span><span class="sxs-lookup"><span data-stu-id="426dd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="426dd-131">要求</span><span class="sxs-lookup"><span data-stu-id="426dd-131">Request</span></span>
<span data-ttu-id="426dd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="426dd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

### <a name="response"></a><span data-ttu-id="426dd-133">応答</span><span class="sxs-lookup"><span data-stu-id="426dd-133">Response</span></span>
<span data-ttu-id="426dd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="426dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
      "id": "1371822e-822e-1371-2e82-71132e827113",
      "displayName": "Display Name value",
      "value": "<Unknown Primitive Type Edm.Double>",
      "unit": "Unit value"
    }
  ]
}
```






