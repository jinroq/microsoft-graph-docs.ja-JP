---
title: managedAppPolicyDeploymentSummary の更新
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f940bac34deca1aa938784eee514b765a78ce64a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408146"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="22f66-103">managedAppPolicyDeploymentSummary の更新</span><span class="sxs-lookup"><span data-stu-id="22f66-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="22f66-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22f66-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22f66-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22f66-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22f66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f66-107">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22f66-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f66-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="22f66-108">Prerequisites</span></span>
<span data-ttu-id="22f66-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22f66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="22f66-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22f66-111">Permission type</span></span>|<span data-ttu-id="22f66-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22f66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f66-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22f66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22f66-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f66-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22f66-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22f66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f66-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f66-116">Not supported.</span></span>|
|<span data-ttu-id="22f66-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22f66-117">Application</span></span>|<span data-ttu-id="22f66-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f66-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f66-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22f66-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="22f66-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22f66-120">Request headers</span></span>
|<span data-ttu-id="22f66-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22f66-121">Header</span></span>|<span data-ttu-id="22f66-122">値</span><span class="sxs-lookup"><span data-stu-id="22f66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22f66-123">Authorization</span></span>|<span data-ttu-id="22f66-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="22f66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22f66-125">Accept</span></span>|<span data-ttu-id="22f66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22f66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f66-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="22f66-127">Request body</span></span>
<span data-ttu-id="22f66-128">要求本文で、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22f66-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="22f66-129">次の表に、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22f66-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="22f66-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22f66-130">Property</span></span>|<span data-ttu-id="22f66-131">型</span><span class="sxs-lookup"><span data-stu-id="22f66-131">Type</span></span>|<span data-ttu-id="22f66-132">説明</span><span class="sxs-lookup"><span data-stu-id="22f66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f66-133">displayName</span><span class="sxs-lookup"><span data-stu-id="22f66-133">displayName</span></span>|<span data-ttu-id="22f66-134">String</span><span class="sxs-lookup"><span data-stu-id="22f66-134">String</span></span>|<span data-ttu-id="22f66-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22f66-135">Not yet documented</span></span>|
|<span data-ttu-id="22f66-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="22f66-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="22f66-137">Int32</span><span class="sxs-lookup"><span data-stu-id="22f66-137">Int32</span></span>|<span data-ttu-id="22f66-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22f66-138">Not yet documented</span></span>|
|<span data-ttu-id="22f66-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="22f66-139">lastRefreshTime</span></span>|<span data-ttu-id="22f66-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f66-140">DateTimeOffset</span></span>|<span data-ttu-id="22f66-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22f66-141">Not yet documented</span></span>|
|<span data-ttu-id="22f66-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="22f66-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="22f66-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22f66-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="22f66-144">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22f66-144">Not yet documented</span></span>|
|<span data-ttu-id="22f66-145">id</span><span class="sxs-lookup"><span data-stu-id="22f66-145">id</span></span>|<span data-ttu-id="22f66-146">String</span><span class="sxs-lookup"><span data-stu-id="22f66-146">String</span></span>|<span data-ttu-id="22f66-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22f66-147">Key of the entity.</span></span>|
|<span data-ttu-id="22f66-148">version</span><span class="sxs-lookup"><span data-stu-id="22f66-148">version</span></span>|<span data-ttu-id="22f66-149">String</span><span class="sxs-lookup"><span data-stu-id="22f66-149">String</span></span>|<span data-ttu-id="22f66-150">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="22f66-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="22f66-151">応答</span><span class="sxs-lookup"><span data-stu-id="22f66-151">Response</span></span>
<span data-ttu-id="22f66-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22f66-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f66-153">例</span><span class="sxs-lookup"><span data-stu-id="22f66-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f66-154">要求</span><span class="sxs-lookup"><span data-stu-id="22f66-154">Request</span></span>
<span data-ttu-id="22f66-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22f66-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="22f66-156">応答</span><span class="sxs-lookup"><span data-stu-id="22f66-156">Response</span></span>
<span data-ttu-id="22f66-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22f66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




