---
title: managedAppPolicyDeploymentSummary の更新
description: managedAppPolicyDeploymentSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7f7870bad9c7c3154afb4b55212fcb272c391f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354136"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="1b69c-103">managedAppPolicyDeploymentSummary の更新</span><span class="sxs-lookup"><span data-stu-id="1b69c-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="1b69c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b69c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b69c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1b69c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b69c-106">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1b69c-106">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b69c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1b69c-107">Prerequisites</span></span>
<span data-ttu-id="1b69c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b69c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b69c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b69c-110">Permission type</span></span>|<span data-ttu-id="1b69c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b69c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b69c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b69c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b69c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b69c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b69c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b69c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b69c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b69c-115">Not supported.</span></span>|
|<span data-ttu-id="1b69c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b69c-116">Application</span></span>|<span data-ttu-id="1b69c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b69c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b69c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b69c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1b69c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b69c-119">Request headers</span></span>
|<span data-ttu-id="1b69c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b69c-120">Header</span></span>|<span data-ttu-id="1b69c-121">値</span><span class="sxs-lookup"><span data-stu-id="1b69c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b69c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b69c-122">Authorization</span></span>|<span data-ttu-id="1b69c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1b69c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b69c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1b69c-124">Accept</span></span>|<span data-ttu-id="1b69c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b69c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b69c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b69c-126">Request body</span></span>
<span data-ttu-id="1b69c-127">要求本文で、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1b69c-127">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="1b69c-128">次の表に、[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1b69c-128">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="1b69c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b69c-129">Property</span></span>|<span data-ttu-id="1b69c-130">型</span><span class="sxs-lookup"><span data-stu-id="1b69c-130">Type</span></span>|<span data-ttu-id="1b69c-131">説明</span><span class="sxs-lookup"><span data-stu-id="1b69c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b69c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1b69c-132">displayName</span></span>|<span data-ttu-id="1b69c-133">String</span><span class="sxs-lookup"><span data-stu-id="1b69c-133">String</span></span>|<span data-ttu-id="1b69c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b69c-134">Not yet documented</span></span>|
|<span data-ttu-id="1b69c-135">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="1b69c-135">configurationDeployedUserCount</span></span>|<span data-ttu-id="1b69c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1b69c-136">Int32</span></span>|<span data-ttu-id="1b69c-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b69c-137">Not yet documented</span></span>|
|<span data-ttu-id="1b69c-138">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="1b69c-138">lastRefreshTime</span></span>|<span data-ttu-id="1b69c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b69c-139">DateTimeOffset</span></span>|<span data-ttu-id="1b69c-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b69c-140">Not yet documented</span></span>|
|<span data-ttu-id="1b69c-141">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="1b69c-141">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="1b69c-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b69c-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="1b69c-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1b69c-143">Not yet documented</span></span>|
|<span data-ttu-id="1b69c-144">id</span><span class="sxs-lookup"><span data-stu-id="1b69c-144">id</span></span>|<span data-ttu-id="1b69c-145">文字列</span><span class="sxs-lookup"><span data-stu-id="1b69c-145">String</span></span>|<span data-ttu-id="1b69c-146">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1b69c-146">Key of the entity.</span></span>|
|<span data-ttu-id="1b69c-147">version</span><span class="sxs-lookup"><span data-stu-id="1b69c-147">version</span></span>|<span data-ttu-id="1b69c-148">String</span><span class="sxs-lookup"><span data-stu-id="1b69c-148">String</span></span>|<span data-ttu-id="1b69c-149">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1b69c-149">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1b69c-150">応答</span><span class="sxs-lookup"><span data-stu-id="1b69c-150">Response</span></span>
<span data-ttu-id="1b69c-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1b69c-151">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b69c-152">例</span><span class="sxs-lookup"><span data-stu-id="1b69c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b69c-153">要求</span><span class="sxs-lookup"><span data-stu-id="1b69c-153">Request</span></span>
<span data-ttu-id="1b69c-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1b69c-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b69c-155">応答</span><span class="sxs-lookup"><span data-stu-id="1b69c-155">Response</span></span>
<span data-ttu-id="1b69c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1b69c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






