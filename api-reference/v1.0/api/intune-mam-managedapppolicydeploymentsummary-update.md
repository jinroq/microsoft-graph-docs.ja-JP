---
title: managedAppPolicyDeploymentSummary の更新
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2522d6a9867993a88ec5420a37da9005e8bd94f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263225"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="928f9-103">managedAppPolicyDeploymentSummary の更新</span><span class="sxs-lookup"><span data-stu-id="928f9-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="928f9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="928f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="928f9-105">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="928f9-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="928f9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="928f9-106">Prerequisites</span></span>
<span data-ttu-id="928f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="928f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="928f9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="928f9-109">Permission type</span></span>|<span data-ttu-id="928f9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="928f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="928f9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="928f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="928f9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="928f9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="928f9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="928f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="928f9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="928f9-114">Not supported.</span></span>|
|<span data-ttu-id="928f9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="928f9-115">Application</span></span>|<span data-ttu-id="928f9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="928f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="928f9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="928f9-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="928f9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="928f9-118">Request headers</span></span>
|<span data-ttu-id="928f9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="928f9-119">Header</span></span>|<span data-ttu-id="928f9-120">値</span><span class="sxs-lookup"><span data-stu-id="928f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="928f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="928f9-121">Authorization</span></span>|<span data-ttu-id="928f9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="928f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="928f9-123">承諾</span><span class="sxs-lookup"><span data-stu-id="928f9-123">Accept</span></span>|<span data-ttu-id="928f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="928f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="928f9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="928f9-125">Request body</span></span>
<span data-ttu-id="928f9-126">要求本文で、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="928f9-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="928f9-127">次の表に、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="928f9-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="928f9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="928f9-128">Property</span></span>|<span data-ttu-id="928f9-129">型</span><span class="sxs-lookup"><span data-stu-id="928f9-129">Type</span></span>|<span data-ttu-id="928f9-130">説明</span><span class="sxs-lookup"><span data-stu-id="928f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="928f9-131">displayName</span><span class="sxs-lookup"><span data-stu-id="928f9-131">displayName</span></span>|<span data-ttu-id="928f9-132">String</span><span class="sxs-lookup"><span data-stu-id="928f9-132">String</span></span>|<span data-ttu-id="928f9-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="928f9-133">Not yet documented</span></span>|
|<span data-ttu-id="928f9-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="928f9-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="928f9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="928f9-135">Int32</span></span>|<span data-ttu-id="928f9-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="928f9-136">Not yet documented</span></span>|
|<span data-ttu-id="928f9-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="928f9-137">lastRefreshTime</span></span>|<span data-ttu-id="928f9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="928f9-138">DateTimeOffset</span></span>|<span data-ttu-id="928f9-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="928f9-139">Not yet documented</span></span>|
|<span data-ttu-id="928f9-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="928f9-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="928f9-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="928f9-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="928f9-142">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="928f9-142">Not yet documented</span></span>|
|<span data-ttu-id="928f9-143">id</span><span class="sxs-lookup"><span data-stu-id="928f9-143">id</span></span>|<span data-ttu-id="928f9-144">文字列</span><span class="sxs-lookup"><span data-stu-id="928f9-144">String</span></span>|<span data-ttu-id="928f9-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="928f9-145">Key of the entity.</span></span>|
|<span data-ttu-id="928f9-146">version</span><span class="sxs-lookup"><span data-stu-id="928f9-146">version</span></span>|<span data-ttu-id="928f9-147">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="928f9-147">String</span></span>|<span data-ttu-id="928f9-148">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="928f9-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="928f9-149">応答</span><span class="sxs-lookup"><span data-stu-id="928f9-149">Response</span></span>
<span data-ttu-id="928f9-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="928f9-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="928f9-151">例</span><span class="sxs-lookup"><span data-stu-id="928f9-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="928f9-152">要求</span><span class="sxs-lookup"><span data-stu-id="928f9-152">Request</span></span>
<span data-ttu-id="928f9-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="928f9-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 588

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
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="928f9-154">応答</span><span class="sxs-lookup"><span data-stu-id="928f9-154">Response</span></span>
<span data-ttu-id="928f9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="928f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



