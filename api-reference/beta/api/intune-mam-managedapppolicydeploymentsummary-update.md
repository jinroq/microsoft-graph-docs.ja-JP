---
title: managedAppPolicyDeploymentSummary の更新
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティを更新します。
ms.openlocfilehash: 2c0bf77e3dbd3720bcb0cfea28d69155174fb776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074475"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="19b92-103">managedAppPolicyDeploymentSummary の更新</span><span class="sxs-lookup"><span data-stu-id="19b92-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="19b92-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19b92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19b92-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19b92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19b92-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="19b92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19b92-107">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="19b92-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19b92-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="19b92-108">Prerequisites</span></span>
<span data-ttu-id="19b92-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19b92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b92-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19b92-111">Permission type</span></span>|<span data-ttu-id="19b92-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="19b92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19b92-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19b92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19b92-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b92-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19b92-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19b92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19b92-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19b92-116">Not supported.</span></span>|
|<span data-ttu-id="19b92-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19b92-117">Application</span></span>|<span data-ttu-id="19b92-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19b92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b92-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19b92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="19b92-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19b92-120">Request headers</span></span>
|<span data-ttu-id="19b92-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19b92-121">Header</span></span>|<span data-ttu-id="19b92-122">値</span><span class="sxs-lookup"><span data-stu-id="19b92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19b92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19b92-123">Authorization</span></span>|<span data-ttu-id="19b92-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="19b92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19b92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19b92-125">Accept</span></span>|<span data-ttu-id="19b92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19b92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b92-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="19b92-127">Request body</span></span>
<span data-ttu-id="19b92-128">要求本文で、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19b92-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="19b92-129">次の表に、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="19b92-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="19b92-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19b92-130">Property</span></span>|<span data-ttu-id="19b92-131">型</span><span class="sxs-lookup"><span data-stu-id="19b92-131">Type</span></span>|<span data-ttu-id="19b92-132">説明</span><span class="sxs-lookup"><span data-stu-id="19b92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b92-133">displayName</span><span class="sxs-lookup"><span data-stu-id="19b92-133">displayName</span></span>|<span data-ttu-id="19b92-134">String</span><span class="sxs-lookup"><span data-stu-id="19b92-134">String</span></span>|<span data-ttu-id="19b92-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="19b92-135">Not yet documented</span></span>|
|<span data-ttu-id="19b92-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="19b92-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="19b92-137">Int32</span><span class="sxs-lookup"><span data-stu-id="19b92-137">Int32</span></span>|<span data-ttu-id="19b92-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="19b92-138">Not yet documented</span></span>|
|<span data-ttu-id="19b92-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="19b92-139">lastRefreshTime</span></span>|<span data-ttu-id="19b92-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19b92-140">DateTimeOffset</span></span>|<span data-ttu-id="19b92-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="19b92-141">Not yet documented</span></span>|
|<span data-ttu-id="19b92-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="19b92-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="19b92-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19b92-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="19b92-144">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="19b92-144">Not yet documented</span></span>|
|<span data-ttu-id="19b92-145">id</span><span class="sxs-lookup"><span data-stu-id="19b92-145">id</span></span>|<span data-ttu-id="19b92-146">String</span><span class="sxs-lookup"><span data-stu-id="19b92-146">String</span></span>|<span data-ttu-id="19b92-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="19b92-147">Key of the entity.</span></span>|
|<span data-ttu-id="19b92-148">version</span><span class="sxs-lookup"><span data-stu-id="19b92-148">version</span></span>|<span data-ttu-id="19b92-149">String</span><span class="sxs-lookup"><span data-stu-id="19b92-149">String</span></span>|<span data-ttu-id="19b92-150">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="19b92-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="19b92-151">応答</span><span class="sxs-lookup"><span data-stu-id="19b92-151">Response</span></span>
<span data-ttu-id="19b92-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19b92-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b92-153">例</span><span class="sxs-lookup"><span data-stu-id="19b92-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="19b92-154">要求</span><span class="sxs-lookup"><span data-stu-id="19b92-154">Request</span></span>
<span data-ttu-id="19b92-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="19b92-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
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
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="19b92-156">応答</span><span class="sxs-lookup"><span data-stu-id="19b92-156">Response</span></span>
<span data-ttu-id="19b92-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="19b92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
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
```




