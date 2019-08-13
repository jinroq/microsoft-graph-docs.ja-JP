---
title: managedDeviceMobileAppConfigurationDeviceSummary の更新
description: managedDeviceMobileAppConfigurationDeviceSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9bd35add678c40a7f79e42994b0cf1c512d3d979
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329769"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="293b2-103">managedDeviceMobileAppConfigurationDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="293b2-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="293b2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="293b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="293b2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="293b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="293b2-106">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="293b2-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="293b2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="293b2-107">Prerequisites</span></span>
<span data-ttu-id="293b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="293b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="293b2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="293b2-110">Permission type</span></span>|<span data-ttu-id="293b2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="293b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="293b2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="293b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="293b2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="293b2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="293b2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="293b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="293b2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="293b2-115">Not supported.</span></span>|
|<span data-ttu-id="293b2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="293b2-116">Application</span></span>|<span data-ttu-id="293b2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="293b2-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="293b2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="293b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="293b2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="293b2-119">Request headers</span></span>
|<span data-ttu-id="293b2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="293b2-120">Header</span></span>|<span data-ttu-id="293b2-121">値</span><span class="sxs-lookup"><span data-stu-id="293b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="293b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="293b2-122">Authorization</span></span>|<span data-ttu-id="293b2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="293b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="293b2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="293b2-124">Accept</span></span>|<span data-ttu-id="293b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="293b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="293b2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="293b2-126">Request body</span></span>
<span data-ttu-id="293b2-127">要求本文で、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="293b2-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="293b2-128">次の表に、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="293b2-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="293b2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="293b2-129">Property</span></span>|<span data-ttu-id="293b2-130">型</span><span class="sxs-lookup"><span data-stu-id="293b2-130">Type</span></span>|<span data-ttu-id="293b2-131">説明</span><span class="sxs-lookup"><span data-stu-id="293b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="293b2-132">id</span><span class="sxs-lookup"><span data-stu-id="293b2-132">id</span></span>|<span data-ttu-id="293b2-133">String</span><span class="sxs-lookup"><span data-stu-id="293b2-133">String</span></span>|<span data-ttu-id="293b2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="293b2-134">Key of the entity.</span></span>|
|<span data-ttu-id="293b2-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="293b2-135">pendingCount</span></span>|<span data-ttu-id="293b2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-136">Int32</span></span>|<span data-ttu-id="293b2-137">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-137">Number of pending devices</span></span>|
|<span data-ttu-id="293b2-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="293b2-138">notApplicableCount</span></span>|<span data-ttu-id="293b2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-139">Int32</span></span>|<span data-ttu-id="293b2-140">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="293b2-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="293b2-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="293b2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-142">Int32</span></span>|<span data-ttu-id="293b2-143">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="293b2-144">successCount</span><span class="sxs-lookup"><span data-stu-id="293b2-144">successCount</span></span>|<span data-ttu-id="293b2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-145">Int32</span></span>|<span data-ttu-id="293b2-146">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="293b2-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="293b2-147">errorCount</span></span>|<span data-ttu-id="293b2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-148">Int32</span></span>|<span data-ttu-id="293b2-149">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-149">Number of error devices</span></span>|
|<span data-ttu-id="293b2-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="293b2-150">failedCount</span></span>|<span data-ttu-id="293b2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-151">Int32</span></span>|<span data-ttu-id="293b2-152">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-152">Number of failed devices</span></span>|
|<span data-ttu-id="293b2-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="293b2-153">conflictCount</span></span>|<span data-ttu-id="293b2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-154">Int32</span></span>|<span data-ttu-id="293b2-155">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="293b2-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="293b2-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="293b2-156">lastUpdateDateTime</span></span>|<span data-ttu-id="293b2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="293b2-157">DateTimeOffset</span></span>|<span data-ttu-id="293b2-158">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="293b2-158">Last update time</span></span>|
|<span data-ttu-id="293b2-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="293b2-159">configurationVersion</span></span>|<span data-ttu-id="293b2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="293b2-160">Int32</span></span>|<span data-ttu-id="293b2-161">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="293b2-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="293b2-162">応答</span><span class="sxs-lookup"><span data-stu-id="293b2-162">Response</span></span>
<span data-ttu-id="293b2-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="293b2-163">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="293b2-164">例</span><span class="sxs-lookup"><span data-stu-id="293b2-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="293b2-165">要求</span><span class="sxs-lookup"><span data-stu-id="293b2-165">Request</span></span>
<span data-ttu-id="293b2-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="293b2-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="293b2-167">応答</span><span class="sxs-lookup"><span data-stu-id="293b2-167">Response</span></span>
<span data-ttu-id="293b2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="293b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```






