---
title: managedAppPolicyDeploymentSummary の取得
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 57517a3edbde884819a1d7671e2c75fbaa40056e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021644"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="b0625-103">managedAppPolicyDeploymentSummary の取得</span><span class="sxs-lookup"><span data-stu-id="b0625-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="b0625-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0625-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0625-105">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b0625-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0625-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b0625-106">Prerequisites</span></span>
<span data-ttu-id="b0625-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0625-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0625-109">Permission type</span></span>|<span data-ttu-id="b0625-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0625-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0625-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0625-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0625-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0625-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0625-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0625-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0625-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0625-114">Not supported.</span></span>|
|<span data-ttu-id="b0625-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0625-115">Application</span></span>|<span data-ttu-id="b0625-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0625-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0625-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0625-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="b0625-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0625-118">Optional query parameters</span></span>
<span data-ttu-id="b0625-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b0625-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0625-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0625-120">Request headers</span></span>
|<span data-ttu-id="b0625-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0625-121">Header</span></span>|<span data-ttu-id="b0625-122">値</span><span class="sxs-lookup"><span data-stu-id="b0625-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0625-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0625-123">Authorization</span></span>|<span data-ttu-id="b0625-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b0625-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0625-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0625-125">Accept</span></span>|<span data-ttu-id="b0625-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0625-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0625-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0625-127">Request body</span></span>
<span data-ttu-id="b0625-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0625-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0625-129">応答</span><span class="sxs-lookup"><span data-stu-id="b0625-129">Response</span></span>
<span data-ttu-id="b0625-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0625-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0625-131">例</span><span class="sxs-lookup"><span data-stu-id="b0625-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0625-132">要求</span><span class="sxs-lookup"><span data-stu-id="b0625-132">Request</span></span>
<span data-ttu-id="b0625-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0625-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="b0625-134">応答</span><span class="sxs-lookup"><span data-stu-id="b0625-134">Response</span></span>
<span data-ttu-id="b0625-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0625-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



