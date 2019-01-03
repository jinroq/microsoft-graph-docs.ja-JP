---
title: managedAppPolicyDeploymentSummary の取得
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 7c33021c0bfa31f6a562bfc54efb4d8d195dadd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334882"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="a44f9-103">managedAppPolicyDeploymentSummary の取得</span><span class="sxs-lookup"><span data-stu-id="a44f9-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="a44f9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a44f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a44f9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a44f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a44f9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a44f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a44f9-107">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a44f9-107">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a44f9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a44f9-108">Prerequisites</span></span>
<span data-ttu-id="a44f9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a44f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a44f9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a44f9-111">Permission type</span></span>|<span data-ttu-id="a44f9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a44f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a44f9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a44f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a44f9-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a44f9-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a44f9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a44f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a44f9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a44f9-116">Not supported.</span></span>|
|<span data-ttu-id="a44f9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a44f9-117">Application</span></span>|<span data-ttu-id="a44f9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a44f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a44f9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a44f9-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="a44f9-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a44f9-120">Optional query parameters</span></span>
<span data-ttu-id="a44f9-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a44f9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a44f9-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a44f9-122">Request headers</span></span>
|<span data-ttu-id="a44f9-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a44f9-123">Header</span></span>|<span data-ttu-id="a44f9-124">値</span><span class="sxs-lookup"><span data-stu-id="a44f9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a44f9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a44f9-125">Authorization</span></span>|<span data-ttu-id="a44f9-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a44f9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a44f9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a44f9-127">Accept</span></span>|<span data-ttu-id="a44f9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a44f9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a44f9-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a44f9-129">Request body</span></span>
<span data-ttu-id="a44f9-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a44f9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a44f9-131">応答</span><span class="sxs-lookup"><span data-stu-id="a44f9-131">Response</span></span>
<span data-ttu-id="a44f9-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a44f9-132">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a44f9-133">例</span><span class="sxs-lookup"><span data-stu-id="a44f9-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a44f9-134">要求</span><span class="sxs-lookup"><span data-stu-id="a44f9-134">Request</span></span>
<span data-ttu-id="a44f9-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a44f9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="a44f9-136">応答</span><span class="sxs-lookup"><span data-stu-id="a44f9-136">Response</span></span>
<span data-ttu-id="a44f9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a44f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




