---
title: managedAppPolicyDeploymentSummary の取得
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b05281ba4acbf3b13d391ac1adbfc94d25a5b787
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354150"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="e84db-103">managedAppPolicyDeploymentSummary の取得</span><span class="sxs-lookup"><span data-stu-id="e84db-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="e84db-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e84db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e84db-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e84db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e84db-106">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e84db-106">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e84db-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e84db-107">Prerequisites</span></span>
<span data-ttu-id="e84db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e84db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e84db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e84db-110">Permission type</span></span>|<span data-ttu-id="e84db-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e84db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e84db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e84db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e84db-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e84db-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e84db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e84db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e84db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e84db-115">Not supported.</span></span>|
|<span data-ttu-id="e84db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e84db-116">Application</span></span>|<span data-ttu-id="e84db-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e84db-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e84db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e84db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e84db-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e84db-119">Optional query parameters</span></span>
<span data-ttu-id="e84db-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e84db-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e84db-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e84db-121">Request headers</span></span>
|<span data-ttu-id="e84db-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e84db-122">Header</span></span>|<span data-ttu-id="e84db-123">値</span><span class="sxs-lookup"><span data-stu-id="e84db-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e84db-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e84db-124">Authorization</span></span>|<span data-ttu-id="e84db-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e84db-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e84db-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e84db-126">Accept</span></span>|<span data-ttu-id="e84db-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e84db-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e84db-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e84db-128">Request body</span></span>
<span data-ttu-id="e84db-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e84db-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e84db-130">応答</span><span class="sxs-lookup"><span data-stu-id="e84db-130">Response</span></span>
<span data-ttu-id="e84db-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e84db-131">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e84db-132">例</span><span class="sxs-lookup"><span data-stu-id="e84db-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e84db-133">要求</span><span class="sxs-lookup"><span data-stu-id="e84db-133">Request</span></span>
<span data-ttu-id="e84db-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e84db-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="e84db-135">応答</span><span class="sxs-lookup"><span data-stu-id="e84db-135">Response</span></span>
<span data-ttu-id="e84db-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e84db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
    "version": "Version value"
  }
}
```






