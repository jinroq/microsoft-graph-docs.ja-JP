---
title: managedDeviceMobileAppConfigurationDeviceSummary の更新
description: managedDeviceMobileAppConfigurationDeviceSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5672fa78f041967064425520a1df5cb52c6ff15c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412668"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="9c930-103">managedDeviceMobileAppConfigurationDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="9c930-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="9c930-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c930-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9c930-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c930-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c930-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9c930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c930-107">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9c930-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c930-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9c930-108">Prerequisites</span></span>
<span data-ttu-id="9c930-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c930-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9c930-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c930-111">Permission type</span></span>|<span data-ttu-id="9c930-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c930-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c930-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c930-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c930-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c930-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c930-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c930-116">Not supported.</span></span>|
|<span data-ttu-id="9c930-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c930-117">Application</span></span>|<span data-ttu-id="9c930-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c930-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c930-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="9c930-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c930-120">Request headers</span></span>
|<span data-ttu-id="9c930-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c930-121">Header</span></span>|<span data-ttu-id="9c930-122">値</span><span class="sxs-lookup"><span data-stu-id="9c930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c930-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c930-123">Authorization</span></span>|<span data-ttu-id="9c930-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9c930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c930-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c930-125">Accept</span></span>|<span data-ttu-id="9c930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c930-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c930-127">Request body</span></span>
<span data-ttu-id="9c930-128">要求本文で、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c930-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="9c930-129">次の表に、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9c930-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="9c930-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c930-130">Property</span></span>|<span data-ttu-id="9c930-131">型</span><span class="sxs-lookup"><span data-stu-id="9c930-131">Type</span></span>|<span data-ttu-id="9c930-132">説明</span><span class="sxs-lookup"><span data-stu-id="9c930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c930-133">id</span><span class="sxs-lookup"><span data-stu-id="9c930-133">id</span></span>|<span data-ttu-id="9c930-134">String</span><span class="sxs-lookup"><span data-stu-id="9c930-134">String</span></span>|<span data-ttu-id="9c930-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9c930-135">Key of the entity.</span></span>|
|<span data-ttu-id="9c930-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="9c930-136">pendingCount</span></span>|<span data-ttu-id="9c930-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-137">Int32</span></span>|<span data-ttu-id="9c930-138">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-138">Number of pending devices</span></span>|
|<span data-ttu-id="9c930-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9c930-139">notApplicableCount</span></span>|<span data-ttu-id="9c930-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-140">Int32</span></span>|<span data-ttu-id="9c930-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="9c930-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="9c930-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="9c930-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-143">Int32</span></span>|<span data-ttu-id="9c930-144">一致していないプラットフォームとポリシーが適用されないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="9c930-145">successCount</span><span class="sxs-lookup"><span data-stu-id="9c930-145">successCount</span></span>|<span data-ttu-id="9c930-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-146">Int32</span></span>|<span data-ttu-id="9c930-147">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="9c930-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="9c930-148">errorCount</span></span>|<span data-ttu-id="9c930-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-149">Int32</span></span>|<span data-ttu-id="9c930-150">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-150">Number of error devices</span></span>|
|<span data-ttu-id="9c930-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="9c930-151">failedCount</span></span>|<span data-ttu-id="9c930-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-152">Int32</span></span>|<span data-ttu-id="9c930-153">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-153">Number of failed devices</span></span>|
|<span data-ttu-id="9c930-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9c930-154">conflictCount</span></span>|<span data-ttu-id="9c930-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-155">Int32</span></span>|<span data-ttu-id="9c930-156">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9c930-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="9c930-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9c930-157">lastUpdateDateTime</span></span>|<span data-ttu-id="9c930-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c930-158">DateTimeOffset</span></span>|<span data-ttu-id="9c930-159">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="9c930-159">Last update time</span></span>|
|<span data-ttu-id="9c930-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="9c930-160">configurationVersion</span></span>|<span data-ttu-id="9c930-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9c930-161">Int32</span></span>|<span data-ttu-id="9c930-162">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="9c930-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="9c930-163">応答</span><span class="sxs-lookup"><span data-stu-id="9c930-163">Response</span></span>
<span data-ttu-id="9c930-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9c930-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c930-165">例</span><span class="sxs-lookup"><span data-stu-id="9c930-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c930-166">要求</span><span class="sxs-lookup"><span data-stu-id="9c930-166">Request</span></span>
<span data-ttu-id="9c930-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9c930-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c930-168">応答</span><span class="sxs-lookup"><span data-stu-id="9c930-168">Response</span></span>
<span data-ttu-id="9c930-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9c930-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




